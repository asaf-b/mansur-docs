<body>
#splay Settings
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
Author: Asaf Ben-Zur <br>
Best used for: fingers, bat wings <br>
This is a general module used for splaying behaviour for any slave modules. <br>
This module does not create any joints. <br>
This module's behaviour is matched to the Meta module's splay behaviour, but can be implemented for any slave module. <br>
A control will be created, and it's translation and rotation values will be connected to all input slave guides in the module settings, creating a gradual translation/rotation for all slaves- creating the splay behaviour. <br>
Splay multipliers that can be manipulated will be created as well on the given control. <br>
This module contains the choice of adding another Splay-Mid control, which will be added to the calculation, creating a gradual behaviour from the middle slave outwards in both directions, instead of the top-to-bottom splay that the main control offers. <br>
Make sure to load slaves IN-ORDER to achive correct behaviour. <br>
Valid-Slaves are root-guide and guides only. The slaves will be the direct related controls to these input guides. <br>
Important: The behaviour is a result of a local channel connection. Since the slaves' orientation is unknowen, you need to make sure that this module's orientation matches the target slaves orientation. <br>
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
<td>lightPin</td>
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
<td>Control channel-box settings</td></tr>
<tr><td>createJoint</td>
<td>False</td>
<td>Choose whether to create and attach a joint to this control</td></tr>
<tr><td>slaveModules</td>
<td>[' ']</td>
<td>All guides- IN ORDER - that will be locally controlled by this splay control. Only root guides and guides are valid inputs, all other types will be ignored</td></tr>
</table></font>
###SplayMid
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>doSplayMid</td>
<td>False</td>
<td>Choose whether to create a mid splay control</td></tr>
<tr><td>midControlShape</td>
<td>lightPin</td>
<td>Splay Mid Control shape</td></tr>
<tr><td>midChannelControl</td>
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
<td>Control channel-box settings</td></tr>
</table></font>
