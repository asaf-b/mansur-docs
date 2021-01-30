<body>
#meta Settings
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
Author: Asaf Ben-Zur <br>
Best used for: Metacarpal (Fingers), Metatarsal (Toes) <br>
This module will create a control for every root guide position, as well as a few global splay controls for the collection of controls based on settings. <br>
The play controls will behave as a global tweaker for the control collection, allowing easier animation. <br>
In order to implement "splayB" feature, simply parent a FK chain modules under each of the main meta guides. <br>
This module construction will try to detect a FK module under each guide, and if any exist, will create the second layer splay control for these FK chains. <br>
</i>
<br>
</font>
<hr width = 100%>
##Attributes
</table></font>
###GlobalSettings
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>tweakersControlShape</td>
<td>cone</td>
<td>Meta main controls shape</td></tr>
<tr><td>tweakerChannelControl</td>
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
<td>Meta control channel-box settings</td></tr>
</table></font>
###SplaySettings
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>doSplayA</td>
<td>True</td>
<td>Choose if you want to create Splay A control</td></tr>
<tr><td>doSplayAMid</td>
<td>True</td>
<td>Choose if you want to create Splay A Mid control</td></tr>
<tr><td>doSplayB</td>
<td>True</td>
<td>Choose if you want to create Splay B control</td></tr>
<tr><td>doSplayBMid</td>
<td>True</td>
<td>Choose if you want to create Splay B Mid control</td></tr>
<tr><td>splayControlShape</td>
<td>diamond</td>
<td>splay controls shape</td></tr>
<tr><td>splayChannelControl</td>
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
<td style="padding:6px"></td>
</tr>
<tr><td style="padding:6px"><b>Y</b></td>
<td style="padding:6px">v</td>
<td style="padding:6px">v</td>
<td style="padding:6px"></td>
</tr>
<tr><td style="padding:6px"><b>Z</b></td>
<td style="padding:6px">v</td>
<td style="padding:6px">v</td>
<td style="padding:6px"></td>
</tr>
</table>
</font>
</td>
<td>Splay control channel-box settings</td></tr>
</table></font>
