<body>
#hindLimb Settings
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
Author: Asaf Ben-Zur <br>
Best used for: Arms, Legs <br>
This module was designed to create a generic 3 joint limb control. <br>
This module will create both the FK and IK controls, and the standard blend control. <br>
On top of the standard behaviour, based on parameters, this module can also include bendy limb controls (as many as you want), Arc layer and Sleeve layer. <br>
Note: When used as a leg, try using the foot module as a direct child of this module to automatically achive a connected behaviour. <br>
</i>
<br>
</font>
<hr width = 100%>
##Attributes
</table></font>
###GlobalSettings
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>interpolationJoints</td>
<td>4</td>
<td>Increments of 3, starting from 4. This setting controls the number of driven interpolation joints needed. This interpolation joint chain will behave according to the module's design, and will inherit transformations that are required by this module. Usually the driven interpolation joint-chain is the compenents result behaviour in animation.</td></tr>
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
<td>0</td>
<td>Default squash mode. Please refer to the documentation of mnsPointsOnCurve node to learn more about each mode</td></tr>
<tr><td>ikFkBlendDefault</td>
<td>0.0</td>
<td>Default value for the main IK-FK blend channel. 0 is IK, 1 is FK.</td></tr>
</table></font>
###IK
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>stretchLimit</td>
<td>1.0</td>
<td>IK Handle stratch limit default value</td></tr>
<tr><td>iKHandleMatchOrient</td>
<td></td>
<td>Select a guide to match the IK-Handle's orientation. This will override the native orientation as well as all symmetry options.</td></tr>
</table></font>
###Main-Ctrl-Shapes
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>rootControlShape</td>
<td>lightSphere</td>
<td>Module root control control shape</td></tr>
<tr><td>ikHandleControlShape</td>
<td>square</td>
<td>IK Handle control shape</td></tr>
<tr><td>poleVectorControlShape</td>
<td>diamond</td>
<td>Pole Vector control shape</td></tr>
<tr><td>ankleBendControlShape</td>
<td>squareRound</td>
<td>IK Ankle Bend control shape</td></tr>
<tr><td>fkControlShape</td>
<td>hexagon</td>
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
