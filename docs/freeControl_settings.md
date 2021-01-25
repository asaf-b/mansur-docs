<body>
#freeControl Settings
<hr width = 100%>
##Attributes
</table></font>
###GlobalSettings
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>controlShape</td>
<td>circle</td>
<td>Control shape</td></tr>
<tr><td>channelControl</td>
<td>
<font size = 2pt>
<table><tr><td style="padding:6px"></td>
<td style="padding:6px"><b>T</b></td>
<td style="padding:6px"><b>R</b></td>
<td style="padding:6px"><b>S</b></td>
</tr>
<tr><td style="padding:6px"><b>X</b></td>
<td style="padding:6px">v</td>
<td style="padding:6px">v</td>
<td style="padding:6px">v</td>
</tr>
<tr><td style="padding:6px"><b>Y</b></td>
<td style="padding:6px">v</td>
<td style="padding:6px">v</td>
<td style="padding:6px">v</td>
</tr>
<tr><td style="padding:6px"><b>Z</b></td>
<td style="padding:6px">v</td>
<td style="padding:6px">v</td>
<td style="padding:6px">v</td>
</tr>
</table>
</font>
</td>
<td>Control channel-box settings</td></tr>
<tr><td>createJoint</td>
<td>True</td>
<td>Choose whether to create and attach a joint to this control</td></tr>
<tr><td>asTweakerDivider</td>
<td>MeshTweaker</td>
<td>Comment wasn't inserted</td></tr>
<tr><td>asMeshTweaker</td>
<td>False</td>
<td>This control can aslo act as a live mesh tweaker. This means that you can attach this control to a mesh, having it follow the deformed mesh. In case you want this control to be affected by the mesh (position of the control) and also affect the mesh (using a skinCluster for example), please make sure that you leave sameMeshEffector attribute ON. You do not need to use any other meshes or joints to implement this behaviour</td></tr>
<tr><td>rivetToMesh</td>
<td></td>
<td>The mesh you want to attach the control to</td></tr>
<tr><td>sameMeshAffector</td>
<td>True</td>
<td>If this is set to False, you will NOT be able to use this control's related joint within the deformation of the above mesh (this will result as a cycle). In case you want the control to follow the mesh as well as have it's related joint within the deformation of the mesh- please leave this ON. In case you want to attach this control to a mesh that will not be affected by the control's related joint, you can safely turn this attribute OFF</td></tr>
<tr><td>isLocal</td>
<td>False</td>
<td>In some cases, you may wish to use this control's related joint in a different skinCluster layer, channeled into the main mesh as a blendShape. If that is the case, you will need to set this attribute to ON. When set to ON, the related joint will be a part of the joint hierarchy, but will keep it's position at origin so you can you it in a local setup</td></tr>
</table></font>
