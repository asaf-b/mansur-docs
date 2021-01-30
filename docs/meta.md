<body>
#meta
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
Author: Asaf Ben-Zur <br>
Best used for: Metacarpal (Fingers), Metatarsal (Toes) <br>
This module will create a control for every root guide position, as well as a few global splay controls for the collection of controls based on settings. <br>
The play controls will behave as a global tweaker for the control collection, allowing easier animation. <br>
In order to implement "splayB" feature, simply parent a FK chain modules under each of the main meta guides. <br>
This module construction will try to detect a FK module under each guide, and if any exist, will create the second layer splay control for these FK chains. <br>
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
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td> list (controls), dict (internalSpaces), MnsNameStd (moduleSpaceAttrHost)</td></tr>
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
