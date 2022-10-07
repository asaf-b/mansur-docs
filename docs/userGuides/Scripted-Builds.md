If you need to operate on Block rigs externaly, use this article to guide you through the few simple Python commands in order to do so.
In some cases, you may need to operate on Block rigs extarnaly, without using Block UI. Use the simple steps described below to operate on any rig using python commands.

#### Mansur-Rig Python Libraries
In order to use Mansur-Rig's external commands, you'll first need to import the Python module containing the methods.

=== "Python module import"

    ``` python
    from mansur.block.core import blockUtility as blkUtils
    ```

This simple import command will import Mansur-Rig's Block-Utility library, which contains the methods you'll require.

#### Global methods
Use these methods to operate on Block Rig's or specific components within it:

<ul>
  <li> 
    <b>gatherMnsRigObject()</b> - Use this command to gather a MnsRig class object to operate on.
  </li>
  <li>
    <b>collectPartialModules()</b> - Most of Block's main methods can operate on an entire rig, as well as module branches, and indevidual modules.
    <br>
    In order to utelize this ability, use this method to collect the modules you want to operate on.
    <br>
    This method will collect module root objects based on the input data.
    In case fromNodes argument is Null, this method will return data based on the current scene selection.
    <br>
    fromNodes is a list argument. 
    In case any input is passed, this method will attempt to aquire the modules to construct based on the mode selected.
    You can pass in any Block-Node names into this method.
    <br>
    mode 0 = ALL
    <br>
    mode 1 = Branch
    <br>
    mode 2 = Module
  </li>
  <li>
    <b>constructRig(fromNodes = [], mode = 0)</b> - Use this simple command to construct a rig using a Python command.
  </li>
  <li>
    <b>deconstructRig(fromNodes = [], mode = 0)</b> - Use this simple command to deconstruct a rig using a Python command.
  </li>
</ul>

#### Examples

=== "Constructing a Rig from selection"

    ``` python
    # Library import
    from mansur.block.core import blockUtility as blkUtils

    #construct command with default arguments- selection based(fromNodes = Null, mode = 0)
    blkUtils.constructRig()
    ```

<br>

=== "Constructing a Specific Rig based on a Rig-Top node name"

    ``` python
    # Library import
    from mansur.block.core import blockUtility as blkUtils

    #construct command with input fromNodes argument, with default construction mode = 0
    blkUtils.constructRig("c_maleDummy_A001_blkRig")
    ```

<br>

=== "Constructing a Specific Rig based on a Rig-Top node name, in branch mode"

    ``` python
    # Library import
    from mansur.block.core import blockUtility as blkUtils

    #construct command with input fromNodes argument, with branch construction mode = 1
    blkUtils.constructRig("c_maleDummy_A001_blkRig", 1)
    ```

<br>

=== "Constructing a single component of a rig"

    ``` python
    # Library import
    from mansur.block.core import blockUtility as blkUtils

    #construct command with input fromNodes argument, with module construction mode = 2
    blkUtils.constructRig("l_arm_A001_rCtrl", 2)
    ```

<br>

=== "Deconstructing a Rig from selection"

    ``` python
    # Library import
    from mansur.block.core import blockUtility as blkUtils

    #construct command with default arguments- selection based(fromNodes = Null, mode = 0)
    blkUtils.deconstructRig()
    ```

<br>

#### Altering Module settings via the API
<ol>
    <li>Some settings require an action post change (like joint structure members), so changing the attributes only isn't sufficiant, you need to run an update command.</li>
    <li>The update command has a few requirements - settings update need to come in a dictionary format, passed in with a double asterisk (**) keyword arguments. The settings must contain a "settingsHolder" definition, which is the root guide, a "rigTop" which is the rig top node, and "originalArguments" dictionary that define the settings format, in order to update the module correctly.</li>
    <li>Some settings have very specific data format (like channel control) and you'll need to be very accurate when changing settings of this type.</li>
</ol>

=== "Altering Module settings via the API"
    
    ``` python
    # Libraries import
    from mansur.block import blockBuildUI
    from mansur.core import utility as mnsUtils
    blockWin = blockBuildUI.MnsBlockBuildUI()
    
    #defining mandatory variables for the update settings command
    rigTop = mnsUtils.validateNameStd("c_blkChar_A001_blkRig")
    rootGuide = mnsUtils.validateNameStd("c_FKChain_A001_rCtrl")
    origArgs, split = blockWin.getModuleSettings(rootGuide)
    
    #creating the settings dictionary
    settings = {"settingsHolder": rootGuide, #mandatory
                "origArgs": origArgs, #mandatory
                "rigTop": rigTop, #mandatory
                "doInterpolationJoints": True, #exmaple change
                "interpolationJoints": 10} #example change
    
    #running the update command
    blockWin.updateSettings(**settings)
    ```

In this example, I created an FK chain module with all default settings.
<br>
Now I want to update the settings and change "doInterpJoints" and the number of interpJoints.
<br>
I passed all required data, and then the settings I want to change.
<br>
Once you run this code, you'll see that not only the attributes have changed, the joint structure is being rebuilt correctly as these are jointStruct members attributes.