<body>
#foot Settings
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
Author: Asaf Ben-Zur <br>
Best used for: Foot <br>
This Module was created for a foot setup mainly. <br>
Some of it's main features are FK controls, BK (backward kinematics) controls, Roll control, Bank Controls, Heel and Tip controls, Dynamic pivot control. <br>
The best application for this module is placing it under a limb module, which will result in a connected (standard) behaviour. <br>
</i>
<br>
</font>
<hr width = 100%>
##Attributes
</table></font>
###ToesFK
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>FKControlShape</td>
<td>cube</td>
<td>Toes FK controls shape</td></tr>
<tr><td>FKChannelControl</td>
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
<td>Toes FK controls channel-box settings</td></tr>
</table></font>
###ToesBK
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>BKControlShape</td>
<td>diamond</td>
<td>BK (Backward Kinematics) controls shape</td></tr>
<tr><td>BKChannelControl</td>
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
<td>BK controls channel-box settings</td></tr>
</table></font>
###BankControls
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>bankControlShape</td>
<td>lightSphere</td>
<td>Bank controls shape</td></tr>
<tr><td>bankChannelControl</td>
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
<td>bank controls channel-box settings</td></tr>
</table></font>
###RollControl
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>doRollCtrl</td>
<td>True</td>
<td>If this is True, a foot Roll control will be created</td></tr>
<tr><td>rollControlShape</td>
<td>cylinder</td>
<td>Roll control channel-box settings</td></tr>
<tr><td>rollDefaultMaxAngle</td>
<td>60.0</td>
<td>Default Roll maximum limit angle. The roll control is used to roll the entire foot chain, and using an angle value to limit the roll of each section, before rolling the next section. This value will be used as default</td></tr>
<tr><td>straightenDefaultAngle</td>
<td>130.0</td>
<td>Default straighten angle. The foot toes will straighten between the max angle above and this angle. As the angle passes the above angle, along the range up to this angle, the rool angle will decrease- strightening the foot on the up position.</td></tr>
</table></font>
###DynamicPivotControl
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>doDynamicPivCtrl</td>
<td>True</td>
<td>This feature will create a control that will try to trace the desired foot shape with it's pivot when rotating it. When choosing to create this control, use the relevant guide's shape to trace the outline of your foot</td></tr>
<tr><td>dynamicPivControlShape</td>
<td>lightSphere</td>
<td>Dynamic roll control shape</td></tr>
<tr><td>mapRotXTo</td>
<td>2</td>
<td>as this feature uses local channels, it is essential to map input values correctly. Please map the correct axes based on the orientation of your guide</td></tr>
<tr><td>mapRotYTo</td>
<td>3</td>
<td>as this feature uses local channels, it is essential to map input values correctly. Please map the correct axes based on the orientation of your guide</td></tr>
<tr><td>mapRotZTo</td>
<td>6</td>
<td>as this feature uses local channels, it is essential to map input values correctly. Please map the correct axes based on the orientation of your guide</td></tr>
<tr><td>distRateMultiplier</td>
<td>5.0</td>
<td>This feature will use the translation of a run-away transform to acquire the best pivot location along the given outline shape. This value will dictate the speed of translation</td></tr>
<tr><td>dynamicPivChannelControl</td>
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
<td style="padding:6px"></td>
<td style="padding:6px"></td>
</tr>
</table>
</font>
</td>
<td>Roll control channel-box settings</td></tr>
</table></font>
