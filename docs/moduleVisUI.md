<body>
#moduleVisUI
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur === <br>
 <br>
</font>
</i>
<hr width = 100%>
##Classes
<hr width = 100%>
<h5 id = "MnsModuleVisUI TARGET"></h5>
###MnsModuleVisUI [Class]
<font color = #5f5f5f size = 3pt>
<i>
Main UI Class <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>MnsModuleVisUI(<b>parent</b>(<i>str</i>) ; [default: mnsUIUtils.get_maya_window()])</td></tr>
<tr><td><b><font color = #4caf50>Inherits from:  </font></b></td><td>form_class, base_class</td></tr>
<tr><td><b><font color = #4caf50>Class Members:  </font></b></td>
<td><ul>
<ul>
<li>rigTop</li>
<li>puppetRoot</li>
<li>origin</li>
<li>rubberBand</li>
<li>moduleAttrs</li>
</ul>
</td></tr>
<tr><td><b><font color = #4caf50>Methods:  </font></b></td><td><ul>
<li><b><a href="#drawTitleRowTARGET">drawTitleRow </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#drawUITARGET">drawUI </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#filterModuleAttrsTARGET">filterModuleAttrs </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#initializeUIStateTARGET">initializeUIState </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setRowVisBasedOnStateTARGET">setRowVisBasedOnState </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#sortModuleAttrsTARGET">sortModuleAttrs </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#dawModuleRowTARGET">dawModuleRow </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#connectSignalsTARGET">connectSignals </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadWindowTARGET">loadWindow </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#eventFilterTARGET">eventFilter </b></a> <font size = 2pt><i>[method]</i></font></li>
</ul>
</td>
</tr>
</table></font>
####MnsModuleVisUI  methods
<hr width = 50%>
<h5 id = "drawTitleRowTARGET"></h5><font color = 464646 size = 3><b>drawTitleRow <font size = 2pt> [<a href="#MnsModuleVisUI TARGET">MnsModuleVisUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>drawTitleRow(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "drawUITARGET"></h5><font color = 464646 size = 3><b>drawUI <font size = 2pt> [<a href="#MnsModuleVisUI TARGET">MnsModuleVisUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>drawUI(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "filterModuleAttrsTARGET"></h5><font color = 464646 size = 3><b>filterModuleAttrs <font size = 2pt> [<a href="#MnsModuleVisUI TARGET">MnsModuleVisUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>filterModuleAttrs(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "initializeUIStateTARGET"></h5><font color = 464646 size = 3><b>initializeUIState <font size = 2pt> [<a href="#MnsModuleVisUI TARGET">MnsModuleVisUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>initializeUIState(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setRowVisBasedOnStateTARGET"></h5><font color = 464646 size = 3><b>setRowVisBasedOnState <font size = 2pt> [<a href="#MnsModuleVisUI TARGET">MnsModuleVisUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setRowVisBasedOnState(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "sortModuleAttrsTARGET"></h5><font color = 464646 size = 3><b>sortModuleAttrs <font size = 2pt> [<a href="#MnsModuleVisUI TARGET">MnsModuleVisUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>sortModuleAttrs(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "dawModuleRowTARGET"></h5><font color = 464646 size = 3><b>dawModuleRow <font size = 2pt> [<a href="#MnsModuleVisUI TARGET">MnsModuleVisUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>dawModuleRow(self, attr = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>attr</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "connectSignalsTARGET"></h5><font color = 464646 size = 3><b>connectSignals <font size = 2pt> [<a href="#MnsModuleVisUI TARGET">MnsModuleVisUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Connect all UI signals</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>connectSignals(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "loadWindowTARGET"></h5><font color = 464646 size = 3><b>loadWindow <font size = 2pt> [<a href="#MnsModuleVisUI TARGET">MnsModuleVisUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Main UI load</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadWindow(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "eventFilterTARGET"></h5><font color = 464646 size = 3><b>eventFilter <font size = 2pt> [<a href="#MnsModuleVisUI TARGET">MnsModuleVisUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Override event filter to catch the tear off to override it's event.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>eventFilter(self, source, event)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>source</b></li>
<li><b>event</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
