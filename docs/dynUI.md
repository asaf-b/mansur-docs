<body>
#dynUI
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur === <br>
Supporting module for the 'defSearch' UI Class. <br>
This module build the base UI for any function UI build called from the defSerach UI. <br>
The build is based on a .ui base file, constructing an empty UI that will accomedate the dynamic UI elemnts requested. <br>
This module also holds the RunCmd. The run command will filter and get any elemnt value based on it's type and recompile an argument string to pass into the function requested. <br>
A template icon is created as well as an empty 'title' item to be changed after creation base on the function name requested. <br>
</font>
</i>
<hr width = 100%>
##Classes
<hr width = 100%>
<h5 id = "MnsDynamicDefUI TARGET"></h5>
###MnsDynamicDefUI [Class]
<font color = #5f5f5f size = 3pt>
<i>
Main UI class <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>MnsDynamicDefUI(<b>defenition</b>,<b>parent</b>(<i>str</i>) ; [default: mnsUIUtils.get_maya_window()],<b>**kwargs</b>)</td></tr>
<tr><td><b><font color = #4caf50>Inherits from:  </font></b></td><td>form_class, base_class</td></tr>
<tr><td><b><font color = #4caf50>Class Members:  </font></b></td>
<td><ul>
<ul>
<li>funObjectCreation</li>
<li>defenition</li>
<li>arguments</li>
<li>optArguments</li>
<li>txtFields</li>
<li>defenitionName</li>
<li>title</li>
<li>preDefinedArgs</li>
<li>sideCB</li>
<li>colOverride</li>
<li>rigTop</li>
<li>split</li>
<li>splitLayout</li>
<li>dividerLayout</li>
<li>allCollapsible</li>
<li>mainVLayout</li>
<li>customRunCommand</li>
<li>fullList</li>
</ul>
</td></tr>
<tr><td><b><font color = #4caf50>Methods:  </font></b></td><td><ul>
<li><b><a href="#setCollapsibleWidgetsBehaviourTARGET">setCollapsibleWidgetsBehaviour </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#closeEventTARGET">closeEvent </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#keyPressEventTARGET">keyPressEvent </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#toggleAllCollapsedTARGET">toggleAllCollapsed </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#assembleFeildValuesTARGET">assembleFeildValues </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#drawUITARGET">drawUI </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadUITARGET">loadUI </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#runCmdTARGET">runCmd </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#drawTitleTARGET">drawTitle </b></a> <font size = 2pt><i>[method]</i></font></li>
</ul>
</td>
</tr>
</table></font>
####MnsDynamicDefUI  methods
<hr width = 50%>
<h5 id = "setCollapsibleWidgetsBehaviourTARGET"></h5><font color = 464646 size = 3><b>setCollapsibleWidgetsBehaviour <font size = 2pt> [<a href="#MnsDynamicDefUI TARGET">MnsDynamicDefUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setCollapsibleWidgetsBehaviour(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "closeEventTARGET"></h5><font color = 464646 size = 3><b>closeEvent <font size = 2pt> [<a href="#MnsDynamicDefUI TARGET">MnsDynamicDefUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>closeEvent(self, event)</td></tr>
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
<h5 id = "keyPressEventTARGET"></h5><font color = 464646 size = 3><b>keyPressEvent <font size = 2pt> [<a href="#MnsDynamicDefUI TARGET">MnsDynamicDefUI </a> class method] </font></font></b>
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
<h5 id = "toggleAllCollapsedTARGET"></h5><font color = 464646 size = 3><b>toggleAllCollapsed <font size = 2pt> [<a href="#MnsDynamicDefUI TARGET">MnsDynamicDefUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>toggleAllCollapsed(self, pressedColWid)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>pressedColWid</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "assembleFeildValuesTARGET"></h5><font color = 464646 size = 3><b>assembleFeildValues <font size = 2pt> [<a href="#MnsDynamicDefUI TARGET">MnsDynamicDefUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Assemble all UI values into a list</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>assembleFeildValues(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>list</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "drawUITARGET"></h5><font color = 464646 size = 3><b>drawUI <font size = 2pt> [<a href="#MnsDynamicDefUI TARGET">MnsDynamicDefUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Main UI draw method.</i><br>
</font>
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
<h5 id = "loadUITARGET"></h5><font color = 464646 size = 3><b>loadUI <font size = 2pt> [<a href="#MnsDynamicDefUI TARGET">MnsDynamicDefUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Main UI load.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadUI(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "runCmdTARGET"></h5><font color = 464646 size = 3><b>runCmd <font size = 2pt> [<a href="#MnsDynamicDefUI TARGET">MnsDynamicDefUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Main method run command trigger.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>runCmd(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "drawTitleTARGET"></h5><font color = 464646 size = 3><b>drawTitle <font size = 2pt> [<a href="#MnsDynamicDefUI TARGET">MnsDynamicDefUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Title set method.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>drawTitle(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
