<body>
#curveAttachment Settings
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
Author: Asaf Ben-Zur <br>
Best used for: Sliding doors, curtains <br>
This is a simple module that allows a control attachment to a given curve. <br>
The attachment can also be created with an offset to current position, as well as some attachment modes and up modes. <br>
Use this module in case you need to attach a control or joint to a curve <br>
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
<td>arrow</td>
<td>Control shape</td></tr>
<tr><td>attachmentCurve</td>
<td></td>
<td>Curve to attach to.</td></tr>
<tr><td>attachmentUpCurve</td>
<td></td>
<td>Up curve to use. This curve will be used to determine the up vector of the created ctrl. In case this isn't used, global module orient will be used.</td></tr>
<tr><td>objectOrientUpAxis</td>
<td>0</td>
<td>In case no up curve is used, this global module rotation axis will be used</td></tr>
<tr><td>attachmentMode</td>
<td>0</td>
<td>Curve sampling mode. Please refer to the documentation of mnsPointsOnCurve node to learn more about curve each mode</td></tr>
<tr><td>maintainOffset</td>
<td>True</td>
<td>Whether to maintain control to curve offset of construction. In case this is True, the guide position will be maintained. In case this is False, the ctrl will be created at U0 position of the input attachment curve.</td></tr>
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
</table></font>
