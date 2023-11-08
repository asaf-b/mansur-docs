<body>
#wheel Settings
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
Author: Asaf Ben-Zur <br>
Best used for: Wheels <br>
A simple module to create an auto-drive for wheels. <br>
This module will calculate the rotation of a wheel based on the input settings, using the module's world position. <br>
This will yield an auto-drive for wheels. <br>
The behaviour will not be confined to a single control being moved, but rather to the modules world position. <br>
This will apply to translation, as well as rotation, in all directions. <br>
</i>
<br>
</font>
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
<tr><td>wheelDiameter</td>
<td>20.0</td>
<td>The driven wheel diameter. This is the base of the calculation and needs to be set accurately</td></tr>
<tr><td>gearRatio</td>
<td>1.0</td>
<td>In case you target is a driven gear, you can set the diameter above to the driver gears diameter, and set the ratio between them for accurate results</td></tr>
<tr><td>mapRoatationToAxis</td>
<td>0</td>
<td>Map the rotation axis needs to be acted on. This is based on the orientaton of your guide</td></tr>
<tr><td>reverseDirection</td>
<td>False</td>
<td>In some cases the direction of the drive is flipped. If this is your case, set this setting to True to correct this issue</td></tr>
<tr><td>autoDriveDefault</td>
<td>1.0</td>
<td>Auto-Drive channel default state</td></tr>
</table></font>
