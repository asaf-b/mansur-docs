<body>
#linkChain Settings
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
Author: Asaf Ben-Zur <br>
Best used for: Tank-Treads, Bike-Chains, Ferris-Wheel, Tire, Conveyor-Belt <br>
This is a comprehensive module, to create a link-chain style behaviour. <br>
Originally created for tank-treads, but can be used for a range of components. <br>
On creation, based on the number on the numberOfLinks setting, joints will be created on a circle Nurbs curve with shapeSections setting amount. <br>
After creation, the shape can be tweaked to fit any need.  <br>
IMPORTANT NOTE: This module requires a joint-struct-rebuild once the Nurbs shape has been tweaked. <br>
Once the joint-struct is revuilt, the joints will be layed out uniformally along the given shape. <br>
Upon construction, a main control will be created for controlling the entire position of the module. <br>
Under, a chain-driver control will be created. Rotating it will drive the joint chain along the curve in both forwards and backwards directions. <br>
Also, use the shape-tweak layer to create a tweak feature for the shape on construction. This will allow manipulation of the shape dynamically while the chain is driven. <br>
Automatic drive based on position is also possible wihin this module using the AutoDrive layer. <br>
</i>
<br>
</font>
<hr width = 100%>
##Attributes
<tr><td>splitOrientSpace</td>
<td>True</td>
<td>If this is set to True, all space switch attributes for this module will split into two spaces- Translate and Orient, for the animator to be able to set different space for tranlation and orientation</td></tr>
</table></font>
###GlobalSettings
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>numberOfLinks</td>
<td>16</td>
<td>Amount of links in the chain. A joint will be created for every link</td></tr>
<tr><td>reverseOffsetDirection</td>
<td>False</td>
<td>In case the the rotation post construction is reversed, set this attribute to ON</td></tr>
<tr><td>upCurveOffset</td>
<td>5.0</td>
<td>The offset value to generate the up curve, based on a center matrix- the modules root joint</td></tr>
<tr><td>controlShape</td>
<td>circle</td>
<td>Control shape</td></tr>
<tr><td>slaveControlShape</td>
<td>dodecagon</td>
<td>Slave control shape</td></tr>
<tr><td>wheelDiameter</td>
<td>20.0</td>
<td>The diameter of your wheel. This is very important to set correctly as the diameter of the wheel is one of the source attributes for the wheels rotation calculation</td></tr>
<tr><td>mapRoatationToAxis</td>
<td>0</td>
<td>Map the rotation action you need to be acted on. This is based on the orientation of your guide</td></tr>
<tr><td>rotationMode</td>
<td>0</td>
<td>In case your chain links are connected to one another- it is recommended to use lookAtNext. In case there isn't a connection between your links, curveTangent might be a better choice</td></tr>
<tr><td>slaveChannelControl</td>
<td>
<font size = 2pt>
<table><tr><td style="padding:6px"></td>
<td style="padding:6px"><b>T</b></td>
<td style="padding:6px"><b>R</b></td>
<td style="padding:6px"><b>S</b></td>
</tr>
<tr><td style="padding:6px"><b>X</b></td>
<td style="padding:6px"></td>
<td style="padding:6px">v</td>
<td style="padding:6px"></td>
</tr>
<tr><td style="padding:6px"><b>Y</b></td>
<td style="padding:6px"></td>
<td style="padding:6px">v</td>
<td style="padding:6px"></td>
</tr>
<tr><td style="padding:6px"><b>Z</b></td>
<td style="padding:6px"></td>
<td style="padding:6px">v</td>
<td style="padding:6px"></td>
</tr>
</table>
</font>
</td>
<td>Slave control channel-box settings</td></tr>
</table></font>
###ShapeTweak
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>doShapeTweakers</td>
<td>False</td>
<td>If this setting in set to True, the shape-tweak feature will be created. In case you want to tweak the shape of the closed-shaped link chain curve in animation, turn this feature on</td></tr>
<tr><td>shapeTweakers</td>
<td>[' ']</td>
<td>Input guides/joints- In order. A closed nurbs-curve shape will be constructed from the inputs and will be used as a tweak to deform the main shape driving the chain. These MUST be Mansur-Rig objects, and a part of the same Block rig.</td></tr>
<tr><td>tweakMethod</td>
<td>1</td>
<td>This attribute will determine the shape tweak method. In Direct-Skin mode, the link chain shape will be directly skinned to all input tweakers. In Build-Transforms-Curve mode a new curve will be constructed based on the curve mode selected and input tweakers, which will be used to deform the master shape indirectly. This mode will allow for a better control over the deformation, as it is based on curve re-generation instead of direct curve deformation. Build transforms curve mode will generate a new closed shape curve based on the input tweak transforms, hence it is order sensative. In case you wish to use this mode, make sure you input the tweakers in order which makes sense to generate a closed curve shape. Rebuild-Then-Skin mode will first rebuild the curve based on the input re-build number of spans attribute, then skin the curve and deform the master curve indirectly</td></tr>
<tr><td>rebuildNumOfSpans</td>
<td>16</td>
<td>relevant only on rebuildThenSkin tweak method. This attribute dectates the amount of sections to rebuild the curve to before skinning</td></tr>
<tr><td>tweakCurveInterpolaion</td>
<td>1</td>
<td>relevant only on mnsBuildTransformsCurve tweak method</td></tr>
<tr><td>tweakCurveDegree</td>
<td>3</td>
<td>relevant only on mnsBuildTransformsCurve, and rebuild then skin tweak methods</td></tr>
</table></font>
###AutoDrive
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>doAutoDrive</td>
<td>False</td>
<td>This feature will create an auto-drive mechanism, that will automatically drive the chain when it moves in space</td></tr>
<tr><td>autoDriveWheelDiameter</td>
<td>20.0</td>
<td>The diameter of the driver wheel, whether it exists or not. This diameter is derived from the main gear driving this link-chain. This diameter will be used to calculate the drive of the chain</td></tr>
<tr><td>gearRatio</td>
<td>1.0</td>
<td>In case your main driver is derived from another gear, you can set its ratio here to get accurate results</td></tr>
<tr><td>reverseDirection</td>
<td>False</td>
<td>In some cases the direction of the drive is flipped. If this is your case, set this setting to True to correct this issue</td></tr>
<tr><td>autoDriveDefault</td>
<td>1.0</td>
<td>Auto-Drive channel default state</td></tr>
</table></font>
