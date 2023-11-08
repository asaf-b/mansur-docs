<body>
#linkChain
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
Author: Asaf Ben-Zur <br>
Best used for: Tank-Treads, Bike-Chains, Ferris-Wheel, Tire, Conveyor-Belt <br>
This is a comprehensive module, to create a link-chain style behaviour. <br>
Originally created for tank-treads, but can be used for a range of components. <br>
On creation, based on the number on the numberOfLinks setting, joints will be created on a circle Nurbs curve with shapeSections setting amount. <br>
After creation, the shape can be tweaked to fit any need.  <br>
IMPORTANT NOTE: This module requires a joint-struct-rebuild once the Nurbs shape has been tweaked. <br>
Once the joint-struct is revuilt, the joints will be layed out uniformally along the given shape. <br>
Upon construction, a main control will be created for controlling the entire position of the module. <br>
Under, a chain-driver control will be created. Rotating it will drive the joint chain along the curve in both forwards and backwards directions. <br>
Also, use the shape-tweak layer to create a tweak feature for the shape on construction. This will allow manipulation of the shape dynamically while the chain is driven. <br>
Automatic drive based on position is also possible wihin this module using the AutoDrive layer. <br>
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
###createUpCurveFromSamples
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createUpCurveFromSamples(mansur, rootGuide, samples, upCurveOffset)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>mansur</b></li>
<li><b>rootGuide</b></li>
<li><b>samples</b></li>
<li><b>upCurveOffset</b></li>
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
deconstruct method implementation for linkChain. <br>
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
###filterValidShapeTweakers
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>filterValidShapeTweakers(tweakersList = [], mansur = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>tweakersList</b>(<i>list</i>) ; [default: []]</li>
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
