<body>
#simpleSquash Settings
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
Author: Asaf Ben-Zur <br>
Best used for: Head Squash, Nose, any general squash behaviour <br>
This module will create a squash behaviour to it's slave joint. <br>
Any child modules under this module will inherit the squash behaviour. <br>
The squash behaviour can be set by the module's settings, and can also be adjusted and keyed post construction.  <br>
</i>
<br>
</font>
<hr width = 100%>
##Attributes
</table></font>
###GlobalSettings
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>controlShape</td>
<td>arrow</td>
<td>Main control shape</td></tr>
<tr><td>upLocalDirection</td>
<td>0</td>
<td>Use this setting to choose which up-axis should the module use on calculation. This is based on the orientation of your guide. Choose the correct complimentary axis based on set aim guide</td></tr>
</table></font>
###Squash
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>squashFactor</td>
<td>0.5</td>
<td>Squash Factor default value</td></tr>
<tr><td>squashMin</td>
<td>0.8</td>
<td>Squash Minimum scale value</td></tr>
<tr><td>squashMax</td>
<td>1.2</td>
<td>Squash Maximum scale value</td></tr>
</table></font>
###Stretch
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>stretchFactor</td>
<td>0.5</td>
<td>Stretch Factor default value</td></tr>
<tr><td>stretchMin</td>
<td>0.8</td>
<td>Stretch Minimum scale value</td></tr>
<tr><td>stretchMax</td>
<td>1.2</td>
<td>Stretch Maximum scale value</td></tr>
</table></font>
###ChanControl
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
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
<td style="padding:6px"></td>
<td style="padding:6px"></td>
</tr>
<tr><td style="padding:6px"><b>Y</b></td>
<td style="padding:6px">v</td>
<td style="padding:6px"></td>
<td style="padding:6px"></td>
</tr>
<tr><td style="padding:6px"><b>Z</b></td>
<td style="padding:6px">v</td>
<td style="padding:6px"></td>
<td style="padding:6px"></td>
</tr>
</table>
</font>
</td>
<td>Squash control channel-box settings</td></tr>
</table></font>
###SlaveControl
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>slaveControlShape</td>
<td>lightSphere</td>
<td>Slave control shape</td></tr>
<tr><td>slaveChannelControl</td>
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
<td>Squash slave control channel-box settings</td></tr>
</table></font>
