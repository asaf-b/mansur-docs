<body>
#localClump Settings
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
Author: Asaf Ben-Zur <br>
Best used for: Clumps of controls. i.e. the first layer of controls in a clump of 5 hair strands (FK chains). <br>
This module was developed to allow a local control driver, over clumps of controls. <br>
For example, a block rig contains 10 hair strands, controled by 10 FK-Shain modules, with 3 controls each. <br>
In some cases it is easier to pose the hair treting it as a single unit instead of indevidual strands. <br>
So, a clump-control can be created for each layer of controls (3, 1 for every unit in each chain). <br>
The control will be created using local channels in order to not break the FK behaviour of the strands. <br>
In case any other method was used (spaces, module parenting), each indevidual strand FK behaviour would have been broken. <br>
The clump controls can also be parented under one another to create a layered-FK behaviour. <br>
This will result in a main clump-fk chain, treating the hair as a single unit, and FK chains below to tread each strand indevidually. <br>
 <br>
In case you want to mimic a normal parenting behaviour, use the conformPivot attribute, which will conform all local driven controls to the pivot of this master clump control. <br>
Leaving conformPivot OFF, will simply connect to the local channels of the slave, leaving its pivots intact. This will result in a slightly different behaviour. <br>
You can also use connectToChannelControl attribute to decide which attributes you want to connect to, and the ones you want to leave out. <br>
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
<tr><td>clumpSlaves</td>
<td>[' ']</td>
<td>All guides that will be locally controlled by this clump</td></tr>
<tr><td>connectToChannelControl</td>
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
<td>This will determine which channels or axes will be connected to the slaves.</td></tr>
<tr><td>conformPivot</td>
<td>True</td>
<td>When ON, the pivot of the target slaves will be conformed to the pivot of this master control. When OFF, the original pivots of the slaves will be preserved.</td></tr>
<tr><td>createJoint</td>
<td>False</td>
<td>Choose whether to create and attach a joint to this control</td></tr>
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
