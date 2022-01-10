###User-Guide
LODs Tool is a simple way for managing visibility switches between model states.
<br>
Often, a given model has different states, or different resolutions, which can be switched while animating to gain performance. These states are most commonly known as LOD (Level-Of-Detail) modes.
<br>
Using this tool you can simply create LOD grouping (as many as you need) and input transforms into these groups to switch visibility states using a simple Enum attribute that will be created automatically (both in deconstructed and constructed states of Block rig).
<br>
This tool can also be used to switch between model variations, or clothing variations of a model.

####UI
Access this Tool via Mansur-Rig main Maya menu
<figure>
  <img src="../userGuidesImages/LODsTool/LODsMenuItem.png"/>
  <figcaption>Menu Entry</figcaption>
</figure>

####Workflow
<ol>
  <li>Open the tool.</li>
  <li>Select any component of a Block rig. If any previous LOD setting were created for this rig, they will be displayed within the UI. If not, only the <i><b>Rig</b></i>(1) indication will display the name of the selected rig.</li>
  <li>Start with adding a LOD group by clicking <i><b>Add LOD</b></i>(6). A new LOD column will be created in the <b><i>LOD groups section</i></b>(5).</li>
  <li>Repeat the previous step to add more LOD groups (columns).</li>
  <li>Use the <i><b>Right-Click Menu</i></b>(8-11) (using right click in the LOD groups section) to edit the contents of each group (selection based). Any transfom can be added here.</li>
  <li>Once you are done editting your LOD groups, click <b><i>Apply Changes</i></b>. This will write the data into the rig, and UI will refresh.</li>
  <li>Now you should see that the <b><i>Current LOD</i></b>(2) drop-down now contains an item for each LOD group you selected. You will also notice that the visibility channels for the nodes you selected are already connected. Using the <i><b>Current LOD</b></i>(2) drop down you can now switch between states.</li>
  <li>In case you want to switch states in deconstructed state without using the UI, simply look for the <b>LOD Vis</b> attribute created on the root guide.</li>
  <li>For the constructed state- the default attribute host will be the world control. In case you want to change the host in constructed state, simply open the UI again, and input the host into the <b><i>LOD Attribute Host</i></b>(3) box. Once you re-construct, the LOD Vis attribute will be created on your selected host.</li>
</ol>
You can edit/change this data at any time.
<br>

####Legend
<figure>
  <img src="../userGuidesImages/LODsTool/LODsToolLegend.png"/>
  <figcaption>LODs Tool- UI</figcaption>
</figure>

<ol>
  <li>
    <b><i>Rig</b></i>- Selected Rig indication.
  </li>
  <li>
    <b><i>Current LOD</b></i>- Switch between existing LODs using the UI.
  </li>
  <li>
    <b><i>LODs Attribute Host</b></i>- Input the constructed state attribute host for the LOD switch.
  </li>
  <li>
    <b><i>LOD Naming Style</b></i>- Select your prefered naming style. Alphabetical will result in lodA, lodB, lodC... style naming. Numeric will result in lod1, lod2, lod3... naming style.
  </li>
  <li>
    <b><i>LODs Defenition</b></i>- This is where the LOD groups data is displayed and editted. Edit your LOD groups using the righ-click menu (8-11).
  </li>
  <li>
    <b><i>Add LOD</b></i>- Add LOD group, increasing the amount of LOD groups.
  </li>
  <li>
    <b><i>Delete Last LOD</b></i>- Remove the last LOD group, decreasing the amount of LOD groups.
  </li>
  <li>
    <b><i>Set Selected Items</b></i>- For the selected LOD group (column), set the selected scene nodes as the group's content. This will replace any existing members of the group.
  </li>
  <li>
    <b><i>Add Selected Items</b></i>- For the selected LOD group (column), add the selected scene nodes as the group's content. Existing members of the group will be kept.
  </li>
  <li>
    <b><i>Remove Selected Items</b></i>- For the selected LOD group (column), remove any UI selected members from the group.
  </li>
  <li>
    <b><i>Clear ALL</b></i>- Clear ALL Data. All LOD groups and members will be removed.
  </li>
  <li>
    <b><i>Apply Changes</b></i>- Once you are happy with your data, apply (write) it into the rig.
  </li>
</ol>

