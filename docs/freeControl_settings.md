<body>
#freeControl Settings
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
Author: Asaf Ben-Zur <br>
Best used for: Free objects, General Control, Mesh Tweaker, Mesh Local Tweaker <br>
This Module is a general single control at it's base state. <br>
It also contains a Mesh-Tweaker feature that will allow you to create a "Double Directional" tweaker- meaning that the control will follow the input Mesh's position (Rivet) and will also be able to affect it. <br>
This effect is also commonly knowen as the "Dorito-Effect". <br>
This feature also includes a "local" mode, to tunnel deformations from the control to a local skinCluster, then a blend-shape to the main Mesh, creating multi-layered skinned mesh. <br>
All of these features will use the main joint as the effector. <br>
Note: When using the "Mesh-Tweaker" feture, when needing to affect a mesh that will also be used as the rivet input- make sure "sameMeshAffector" is set to ON. <br>
</i>
<br>
</font>
<hr width = 100%>
##Attributes
<tr><td>symmetryType</td>
<td>0</td>
<td>Choose the mirror type for right side controls</td></tr>
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
<tr><td>positionMode</td>
<td>0</td>
<td>this will determine the output rivet position mode.</td></tr>
<tr><td>doRotation</td>
<td>False</td>
<td>when off, the rivet will not inherit rotations from the mesh</td></tr>
<tr><td>sameMeshAffector</td>
<td>True</td>
<td>If this is set to False, you will NOT be able to use this control's related joint within the deformation of the above mesh (this will result as a cycle). In case you want the control to follow the mesh as well as have it's related joint within the deformation of the mesh- please leave this ON. In case you want to attach this control to a mesh that will not be affected by the control's related joint, you can safely turn this attribute OFF.</td></tr>
<tr><td>isLocal</td>
<td>False</td>
<td>In some cases, you may wish to use this control's related joint in a different skinCluster layer, channeled into the main mesh as a blendShape. If that is the case, you will need to set this attribute to ON. When set to ON, the related joint will be a part of the joint hierarchy, but will keep it's position at origin so you can you it in a local setup. In case the riveted mesh's deformation is affected by this module's related joint in any way, remember to keep sameMeshEffector ON, even if its not a part of the main skinCluster. This means that even if the joint is controlling a localized skin-cluter, and then channeled as a blend shape into the riveted mesh, sameMeshAffector should be left ON.</td></tr>
</table></font>
###spring
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>doSpring</td>
<td>False</td>
<td>This feature will create a spring node below the control master. This will result in a procedural simple spring action. In case meshTweaker feature was selected, the slave control will not be visible. This feature will NOT be created in case isLocal is set to ON.</td></tr>
<tr><td>springX</td>
<td>True</td>
<td>Comment wasn't inserted</td></tr>
<tr><td>springY</td>
<td>True</td>
<td>Comment wasn't inserted</td></tr>
<tr><td>springZ</td>
<td>True</td>
<td>Comment wasn't inserted</td></tr>
<tr><td>defaultStiffness</td>
<td>0.5</td>
<td>Comment wasn't inserted</td></tr>
<tr><td>defaultDamping</td>
<td>0.5</td>
<td>Comment wasn't inserted</td></tr>
<tr><td>springSlaveControlShape</td>
<td>lightSphere</td>
<td>Spring slave control shape</td></tr>
</table></font>
###InterpolatedOrientation
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>doInterpOrient</td>
<td>False</td>
<td>Comment wasn't inserted</td></tr>
<tr><td>spaceA</td>
<td></td>
<td>Comment wasn't inserted</td></tr>
<tr><td>spaceB</td>
<td></td>
<td>Comment wasn't inserted</td></tr>
<tr><td>spaceAWeight</td>
<td>0.5</td>
<td>Comment wasn't inserted</td></tr>
<tr><td>doAngleBasedScale</td>
<td>False</td>
<td>create an angle based scale driver, to scale the target slave joint when the angle changes between the two sources. Originally designed for double-chin setup</td></tr>
<tr><td>scaleWhenAngle</td>
<td>0</td>
<td>Comment wasn't inserted</td></tr>
<tr><td>maxScale</td>
<td>2.0</td>
<td>Comment wasn't inserted</td></tr>
<tr><td>angleMaxRange</td>
<td>180.0</td>
<td>Comment wasn't inserted</td></tr>
<tr><td>connectToTargetAxis</td>
<td>1</td>
<td>Comment wasn't inserted</td></tr>
</table></font>
