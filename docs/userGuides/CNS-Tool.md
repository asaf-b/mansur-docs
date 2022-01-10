###User-Guide
This tool was created to allow animators to create offset additional control for any control within block rig, if they have a need to constrain the control to a different object.
<br>
Often, animators need to constrain a control to a different object to create the required animation. Since this operation will result in locking the control's transform channels, it is neccessary to create an aditional offset control above in order to constrain the offset control, maintaining animation ability on the child control.
<br>
This tool is operational both in normal rig state as well as in a referenced rig state.

####UI
Access this Tool via Mansur-Rig main Maya menu
<figure>
  <img src="../userGuidesImages/CNSTool/CNSToolMenuItem.png"/>
  <figcaption>Menu Entry</figcaption>
</figure>

####Workflow
<ol>
  <li>Open the tool. The UI will list all existing CNS controls within the scene.</li>
  <li>Select any control and click <b><i>Create CNS</i></b>(1). This will create the offset CNS, maintining the selected control's transforms.</li>
  <li>In case you want to remove an existing CNS, use <b><i>Remove CNS</i></b>(2).</li>
</ol>

####Legend
<figure>
  <img src="../userGuidesImages/CNSTool/CNSToolLegend.png"/>
  <figcaption>CNS Tool- UI</figcaption>
</figure>

<ol>
  <li>
    <b><i>Create CNS</b></i>- Create a CNS for selected controls.
  </li>
  <li>
    <b><i>Delete CNS</b></i>- Delete an existing CNS for selected controls.
  </li>
  <li>
    <b><i>Scene CNS Controls</b></i>- Existing scene CNS controls display.
  </li>
</ol>

