<body>
#UIUtils
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur === <br>
UI Utility function assembly. <br>
This module holds all UI utility functions as well s any QT dynamic draw functions. <br>
All UI functions should be held in here for multi-usage of the same UI draw functions. <br>
 <br>
This module also holds the QT ui dynamic conversion to '.py' and the 'get_maya_window' function. <br>
 <br>
</font>
</i>
<hr width = 100%>
##Classes
<hr width = 100%>
<h5 id = "CollapsibleFrameWidget TARGET"></h5>
###CollapsibleFrameWidget [Class]
<font color = #5f5f5f size = 3pt>
<i>
Collapsible frame Widget class. <br>
This is a wrapper widget that allows for a collapisble frame to be built. <br>
The QFrame object will allow for Layouts to be inserted into the Collapsible frame, inserting any widgets within it,  <br>
collapsing and expanding it by a click trigger (from the user). <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>CollapsibleFrameWidget(<b>parent</b>(<i>str</i>) ; [default: None],<b>title</b>(<i>str</i>) ; [default: None])</td></tr>
<tr><td><b><font color = #4caf50>Inherits from:  </font></b></td><td>QFrame</td></tr>
<tr><td><b><font color = #4caf50>Class Members:  </font></b></td>
<td><ul>
<ul>
<li>_is_collasped</li>
<li>_title_frame</li>
<li>_content</li>
<li>_main_v_layout</li>
<li>clickedSignal</li>
</ul>
</td></tr>
<tr><td><b><font color = #4caf50>Methods:  </font></b></td><td><ul>
<li><b><a href="#initCollapsableTARGET">initCollapsable </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#toggleCollapsedTARGET">toggleCollapsed </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setArrowTARGET">setArrow </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#initArrowTARGET">initArrow </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#initContentTARGET">initContent </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#initTitleFrameTARGET">initTitleFrame </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#addWidgetTARGET">addWidget </b></a> <font size = 2pt><i>[method]</i></font></li>
</ul>
</td>
</tr>
</table></font>
####CollapsibleFrameWidget  methods
<hr width = 50%>
<h5 id = "initCollapsableTARGET"></h5><font color = 464646 size = 3><b>initCollapsable <font size = 2pt> [<a href="#CollapsibleFrameWidget TARGET">CollapsibleFrameWidget </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>initCollapsable(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "toggleCollapsedTARGET"></h5><font color = 464646 size = 3><b>toggleCollapsed <font size = 2pt> [<a href="#CollapsibleFrameWidget TARGET">CollapsibleFrameWidget </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>toggleCollapsed(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setArrowTARGET"></h5><font color = 464646 size = 3><b>setArrow <font size = 2pt> [<a href="#CollapsibleFrameWidget TARGET">CollapsibleFrameWidget </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setArrow(self, arrow_dir)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>baseClass, formClass</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>arrow_dir</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "initArrowTARGET"></h5><font color = 464646 size = 3><b>initArrow <font size = 2pt> [<a href="#CollapsibleFrameWidget TARGET">CollapsibleFrameWidget </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>initArrow(self, collapsed)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>collapsed</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "initContentTARGET"></h5><font color = 464646 size = 3><b>initContent <font size = 2pt> [<a href="#CollapsibleFrameWidget TARGET">CollapsibleFrameWidget </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>initContent(self, collapsed)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>collapsed</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "initTitleFrameTARGET"></h5><font color = 464646 size = 3><b>initTitleFrame <font size = 2pt> [<a href="#CollapsibleFrameWidget TARGET">CollapsibleFrameWidget </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>initTitleFrame(self, title, collapsed)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>title</b></li>
<li><b>collapsed</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "addWidgetTARGET"></h5><font color = 464646 size = 3><b>addWidget <font size = 2pt> [<a href="#CollapsibleFrameWidget TARGET">CollapsibleFrameWidget </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>addWidget(self, widget)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>widget</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
<h5 id = "MnsAbout TARGET"></h5>
###MnsAbout [Class]
<font color = #5f5f5f size = 3pt>
<i>
Mansur - About dialog <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>MnsAbout(<b>parent</b>(<i>str</i>) ; [default: get_maya_window()],<b>version</b>(<i>str</i>) ; [default: "dev"])</td></tr>
<tr><td><b><font color = #4caf50>Inherits from:  </font></b></td><td>QtWidgets.QDialog</td></tr>
<tr><td><b><font color = #4caf50>Class Members:  </font></b></td>
<td><ul>
<ul>
<li>iconsDir</li>
<li>versionDisplay</li>
<li>close_btn</li>
</ul>
</td></tr>
</tr>
</table></font>
