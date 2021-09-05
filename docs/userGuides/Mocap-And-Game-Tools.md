Mansur-Rig is equipped with a full toll-set to manage Mocap data as well as manipulate rigs to be game-engine ready.
<br>
This guide will cover the entire tool-set, and some example use-scenarions/workflows.
<br>
<hr>

###Block Builder- Mocap/Game tab
<figure>
  <img src="../userGuidesImages/mocap/mocap-legend.png"/>
  <figcaption>Mocap Tab Legend</figcaption>
</figure>
<hr>

####Offset-Rig Section
<ol>
  <li>
    <b>Guide Preset section</b>- Mnausr-Rig is delivered with pre-existing guide presets for ease of use. Use the <b>Import</b> button to gather the guide prset of you choice.
  </li>
  <li>
    <b>Create Offset Rig</b>- A Block-Offset-Rig, is a joint skeleton, created from the base joint-structure, that can be used to control the puppet. In essence reversing the puppet structure. Instead of the puppet controling the skeleton, this new skeleton will control the puppet. The puppet will of course still control the base-skeleton which drives the deformations. This behaviour is used to import mocap data onto the offset skeleton, which drives the puppet. This in turn will allow you to bake the animation into the puppet-controls- for post-editting the animation/cleanup, mainaing the kinematics of the puppet.
    <br>
    The joint-control relationship is set within Block's internal contruct process, so you don't need to define it, the offset skeleton will know how to connect to the puppet automatically.
    <br>
    Note that the control isn't automatically transferred- use <b>Authority To Skeleton</b>(4).
  </li>
</ol>

<figure>
  <img src="../userGuidesImages/mocap/offsetSkelDemo.png"/>
  <figcaption>Offset Skeleton Example</figcaption>
</figure>

<ol start = "2">
  <li>
    <b>Delete Offset Rig</b>- Delete the Offset-Rig, if it exists.
  </li>
  <li>
    <b>Authority To Skeleton</b>- Use this utilty to constrain the puppet controls to the offset-Skeleton. Make sure the puppet and offset-skeleton are in the same pose.
  </li>
  <li>
    <b>Authority To Puppet</b>- If the puppet controls are constrained to the offset skeleton, use this utility to release that connection, restorinng normal bahvaviour.
  </li>
  <li>
    <b>Select Slave Controls</b>- Select all controls that are set to be driven by the offset-rig connection.
  </li>
  <li>
    <b>Bake Controls</b>- Bake the slave controls, within the current animation range. 
    <br>
    If require further bakinng options, use <b>Select Slave Controls</b>(6) to select the slave controls, then use Maya's Bake-Animation utility.
  </li>
</ol>
<hr>

####Utilities Section

<ol start = "8">
  <li>
    <b>Rest Puppet</b>- Reset all puppet controls. 
  </li>
  <li>
    <b>Rest Offset-Rig</b>- Reset the offset-skeleton.
  </li>
  <li>
    <b>Joint Rotate To Orient</b>- Attempt to transfer all joint rotation values into the joint orient values, to "zero out" the rotation values. This action will be performed on the entire seleted heirarchy. 
  </li>
</ol>
<hr>

####Character Definition Section

<ol start = "11">
  <li>
    <b>Character Definition</b>- Load the Character-Definition Tool- which will allow you to charactraize your pupprts/skeletons into HumanIK, in order to retarget mocap data.
  </li>
</ol>
<hr>

####Extract Skeleton Section
<ol start = "12">
  <li>
    <b>Extract Skeleton</b>- Use this utility to easily extract your puppet's skeleton, in order to export it.
    <br>
    Once you extracted your skeleton, you will be able to delete Block's rig, leaving only the skeleton (with or without animation) and your geometry (with it's deformation). This will make exporting using any tool of your choosing fast and easy.
  </li>
  <li>
    <b>Snap Extracted Skeleton To Base</b>- Match extracted skeleton transformations to the base skeleton
  </li>
  <li>
    <b>Pose Edit Section</b>- Use these utilities to save\load dagPoses onto your extracted skeleton.
  </li>
</ol>

<hr>

###Character Definition Tool
This tool was created to enhance mocap data retargeting to Block rigs.
<br>
Using this tool, you can easily Characterize your puppets into Maya's Human-IK tool.
<br>
The goal behind this tool is to speed up your motion-capture data import workflow.
<br>
Not only Mansur-Rig is equipped with many mocap-data presents, it will also allow you to create custom presets easily and export them to re-use.


<figure>
  <img src="../userGuidesImages/mocap/charDefUILegend.png"/>
  <figcaption>Character Definition UI Legend</figcaption>
</figure>

