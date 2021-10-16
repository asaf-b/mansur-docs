###User-Guide
Create volume joints to refine and enhence you deformations. These joints are driven by 2 parent & child joints. Using the new UI, you can choose actions (translation/scale) to take for every angle direction between the 2 joint drivers.

####Example
<figure>
  <img src="../userGuidesImages/volumeJoints/vJnts_demo.gif"/>
  <figcaption>Volume-Joints- Example</figcaption>
</figure>

####UI
Access this UI via Mansur-Rig main Maya menu
<figure>
  <img src="../userGuidesImages/volumeJoints/menuItem.png"/>
  <figcaption>Menu Entry</figcaption>
</figure>


####Legend
<figure>
  <img src="../userGuidesImages/volumeJoints/vJointsLegend.png"/>
  <figcaption>Volume-Joints- UI</figcaption>
</figure>

<ol>
<li>
  <b><i>Volume-Joint List</b></i>- List of all Volume joints within the current scene. Use the <b><i>Refresh(4)</i></b> button to refresh.
</li>
<li>
  <b><i>Create</b></i>- Creation button.
  <br>This will create a volume joint, based on the current scene selection. 
  <br>The selected object should be the "child" item- meaning, if you want to create a volume joint for a knee, select an object relating to the <b>lower</b> leg section. This will create a volume joint between the upper-leg, and lower leg. 
  <br>Valid selection object types are- Joints, Guides, Ctrls. In case a joint wasn't selected, the system will attemp to retreive the joint related to the selection. If the system did not find a related joint, nothing will be created. 
  <br><b>Important note</b>: Volume joints have a "Rest state"- which is the base state or "Zero" state- where nothing is triggered- when creating a volume joint, the current state will be set as the rest state. In case you want to update the rest position, use the "Set current as rest position" button undeer the General tab when the requested volume-joint is selected.</b>
  <br>In case <b><i>Auto-Symmetry(7)</i></b> is selected, the system will attempt to create a symmetrical volume-joint (if relevant).
  <br>The amount of Volume-Joints is <b>unlimited</b>.
</li>
<li>
  <b><i>Delete</b></i>- Delete the selected volume joint.
  <br>In case <b><i>Auto-Symmetry(7)</i></b> is selected, the system will attempt to delete the symmetrical volume-joint (if one exists).
</li>
<li>
  <b><i>Refresh</b></i>- Refresh the UI. Rescan the current scene.
</li>
<li>
  <b><i>Symmetrize</b></i>- Attempt to create/update a symmetrical volume joint based on the selected colume joint. 
</li>
<li>
  <b><i>Symmetrize ALL</b></i>- Attempt to create/update ALL volume joints in the scene.
</li>
<li>
  <b><i>Auto-Symmetry</b></i>- In case this is checked ON, all actions will attempt to symmetrize.
  <br>That includes- Creation, Deletion, Symmetry, any value edit.
  <br>This is recommended to be kept on.
</li>
<li>
  <b><i>Current-State-Display</b></i>- This section was design to minimize confusion when dealing with volume joints. 
  <br>Based on the UI-selected volume joint, this display will update based on the current state of the angle relationship between the two master (source) joints.
  <br>When editting a volume joint's behaviour, it is very convenient to visually determine the current angle state the sources are in.
  <br>Since the angles are based on the guide's original orientation, this changes between modules.
  <br>For example, if you need to create a volume joint for an elbow, create it in rest-state, the "bend" the elbow- the display will indicate which direction the elbow bend is set to, so you can open the correct dropdown menu to edit the behaviour.
</li>
<li>
  <b><i>Edit Section</b></i>- This is where the behaviour for each volume joint is set.
  <ul>
    <li>
      General Section- 
      <ul>
        <li>
          <i><b>Rotation-Blend</b></i> attribute, which will determine the orientation blend between the parent and the child joints for the selected volume joint.
        </li>
        <li>
          <i><b>Set Current As Rest</b></i> utility.
        </li>
      </ul>
    </li>
    <li>
      Rest Section-
      <ul>
        <li>
          <i><b>Rest-Translation</b></i> attributes
        </li>
      </ul>
    </li>
    <li>
      All Angle Sections-
      <ul>
        <li>
          <i><b>Translation-Target</b></i> attributes
        </li>
        <li>
          <i><b>Scale-Target</b></i> attributes
        </li>
        <li>
          <i><b>Translation-Limit</b></i> attributes
        </li>
        <li>
          <i><b>Scale-Limit</b></i> attributes
        </li>
        <li>
          <i><b>Current Values</b></i> display
        </li>
      </ul>
    </li>
  </ul>
</ol>
