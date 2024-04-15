<body>
#curveZipB
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
Author: Asaf Ben-Zur <br>
Best used for: Eyelids, Eyelashes <br>
This facial module was created to allow adavnced control over eyelids and eyelashes. <br>
Based on settings, this module will create a very flexible control over eyelids, and if choosen (Attachment Curves) to eyelashes on top of the eyelids as well. <br>
The main features of this modules are: Joint positions based on a center matrix (Around the eye), Blink controls, Blink height control, Eyelid tweak controls (dynamic), Zip controls, and much more. <br>
The joint structure of this module will be dictated by input vertices on a given mesh. <br>
Note: Please select upper and lower vertices along a single closed loop <br>
 <br>
</font>
</i>
<hr width = 100%>
##Defenitions
<hr width = 100%>
###connectCustomGuidesToPoc
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>connectCustomGuidesToPoc(mansur, guides, cGuides)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>mansur</b></li>
<li><b>guides</b></li>
<li><b>cGuides</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
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
###createBindCurvesFromModuleSettings
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createBindCurvesFromModuleSettings(mansur, rootGuide = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>mansur</b></li>
<li><b>rootGuide</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###createTangentsForCtrl
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createTangentsForCtrl(mansur, MnsBuildModule, ctrl, btcNode, cornerACtrl, cornerBCtrl, nameID, doCornerTangents, mainCtrl)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>mansur</b></li>
<li><b>MnsBuildModule</b></li>
<li><b>ctrl</b></li>
<li><b>btcNode</b></li>
<li><b>cornerACtrl</b></li>
<li><b>cornerBCtrl</b></li>
<li><b>nameID</b></li>
<li><b>doCornerTangents</b></li>
<li><b>mainCtrl</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###customGuides
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>customGuides(mansur, builtGuides)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>mansur</b></li>
<li><b>builtGuides</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###deconstruct
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>deconstruct(mansur, MnsBuildModule, **kwargs)</td></tr>
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
###getEdgesFromModuleSettings
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getEdgesFromModuleSettings(mansur, rootGuide = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>mansur</b></li>
<li><b>rootGuide</b>(<i>str</i>) ; [default: None]</li>
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