<hr>
####Presets import/Export
<ol>
  <li>
    <b>Presets dropdown</b>- Choose a predefined naming preset to import.
  </li>
  <li>
    <b>Target Column dropdown</b>- Choose which column to import the preset to, or export from. 
    <br>
    <b>Humak-IK</b> column will be exported always along side the column selected.
  </li>
  <li>
    <b>Import</b>- Improt from the predifined preset selecter, into the selected column.
  </li>
  <li>
    <b>Import From File</b>- Improt from a custom preset file exported previously, into the selected column.
  </li>
  <li>
    <b>Export</b>- Export the select column, as well as it's related Human-IK defintion into a file. 
    <br>
    Use this preset later-on using the <b>Import From File</b>(4) utility.
  </li>
</ol>

<hr>
####Display Settings
<ol start = "6">
  <li>
    <b>Filter</b>- Filter UI display to easily find the component you are after.
  </li>
  <li>
    <b>Update Selection</b>- When this checkbox is ON, the main scene selection will update based on the selected rows, in case any of the objects within it exists. 
    <br>
    When OFF, scene selection will not be changed.
  </li>
  <li>
    <b>Reset UI</b>- Clear the entire UI.
  </li>
</ol>

<hr>
####Data Section
<ol start = "9">
  <li>
    <b>Data Viewer</b>- This is where all of the data is displayed.
    <br>
    Data in this UI can be editted, not only viewed.
    <br>
    In case you need to create a preset, you can always start with a similar preset and edit it to your needs to avoid creating it from scratch.
    <br>
    <b>Right-Click</b>- Edit menu
    <br>
    <b>Double-Click</b>- Free edit
    <br><br>
    <b><i>Column description</i></b>
    <ul>
      <li>
        <b>Component Column</b>- This culomn is the name of the component. This name is entirly up to you- it is simply an indetifier for the row.
      </li>
      <li>
        <b>Block Skeleton Column</b>- This column represent the Block joint related to this component row.
        <br>
        Objects in this Column must be from Block's rig base skeleton- NOT the offset-skeleton.
      </li>
      <li>
        <b>Target Skeleton Column</b>- This column represets a joint from an external source (not block). 
        <br>
        The target skeleton may be a skeleton you wish to retarget data from, or retarget data to.
        <br>
        This skeleton can be any skeleton. 
        <br>
        In case a preset doesn't exist for your target skeleton, you can always create a custom one yourself.
      </li>
      <li>
        <b>Human-IK Column</b>- This column represents the Human-IK slot this row is related to.
        <br>
        Since Human-IK slots are pre-defined, this column can not be editted freely.
        <br>
        Please use the right-click menu to access all Human-IK slots.
      </li>
    </ul>
  </li>
  <li>
    <b>Name-Sapces</b>- In case your target/block contain a namespace, input it into the correct boxed.
    <br>
    In case a namespace exists for a target/block skeleton and they are not inputed correctly, the objects won't be found and the characterazation process will fail.
    <br>
    For ease, simply select one of your name-spaced objects and press the arrow button to the right of the box you want to input it to.
  </li>
</ol>

<hr>
####Match Section
In case you have a skeleton you wish to animate (Metahuman for example), and you need a puppet for it, you can use this section.
<ol start = "11">
  <li>
    <b>Match Block Guides To Target</b>- Match the Block guides position to the target skeleton.
    <br>
    Simply input all of the data into the UI, using presets/edit, while your Block-skeleton column is set to an existing Block-Rig (in deconstructed state), and match the guides' position to the target skeleton you want to animate.
    <br>
    Once again, The Block column input should contain base skeleton objects.
    <br>
    When using this utility, the system will find the correct guides automatically.
    <br>
    Then, you can construct your rig to aquire a fully functioning puppet.
    <br>
    Then simply use <b>Connect Target Skeleton</b>(12) to connect your target skeleton to the base skeleton.
    <br>
    Now you have a fully functional animation puppet you can animate your skeleton with.
  </li>
  <li>
    <b>Connect Target Skeleton</b>- Connect a Block puppet to the target skeleton in order to animate.
  </li>
  <li>
    <b>Disconnect Target Skeleton</b>- Break the connection between Blok puppet and the target skeleton (if exists).
    <br>
    When you finish animating, you can simply bake your target skeleton animation, disconnect the connection to Block's puppet.
  </li>
</ol>

####Match Section

<hr>
####Human-IK section
<ol start = "14">
  <li>
    <b>Humak-IK UI</b>- Open Maya's Human-IK tool.
  </li>
  <li>
    <b>Characterize</b>- Create a Human-IK character definition based on the current data.
    <br>
    You can do this for both Block skeleton and the target skeleton.
    <br>
    This process will create a new character definition in Human-IK, and attempt the connect all objects to their related slot within that character definition.
  </li>
</ol>