<body>
#lookAtControl Settings
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
Author: Asaf Ben-Zur <br>
Best used for: Eyes, Generic Orientation based components <br>
This module was written to function as an eye IK (look at setup), but can be used for many other generic components. <br>
This module will create a slave control (at root position) which is aim-constraint to custom look-at guide. <br>
The slave control will be the control authority for the joint, as the look-at control will control its orientation. <br>
</i>
<br>
</font>
<hr width = 100%>
##Attributes
</table></font>
###GlobalSettings
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>slaveControlShape</td>
<td>lightSphere</td>
<td>Origin slave control shape</td></tr>
<tr><td>targetControlShape</td>
<td>circle</td>
<td>Main control shape</td></tr>
<tr><td>upLocalDirection</td>
<td>0</td>
<td>Main control shape</td></tr>
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
<td>Main control channel-box settings</td></tr>
</table></font>
###InterpolatedOrientation
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>doInterpOrient</td>
<td>False</td>
<td>This feature is used to create a weighten split orientation. When you need to create a weighted orientation for a control between two spaces, use this feature</td></tr>
<tr><td>spaceA</td>
<td></td>
<td>The first space to be interpolated. This can be a guide, joint, or control.</td></tr>
<tr><td>spaceB</td>
<td></td>
<td>The second space to be interpolated. This can be a guide, joint, or control.</td></tr>
<tr><td>spaceAWeight</td>
<td>0.5</td>
<td>The deafult weight for the first space. The second space weight will be the complimentary weight adding to 1</td></tr>
<tr><td>doAngleBasedScale</td>
<td>False</td>
<td>create an angle based scale driver, to scale the target slave joint when the angle changes between the two sources. Originally designed for double-chin setup</td></tr>
<tr><td>scaleWhenAngle</td>
<td>0</td>
<td>This setting controls the trigger mode for action. Icreases- means that the trigger for action will occur when the intorpolated angle increases, and do nothing when it decreases. decreases- means that the trigger for action will occur when the intorpolated angle decreases, and do nothing when it increases</td></tr>
<tr><td>maxScale</td>
<td>2.0</td>
<td>The actions maximum value clamp value</td></tr>
<tr><td>angleMaxRange</td>
<td>180.0</td>
<td>The maximum angle clamp that the action should be targeted to</td></tr>
<tr><td>connectToTargetAxis</td>
<td>1</td>
<td>This setting will set the target axis to act on. Please map the axis needed to be scaled based on the orientation of your guide</td></tr>
</table></font>
###spring
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>doLookAtSpring</td>
<td>False</td>
<td>This feature will create a spring node blowe the look-at master. This will result in a rotation-based spring, mostly used for vehicle center suspension to achive secondary motion</td></tr>
<tr><td>defaultStiffness</td>
<td>0.5</td>
<td>Spring default stiffness value</td></tr>
<tr><td>defaultDamping</td>
<td>0.5</td>
<td>Spring default damping value</td></tr>
</table></font>
###asEyeLook
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>pupilDilateAttribute</td>
<td></td>
<td>Input bland-shape attribute to connect pupil dialation control to</td></tr>
<tr><td>pupilContractAttribute</td>
<td></td>
<td>Input bland-shape attribute to connect pupil contaction control to</td></tr>
<tr><td>irisDilateAttribute</td>
<td></td>
<td>Input bland-shape attribute to connect iris dialation control to</td></tr>
<tr><td>irisContractAttribute</td>
<td></td>
<td>Input bland-shape attribute to connect iris contaction control to</td></tr>
<tr><td>combinedAttributeHost</td>
<td></td>
<td>If this is set to True, a global attribute for the above pupil and iris controls will be created on the specified attribute host. This feature is mainly to combine two different eye shapes controls into one single control, or moving the location of this attribute to a diffent module in case the eye meshs are combined</td></tr>
</table></font>
