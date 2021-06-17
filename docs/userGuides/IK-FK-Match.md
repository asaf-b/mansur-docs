### How To Match Limb Module IK & FK Controls
In order to switch & match IK and FK controls of a limb module, please use the following code snippets.
The following code is selection based. Select any control related to the limb module you want to switch and run the method.

- <b>Mode 0:</b> Match IK Controls to the FK controls
- <b>Mode 1:</b> Match FK Controls to the IK controls

=== "IK to FK (Python)"

    ``` python
    #import Mansur-Rig's Block-Utility python module, to access the method    
    from mansur.block.core import blockUtility as blkUtils

    #Mode 0 - Match IK to FK
	blkUtils.limbMatchFkIK(pm.ls(sl=True)[0], 0)
    ```

=== "FK to IK (Python)"

    ``` python
    #import Mansur-Rig's Block-Utility python module, to access the method    
    from mansur.block.core import blockUtility as blkUtils

    #Mode 1 - Match FK to IK
	blkUtils.limbMatchFkIK(pm.ls(sl=True)[0], 1)
    ```

### Using the code snippet as a picker button
In case you are creating a picker, it is recommended to add FK & IK switch buttons for easy access in animation.
The way to do so is simply to insert the above snippets as a "custom script" into a picker button.

1. Open Block Builder, and move to "Picker" tab.
<figure>
  <img src="../userGuidesImages/ikfk/pickerTab.png">
  <figcaption>Picker Tab</figcaption>
</figure>
2. While any control is selected, click "Edit Picker Layout" to open the picker layout editor.
3. Click "Create Free PLG" to create a new free picker button, and position it within your picker layout.
4. While the new PLG is selected, click "PLG Settings" to open it's attributes.
5. In the opened UI, insert any of the above code snippets.
6. Optionally add a text in the "button text" line edit to indicate it's behaviour- for example: "To FK" or "To IK".
7. Optionally add the Module's UI control into the controls select list.
<figure>
  <img src="../userGuidesImages/ikfk/ikFKPLGSettings.png">
  <figcaption>PLG Settings</figcaption>
</figure>
8. Repeat the process for the reverse operation.
9. test the buttons by openning the picker, and clicking the button.

<figure>
  <img src="../userGuidesImages/ikfk/ikFKSwitch.gif">
  <figcaption>Result Example</figcaption>
</figure>