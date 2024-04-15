<body>
#wing
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
Author: Asaf Ben-Zur <br>
Best used for: Bird Wings <br>
This module is designed for birds (feathered) wings. <br>
This is a compound module. <br>
The main module is based on the limb module, including most of it's features. <br>
On top of the main limb module, there is a compound FK chain modules extending from each of the main modules main guides, to create a global feathers silhouette control. <br>
Out of these compounds, a grid of interp-joints is created to control the shape's deformation, using mnsPointOnCuveNode as a driver. <br>
As a bird wing is incredibly complex, controlling it precisely is incredibly difficult. <br>
With that in mind, the grid of interp joints is designed to control the overall shape of the feathers as a group, mid-controls to curl them as a group, as well as control each feather row individually. <br>
Use featherJoints attribute to define the number of feathers along the wings main skeleton. <br>
Post joint-struct creation, use the custom position adjustment attribute on the root-guide to adjust the position of the joint grid to match your needs. <br>
This module also contains multiple features to make animation even better: <br>
Feathers spring, global wave control, individual feather control, bendy limbs, extension-to-look-at for easy wing fold control. <br>
 <br>
</font>
</i>
<hr width = 100%>
##Defenitions
<hr width = 100%>
###attempFeatherParamAdjustRemap
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>attempFeatherParamAdjustRemap(mansur, rootGuide = None, previousValues = {})</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>mansur</b></li>
<li><b>rootGuide</b>(<i>str</i>) ; [default: None]</li>
<li><b>previousValues</b>(<i>dict</i>) ; [default: {}]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###collectFeathParamAdjustValues
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>collectFeathParamAdjustValues(rootGuide)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rootGuide</b></li>
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
<font color = #5f5f5f size = 3pt>
<i>
deconstruct method implementation.  <br>
Transfer interJoints control back to the main joints. <br>
</i>
<br>
</font>
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
###deleteUnusedMnsNodesFromRootGuide
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>deleteUnusedMnsNodesFromRootGuide(rootNode = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rootNode</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getNumSections
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getNumSections(tweakersPerSection, doTweakers = False)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>tweakersPerSection</b></li>
<li><b>doTweakers</b>(<i>bool</i>) ; [default: False]</li>
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
###jointStructureSoftMod
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>jointStructureSoftMod(mansur, guides, mnsBuildModule = None, **kwargs)</td></tr>
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
###moduleCompound
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>moduleCompound(mansur, bmButtonList, guides, mnsBuildModule = None, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>mansur</b></li>
<li><b>bmButtonList</b></li>
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
