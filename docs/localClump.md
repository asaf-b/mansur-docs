<body>
#localClump
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
In case you want to mimic a normal parenting behaviour, use the conformPivot attribute, which will conform all local driven controls to the pivot of this master clump control. <br>
Leaving conformPivot OFF, will simply connect to the local channels of the slave, leaving its pivots intact. This will result in a slightly different behaviour. <br>
You can also use connectToChannelControl attribute to decide which attributes you want to connect to, and the ones you want to leave out. <br>
 <br>
</font>
</i>
<hr width = 100%>
##Defenitions
<hr width = 100%>
###construct
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>construct(mansur, MnsBuildModule, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td> list (controls), dict (internalSpaces)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>mansur</b></li>
<li><b>MnsBuildModule</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###filterValidClumpSlaves
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>filterValidClumpSlaves(slavesList = [], mansur = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>slavesList</b>(<i>list</i>) ; [default: []]</li>
<li><b>mansur</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###jointStructure
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>jointStructure(mansur, guides, mnsBuildModule = None, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>mansur</b></li>
<li><b>guides</b></li>
<li><b>mnsBuildModule</b>(<i>str</i>) ; [default: None]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###postConstruct
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>postConstruct(mansur, MnsBuildModule, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>mansur</b></li>
<li><b>MnsBuildModule</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
