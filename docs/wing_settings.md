<body>
#wing Settings
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
Author: Asaf Ben-Zur <br>
Best used for: Bird Wings <br>
This module is designed for birds (feathered) wings. <br>
This is a compound module. <br>
The main module is based on the limb module, including most of it's features. <br>
On top of the main limb module, there is a compound FK chain modules extending from each of the main modules main guides, to create a global feathers silhouette control. <br>
Out of these compounds, a grid of interp-joints is created to control the shape's deformation, using mnsPointOnCuveNode as a driver. <br>
As a bird wing is incredibly complex, controlling it precisely is incredibly difficult. <br>
With that in mind, the grid of interp joints is designed to control the overall shape of the feathers as a group, mid-controls to curl them as a group, as well as control each feather row individually. <br>
Use featherJoints attribute to define the number of feathers along the wings main skeleton. <br>
Post joint-struct creation, use the custom position adjustment attribute on the root-guide to adjust the position of the joint grid to match your needs. <br>
This module also contains multiple features to make animation even better: <br>
Feathers spring, global wave control, individual feather control, bendy limbs, extension-to-look-at for easy wing fold control. <br>
</i>
<br>
</font>
<hr width = 100%>
##Attributes
</table></font>
###GlobalSettings
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>interpolationJoints</td>
<td>5</td>
<td>Increments of 4, starting from 5. This setting controls the number of driven interpolation joints needed. This interpolation joint chain will behave according to the module's design, and will inherit transformations that are required by this module. Usually the driven interpolation joint-chain is the compenents result behaviour in animation</td></tr>
<tr><td>offsetX</td>
<td>20.0</td>
<td>Up curve X value offset for the interpolation joints</td></tr>
<tr><td>offsetZ</td>
<td>0.0</td>
<td>Up curve Z value offset for the interpolation joints</td></tr>
<tr><td>FKSymmetryType</td>
<td>0</td>
<td>FK controls symmetry type, in case it needs to differ from the main symmetry type</td></tr>
<tr><td>scaleMode</td>
<td>2</td>
<td>Default scale mode. Please refer to the documentation of mnsPointsOnCurve node to learn more about each mode</td></tr>
<tr><td>squashMode</td>
<td>4</td>
<td>Default squash mode. Please refer to the documentation of mnsPointsOnCurve node to learn more about each mode</td></tr>
<tr><td>ikFkBlendDefault</td>
<td>1.0</td>
<td>Default value for the main IK-FK blend channel. 0 is IK, 1 is FK.</td></tr>
</table></font>
###FeathersSettings
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>featherJoints</td>
<td>15</td>
<td>The amount of primary feathers. Ideally, a joint chain will be craeted for each primary feather for the most control in animation. This setting sets the mount of primary feathers, or the amount of feather column chains created</td></tr>
<tr><td>featherFKSections</td>
<td>3</td>
<td>The amount of sections each primary feather joint column will consist of. In case the amount of sections set is 3 for example, a column of 4 joints will be created for the amount of feather joints selected above</td></tr>
<tr><td>doFeathersSpring</td>
<td>True</td>
<td>Choose whether create the automatic feather spring feature or not</td></tr>
<tr><td>doFeatherIsolatedCtrls</td>
<td>True</td>
<td>In case this setting is set to true, the isolated-feather controls feature will be created</td></tr>
<tr><td>featherFKControlShape</td>
<td>cube</td>
<td>Feather FK controls shape</td></tr>
<tr><td>featherIsolatedControlShape</td>
<td>square</td>
<td>Feather isolted controls shape</td></tr>
<tr><td>extensionLookAtControlShape</td>
<td>lightPin</td>
<td>Extensions look-at control shape</td></tr>
</table></font>
###IK
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>stretchLimit</td>
<td>1.0</td>
<td>IK Handle stratch limit default value</td></tr>
<tr><td>softness</td>
<td>0.0</td>
<td>IK handle softness default value</td></tr>
<tr><td>iKHandleMatchOrient</td>
<td></td>
<td>Select a guide to match the IK-Handle's orientation. This will override the native orientation as well as all symmetry options</td></tr>
</table></font>
###Main-Ctrl-Shapes
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>rootControlShape</td>
<td>plus</td>
<td>Module root control control shape</td></tr>
<tr><td>ikHandleControlShape</td>
<td>square</td>
<td>IK Handle control shape</td></tr>
<tr><td>poleVectorControlShape</td>
<td>diamond</td>
<td>Pole Vector control shape</td></tr>
<tr><td>fkControlShape</td>
<td>cylinder</td>
<td>FK controls shape</td></tr>
<tr><td>tertiariesControlShape</td>
<td>flatDiamond</td>
<td>Tweak tertiary controls shape</td></tr>
</table></font>
###tweakers/bendy-Limbs
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>doTweakers</td>
<td>False</td>
<td>This feature will create a secondary tweak layer below the main control chain. This is commonly known as Bendy-Limbs</td></tr>
<tr><td>tweakersSymmetryType</td>
<td>3</td>
<td>Tweak controls symmetry type, in case it needs to differ from the main symmetry type</td></tr>
<tr><td>tweakersPerSection</td>
<td>1</td>
<td>The amount of bendy controls per section. A value of one will create two controls in total - one for the upper section of the limb, on for the lower section</td></tr>
<tr><td>createExtraAttributes</td>
<td>True</td>
<td>If this is set to True, some extra tertiary channel-box control attributes will be added to the attribute-host</td></tr>
<tr><td>tweakControlShape</td>
<td>dialSquare</td>
<td>Tweak controls shape</td></tr>
<tr><td>negateOffsetOnSymmetry</td>
<td>False</td>
<td>If this is set to True, the above offsetX and offsetZ value for the up curve will be negated</td></tr>
<tr><td>tweakersChannelControl</td>
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
<td>Tweak controls channel-box settings</td></tr>
</table></font>
