<body>
#freeControl
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
Author: Asaf Ben-Zur <br>
Best used for: Free objects, General Control, Mesh Tweaker, Mesh Local Tweaker <br>
This Module is a general single control at it's base state. <br>
It also contains a Mesh-Tweaker feature that will allow you to create a "Double Directional" tweaker- meaning that the control will follow the input Mesh's position (Rivet) and will also be able to affect it. <br>
This effect is also commonly knowen as the "Dorito-Effect". <br>
This feature also includes a "local" mode, to tunnel deformations from the control to a local skinCluster, then a blend-shape to the main Mesh, creating multi-layered skinned mesh. <br>
All of these features will use the main joint as the effector. <br>
Note: When using the "Mesh-Tweaker" feture, when needing to affect a mesh that will also be used as the rivet input- make sure "sameMeshAffector" is set to ON. <br>
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
