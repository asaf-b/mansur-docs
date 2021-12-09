This simple animation tool was created to allow animators to space switch and IK->FK switch easily.
<br>
This tool is selection based. Please select controls to enable relevant capabilities.
<br>
For spaces, simply select the controls you want to act upon, choose your target spaces, and press "switch". This will switch the space, while maintaining the controls's transforms, using keys created automatically.
<br>
For Limbs, simply select any control/s for the limbs that you wish to act upon, and press the relevant button- To-IK or To-FK.
<br>
This will switch the limb/controls to the selected state. 
This tool also includes Auto-Key switches, as well as a sequence and bake modes.
<br>
<hr>

###Spaces/IK-FK Tool Load
<figure>
  <img src="../userGuidesImages/spacesTool/spacesToolLoad.png"/>
  <figcaption>Spaces/FK-IK Tool Menu Item</figcaption>
</figure>
<hr>

###How to use
The spaces tool is quite standard, but if ever you get confused, here are a few guidelines.
<br>
<figure>
  <img src="../userGuidesImages/spacesTool/spacesToolLegend.png"/>
  <figcaption>Spaces/FK-IK Tool Legend</figcaption>
</figure>
<br>
<ol>
  <li><b><i>Auto-Key Button</b></i> - When this button is checked, keys will be inserted automatically when performing actions.</li>
  <li><b><i>Bake Button</b></i> - When this button is checked, the auto-key button is checked, and the sequence mode is selected, every frame within the frame range selected will be keyed- "baking" the switch for the selected frame-range,</li>
  <li><b><i>Current-Frame/Sequence Mode</b></i> - In case the "Current-Frame" mode is selected, any action will be performed on the current frame selected. In case "Sequence" mode is selected, any action will be performed on the selected frame-range.</li>
  <li><b><i>Frame-Range Section</b></i> - This section will determine the frame range to act upon, when "Sequence" is selected.</li>
  <li><b><i>Spaces/IK-FK Tabs</b></i> - This tool has two modes- Spaces, and IK-FK. Choose the relevant tab based on the action you are interested in. Please read the two next bullets (6A & 6B) for additional information on both modes.</li>
  <li>Tool Modes:
    <ol type="A">
      <li><b><i>Spaces-Mode</b></i> - This mode is for switching control spaces. In contrast of switching a space using the channel box, this tool will switch to the selected space while maintaining the control's transform.
        <ul>
          <li><b><i>On Current-Frame Mode</b></i> - The space of the control will be switched for the current frame, maintaining the control's transform. When "Auto-Key" button is checked, a key of the current frame will be inserted automatically.</li>
          <li><b><i>On Sequence Mode:</b></i>
            <ul>
              <li><b>On Non-Bake mode:</b>  - A key will be inserted for every frame the space-switch attribute in question has a key, within the selected range. The current tranform for the control/s in question will be maintained.</li>
              <li><b>On Bake mode:</b>  - A key will be inserted for every frame within the selected range. The current tranform for the control/s in question (at the relevant frame) will be maintained- "Baking" the switch.</li>  
            </ul>
          </li>
        </ul>
      </li>
      <li><b><i>IK-FK-Mode</b></i> - This mode is for switching IK-FK modes for limbs.  In contrast of switching FK-IK modes for limbs using the channel box, this tool will switch to the selected kinematics while maintaining the limb controls' transforms.</li>
        <ul>
          <li><b><i>On Current-Frame Mode</b></i> - The kinematic state of the limb will be switched for the current frame, maintaining the limb controls' transform. When "Auto-Key" button is checked, a key of the current frame will be inserted automatically.</li>
          <li><b><i>On Sequence Mode:</b></i>
            <ul>
              <li><b>On Non-Bake mode:</b>  - A key will be inserted for every frame the kinematic-switch attribute in question has a key, within the selected range. The current limb controls' in question will be maintained.</li>
              <li><b>On Bake mode:</b>  - A key will be inserted for every frame within the selected range. The current limb controls' in question (at the relevant frame) will be maintained- "Baking" the switch.</li>
              <li><b>Select Host:</b>  - Select the kinematic switch attribute control holder for the selected limb modules.</li>  
            </ul>
          </li>
        </ul>
    </ol>
  </li>
</ol>