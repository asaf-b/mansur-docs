<body>
#limb Settings
<hr width = 100%>
##Attributes
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr>
<td>offsetX</td>
<td>20.0</td>
<td>Up curve X value offset for the interpolation joints</td>
</tr></td>
<tr>
<td>offsetZ</td>
<td>0.0</td>
<td>Up curve Z value offset for the interpolation joints</td>
</tr></td>
<tr>
<td>FKSymmetryType</td>
<td>0</td>
<td>FK controls symmetry type, in case it needs to differ from the main symmetry type</td>
</tr></td>
<tr>
<td>scaleMode</td>
<td>2</td>
<td>Default scale mode. Please refer to the documentation of mnsPointsOnCurve node to learn more about each mode</td>
</tr></td>
<tr>
<td>squashMode</td>
<td>0</td>
<td>Default squash mode. Please refer to the documentation of mnsPointsOnCurve node to learn more about each mode</td>
</tr></td>
<tr>
<td>stretchLimit</td>
<td>1.0</td>
<td>IK Handle stratch limit default value</td>
</tr></td>
<tr>
<td>softness</td>
<td>0.0</td>
<td>IK handle softness default value</td>
</tr></td>
<tr>
<td>rootControlShape</td>
<td>lightSphere</td>
<td>Module root control control shape</td>
</tr></td>
<tr>
<td>ikHandleControlShape</td>
<td>square</td>
<td>IK Handle control shape</td>
</tr></td>
<tr>
<td>poleVectorControlShape</td>
<td>diamond</td>
<td>Pole Vector control shape</td>
</tr></td>
<tr>
<td>fkControlShape</td>
<td>hexagon</td>
<td>FK controls shape</td>
</tr></td>
<tr>
<td>tertiariesControlShape</td>
<td>flatDiamond</td>
<td>Tweak tertiary controls shape</td>
</tr></td>
<tr>
<td>doTweakers</td>
<td>False</td>
<td>This feature will create a secondary tweak layer below the main control chain. This is commonly known as Bendy-Limbs</td>
</tr></td>
<tr>
<td>tweakersSymmetryType</td>
<td>3</td>
<td>Tweak controls symmetry type, in case it needs to differ from the main symmetry type</td>
</tr></td>
<tr>
<td>tweakersPerSection</td>
<td>1</td>
<td>The amount of bendy controls per section. A value of one will create two controls in total - one for the upper section of the limb, on for the lower section</td>
</tr></td>
<tr>
<td>createExtraAttributes</td>
<td>True</td>
<td>If this is set to True, some extra tertiary channel-box control attributes will be added to the attribute-host</td>
</tr></td>
<tr>
<td>tweakControlShape</td>
<td>dialSquare</td>
<td>Tweak controls shape</td>
</tr></td>
<tr>
<td>negateOffsetOnSymmetry</td>
<td>False</td>
<td>If this is set to True, the above offsetX and offsetZ value for the up curve will be negated</td>
</tr></td>
<tr>
<td>tweakersChannelControl</td>
<td>{'s': (True, True, True), 'r': (True, True, True), 't': (True, True, True)}</td>
<td>Tweak controls channel-box settings</td>
</tr></td>
<tr>
<td>doArc</td>
<td>False</td>
<td>This feature will use mnsThreePointArc node to create an automatic arc layer on the final curve output</td>
</tr></td>
<tr>
<td>arcDegree</td>
<td>3</td>
<td>Arc's curve degree. Refer to mnsThreePointArc node documentation to learn more about this attribute</td>
</tr></td>
<tr>
<td>arcSections</td>
<td>8</td>
<td>The amount of samples used to create the arc. Since three samples will create no effect (the result arc needs more points in between to describe the shape), use a higher value to create an effect. The higher the sample amount, the more precise the arc will be</td>
</tr></td>
<tr>
<td>resampleCurveSections</td>
<td>16</td>
<td>Post creation sample amount</td>
</tr></td>
<tr>
<td>collinearAction</td>
<td>0</td>
<td>this attribute will be used to dictate what to do when the limb is straight (the collinear case). Input curve will match the input curve plugged into this node (recommended), re-sample will create a new curve based on the node's attributes</td>
</tr></td>
<tr>
<td>conformToMidPoint</td>
<td>True</td>
<td>If this is set to True, the node will attempt to pin the middle origin sample in its place, resulting in a much stabler result. If this is set to False, the middle origin sample might shift while animating the arc value (not recommended)</td>
</tr></td>
<tr>
<td>addSwipes</td>
<td>True</td>
<td>Add swipe channel-channel box attributes to the attribute host</td>
</tr></td>
<tr>
<td>doSleeve</td>
<td>False</td>
<td>Do sleeve feature. This feature will create a curbe and controls along the result interpolation joints of this module. This will result in the ability to control a sleeve position along the limb as well as many other features</td>
</tr></td>
<tr>
<td>numSleeveJoints</td>
<td>3</td>
<td>The amount of joints to sample along the sleeve curve</td>
</tr></td>
<tr>
<td>sleeveControlShape</td>
<td>octagon</td>
<td>Sleeve control shape</td>
</tr></td>
<tr>
<td>sleeveCurveDegree</td>
<td>3</td>
<td>Sleeve curve degree</td>
</tr></td>
<tr>
<td>sleeveBuildMode</td>
<td>0</td>
<td>Sleeve curve generation mode</td>
</tr></td>
</table></font>
