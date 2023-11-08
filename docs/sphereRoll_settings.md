<body>
#sphereRoll Settings
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
Author: Asaf Ben-Zur <br>
Best used for: Balls, BB-8-Style <br>
A simple module to drive a sphere roll based on position. <br>
Upon contruction, based on the given settings, the main joint orientation will be driven by the module's position. <br>
This module will calculate the roll of the sphere needed to reach the target position, without slipping, in any direction. <br>
This behaviour is not confined to a single control being moved, but rather calculated based on the module's world-position. <br>
</i>
<br>
</font>
<hr width = 100%>
##Attributes
<tr><td>splitOrientSpace</td>
<td>True</td>
<td>Comment wasn't inserted</td></tr>
</table></font>
###GlobalSettings
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>controlShape</td>
<td>lightSphere</td>
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
<tr><td>sphereRadius</td>
<td>20.0</td>
<td>The controled sphere radius. This is the source of the calculation and needs to be set accurately</td></tr>
<tr><td>autoRollDefault</td>
<td>1.0</td>
<td>Auto-Roll channel default state</td></tr>
</table></font>
