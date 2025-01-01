<body>
#schemeEditor
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
PluginRelease UI Class. <br>
=== Author: Assaf Ben Zur === <br>
 <br>
</font>
</i>
<hr width = 100%>
##Classes
<hr width = 100%>
<h5 id = "ColorPushBtn TARGET"></h5>
###ColorPushBtn [Class]
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>ColorPushBtn(<b>parent</b>(<i>str</i>) ; [default: None],<b>**kwargs</b>)</td></tr>
<tr><td><b><font color = #4caf50>Inherits from:  </font></b></td><td>QtWidgets.QPushButton</td></tr>
<tr><td><b><font color = #4caf50>Class Members:  </font></b></td>
<td><ul>
<ul>
<li>colorStore</li>
<li>colorSet</li>
<li>slaves</li>
<li>parentWindow</li>
</ul>
</td></tr>
<tr><td><b><font color = #4caf50>Methods:  </font></b></td><td><ul>
<li><b><a href="#finalizeColorSetTARGET">finalizeColorSet </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getColorTARGET">getColor </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setColorTARGET">setColor </b></a> <font size = 2pt><i>[method]</i></font></li>
</ul>
</td>
</tr>
</table></font>
####ColorPushBtn  methods
<hr width = 50%>
<h5 id = "finalizeColorSetTARGET"></h5><font color = 464646 size = 3><b>finalizeColorSet <font size = 2pt> [<a href="#ColorPushBtn TARGET">ColorPushBtn </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>finalizeColorSet(self, result)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>result</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getColorTARGET"></h5><font color = 464646 size = 3><b>getColor <font size = 2pt> [<a href="#ColorPushBtn TARGET">ColorPushBtn </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getColor(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setColorTARGET"></h5><font color = 464646 size = 3><b>setColor <font size = 2pt> [<a href="#ColorPushBtn TARGET">ColorPushBtn </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setColor(self, color = "#535252", setSlaves = False, skipLive = False)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>color</b>(<i>str</i>) ; [default: "#535252"]</li>
<li><b>setSlaves</b>(<i>bool</i>) ; [default: False]</li>
<li><b>skipLive</b>(<i>bool</i>) ; [default: False]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
<h5 id = "MnsSchemeEditor TARGET"></h5>
###MnsSchemeEditor [Class]
<font color = #5f5f5f size = 3pt>
<i>
pluginRelease UI class <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>MnsSchemeEditor(<b>parent</b>(<i>str</i>) ; [default: mnsUIUtils.get_maya_window()])</td></tr>
<tr><td><b><font color = #4caf50>Inherits from:  </font></b></td><td>form_class, base_class</td></tr>
<tr><td><b><font color = #4caf50>Class Members:  </font></b></td>
<td><ul>
<ul>
<li>undostack</li>
<li>colorsSet</li>
<li>colorWidgetDict</li>
<li>blockWin</li>
</ul>
</td></tr>
<tr><td><b><font color = #4caf50>Methods:  </font></b></td><td><ul>
<li><b><a href="#connectSignalsTARGET">connectSignals </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#exportSchemeTARGET">exportScheme </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#gatherDataTARGET">gatherData </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#gatherStyleTARGET">gatherStyle </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getBlockWinTARGET">getBlockWin </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#initUITARGET">initUI </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#initWidgetsTARGET">initWidgets </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#keyPressEventTARGET">keyPressEvent </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadWindowTARGET">loadWindow </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#saveToGlobalsTARGET">saveToGlobals </b></a> <font size = 2pt><i>[method]</i></font></li>
</ul>
</td>
</tr>
</table></font>
####MnsSchemeEditor  methods
<hr width = 50%>
<h5 id = "connectSignalsTARGET"></h5><font color = 464646 size = 3><b>connectSignals <font size = 2pt> [<a href="#MnsSchemeEditor TARGET">MnsSchemeEditor </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Connect all the UI signals</i><br>
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
<h5 id = "exportSchemeTARGET"></h5><font color = 464646 size = 3><b>exportScheme <font size = 2pt> [<a href="#MnsSchemeEditor TARGET">MnsSchemeEditor </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>exportScheme(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "gatherDataTARGET"></h5><font color = 464646 size = 3><b>gatherData <font size = 2pt> [<a href="#MnsSchemeEditor TARGET">MnsSchemeEditor </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>gatherData(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "gatherStyleTARGET"></h5><font color = 464646 size = 3><b>gatherStyle <font size = 2pt> [<a href="#MnsSchemeEditor TARGET">MnsSchemeEditor </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>gatherStyle(self, applyToGlobals = False)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>applyToGlobals</b>(<i>bool</i>) ; [default: False]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getBlockWinTARGET"></h5><font color = 464646 size = 3><b>getBlockWin <font size = 2pt> [<a href="#MnsSchemeEditor TARGET">MnsSchemeEditor </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getBlockWin(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "initUITARGET"></h5><font color = 464646 size = 3><b>initUI <font size = 2pt> [<a href="#MnsSchemeEditor TARGET">MnsSchemeEditor </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>initUI(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "initWidgetsTARGET"></h5><font color = 464646 size = 3><b>initWidgets <font size = 2pt> [<a href="#MnsSchemeEditor TARGET">MnsSchemeEditor </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>initWidgets(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "keyPressEventTARGET"></h5><font color = 464646 size = 3><b>keyPressEvent <font size = 2pt> [<a href="#MnsSchemeEditor TARGET">MnsSchemeEditor </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>keyPressEvent(self, event)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>event</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "loadWindowTARGET"></h5><font color = 464646 size = 3><b>loadWindow <font size = 2pt> [<a href="#MnsSchemeEditor TARGET">MnsSchemeEditor </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Main window load</i><br>
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
<h5 id = "saveToGlobalsTARGET"></h5><font color = 464646 size = 3><b>saveToGlobals <font size = 2pt> [<a href="#MnsSchemeEditor TARGET">MnsSchemeEditor </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>saveToGlobals(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
<h5 id = "setColorUndoCommand TARGET"></h5>
###setColorUndoCommand [Class]
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setColorUndoCommand(<b>oldColor</b>,<b>newColor</b>,<b>parent</b>(<i>str</i>) ; [default: None])</td></tr>
<tr><td><b><font color = #4caf50>Inherits from:  </font></b></td><td>QUndoCommand</td></tr>
<tr><td><b><font color = #4caf50>Class Members:  </font></b></td>
<td><ul>
<ul>
<li>senderWidget</li>
<li>oldColor</li>
<li>newColor</li>
</ul>
</td></tr>
<tr><td><b><font color = #4caf50>Methods:  </font></b></td><td><ul>
<li><b><a href="#redoTARGET">redo </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#undoTARGET">undo </b></a> <font size = 2pt><i>[method]</i></font></li>
</ul>
</td>
</tr>
</table></font>
####setColorUndoCommand  methods
<hr width = 50%>
<h5 id = "redoTARGET"></h5><font color = 464646 size = 3><b>redo <font size = 2pt> [<a href="#setColorUndoCommand TARGET">setColorUndoCommand </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>redo(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "undoTARGET"></h5><font color = 464646 size = 3><b>undo <font size = 2pt> [<a href="#setColorUndoCommand TARGET">setColorUndoCommand </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>undo(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
##Defenitions
<hr width = 100%>
###loadSchemeEditor
<font color = #5f5f5f size = 3pt>
<i>
Load the plugin Release UI from globals, avoid UI duplication. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadSchemeEditor()</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
