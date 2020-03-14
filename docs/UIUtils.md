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
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
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
##Defenitions
<hr width = 100%>
###acquireExternalWindow
<font color = #5f5f5f size = 3pt>
<i>
A simple method to acquire an external QT window, into an actual PyQt MianWindow object. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>acquireExternalWindow(UIName = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>QMainWindow (UI Class)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>UIName</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###buildFormBaseClassForUI
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>buildFormBaseClassForUI(script_dir, rel_path)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>baseClass, formClass</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>script_dir</b></li>
<li><b>rel_path</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###buildTabForModuleParentDir
<font color = #5f5f5f size = 3pt>
<i>
Main BLOCK dynamiuc tab builder. <br>
Builds a tab for a given tab parent including all the neccesary layouts within, returning the main layout that can be inserted with new q items. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>buildTabForModuleParentDir(modDirName, insertIndex, tabWidget, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>modDirName</b></li>
<li><b>insertIndex</b></li>
<li><b>tabWidget</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
<td><ul>
<li><b>modSet</b>(<i>bool</i>)</li>
</ul></td>
</tr>
</table></font>
<hr width = 100%>
###checkChannelCommand
<font color = #5f5f5f size = 3pt>
<i>
DynUI 'channel control' checkBox changed command trigger. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>checkChannelCommand(chanBtn,chanCbxs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>chanBtn</b></li>
<li><b>chanCbxs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###colOverrideBlockDefTriggerCommand
<font color = #5f5f5f size = 3pt>
<i>
DynUI color-override default command trigger. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>colOverrideBlockDefTriggerCommand(colorOverrideCbx, sideCB, ovverideBtnList)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>colorOverrideCbx</b></li>
<li><b>sideCB</b></li>
<li><b>ovverideBtnList</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###colOverrideStateChange
<font color = #5f5f5f size = 3pt>
<i>
DynUI color-override changed command trigger. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>colOverrideStateChange(colorOverrideCbx, sideCB, ovverideBtnList)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>colorOverrideCbx</b></li>
<li><b>sideCB</b></li>
<li><b>ovverideBtnList</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###customScriptsAddCommand
<font color = #5f5f5f size = 3pt>
<i>
Add button trigger command for "custom scripts" slot of synamic UI. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>customScriptsAddCommand(listWidget)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>listWidget</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###customScriptsDefaultCommand
<font color = #5f5f5f size = 3pt>
<i>
Default trigger command for 'custom scripts' slot in dynUI. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>customScriptsDefaultCommand(listWidget, MnsArgumentObj)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>listWidget</b></li>
<li><b>MnsArgumentObj</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###customScriptsRemoveCommand
<font color = #5f5f5f size = 3pt>
<i>
Remove button trigger command for "custom scripts" slot of synamic UI. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>customScriptsRemoveCommand(listWidget)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>listWidget</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###deleteAllLayoutItems
<font color = #5f5f5f size = 3pt>
<i>
A method to delete all widgets/object from a given layout <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>deleteAllLayoutItems(layout, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>layout</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###drawBooleanChk
<font color = #5f5f5f size = 3pt>
<i>
Main dynamic check-box UI draw. <br>
Creates a simple boolean check-box (QCheckBox) as well as a connected 'default' button. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>drawBooleanChk(MnsArgumentObj, layoutParent)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>QCheckBox</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>MnsArgumentObj</b></li>
<li><b>layoutParent</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###drawButtonAndField
<font color = #5f5f5f size = 3pt>
<i>
Main dynamic 'button and field' draw.  <br>
Draws a deault button, text field and an 'Insert items from scene' button into the given parent layout. <br>
This function makes all relevant connections between the QItems created- <br>
- 'Load command' from the QPushButton (insert) to the text field <br>
- 'Clear' trigger for the text field. <br>
- 'Set default' from the QPushButton 'default' to the text field. <br>
These connections are made within in order the return the QLEdit only, with no need to worrie about the 'functionallity' buttons created, only the value within the text field. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>drawButtonAndField(MnsArgumentObj, layoutParent, alphaLimit = False)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>QLEdit</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>MnsArgumentObj</b></li>
<li><b>layoutParent</b></li>
<li><b>alphaLimit</b>(<i>bool</i>) ; [default: False]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###drawButtonAndFieldUnknown
<font color = #5f5f5f size = 3pt>
<i>
Main 'unknown' button and field UI draw. <br>
In case the MnsArgument.type in question is an unknown type, draw a button and field style item for it. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>drawButtonAndFieldUnknown(MnsArgumentObj, layoutParent)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>QLEdit</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>MnsArgumentObj</b></li>
<li><b>layoutParent</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###drawChannelColumnAndConnect
<font color = #5f5f5f size = 3pt>
<i>
Draw channel column (part of channel control) into a DynUI. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>drawChannelColumnAndConnect(MnsArgumentObj, channel)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>QVBoxLayout (layout), list (drawen boxes)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>MnsArgumentObj</b></li>
<li><b>channel</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###drawChannelControl
<font color = #5f5f5f size = 3pt>
<i>
Draw the predefined channel-control slot into a DynUI. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>drawChannelControl(MnsArgumentObj, layoutParent)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>list (all channel cbxs)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>MnsArgumentObj</b></li>
<li><b>layoutParent</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###drawColorBox
<font color = #5f5f5f size = 3pt>
<i>
Main dynamic 'draw color box' creation function. <br>
Will create a new QPushButton with its 'color picker' style display and inserts it into the given layoutParent. <br>
An automatic connection to the 'getColor' function is made, as well as a 'default' button creation and connection is made. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>drawColorBox(MnsArgumentObj, layoutParent)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>QPushButton</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>MnsArgumentObj</b></li>
<li><b>layoutParent</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###drawColorBtnAndConnect
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>drawColorBtnAndConnect(default, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>QPushButton</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>default</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
<td><ul>
<li><b>buttonSize</b>(<i>int</i>) ; [default: 25]</li>
<li><b>colOverrideCbx</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
</table></font>
<hr width = 100%>
###drawColorScheme
<font color = #5f5f5f size = 3pt>
<i>
Main block 'draw color scheme box' creation function. <br>
Will create a new QPushButton series with 'color picker's style display and inserts it into the given layoutParent. <br>
An automatic connection to the 'getColor' function is made, as well as a 'default' button creation and connection is made. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>drawColorScheme(MnsArgumentObj, layoutParent)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>list</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>MnsArgumentObj</b></li>
<li><b>layoutParent</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###drawColorSchemeOverride
<font color = #5f5f5f size = 3pt>
<i>
Draw the predefined 'color scheme' slot into a dynUI. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>drawColorSchemeOverride(MnsArgumentObj, layoutParent, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>list</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>MnsArgumentObj</b></li>
<li><b>layoutParent</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
<td><ul>
<li><b>sideCB</b>(<i>str</i>) ; [default: None]</li>
<li><b>colOverride</b>(<i>bool</i>)</li>
<li><b>rigTop</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
</table></font>
<hr width = 100%>
###drawCustomScriptsSlot
<font color = #5f5f5f size = 3pt>
<i>
draw a "custom scripts" slot into dyn UI. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>drawCustomScriptsSlot(MnsArgumentObj, layoutParent)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>QListWidget</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>MnsArgumentObj</b></li>
<li><b>layoutParent</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###drawFloatScroll
<font color = #5f5f5f size = 3pt>
<i>
Main dynamic "Float spinner" UI draw <br>
Creates a Float QDoubleSpinBox widget, and a default button connected to it. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>drawFloatScroll(MnsArgumentObj, layoutParent)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>QDoubleSpinBox</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>MnsArgumentObj</b></li>
<li><b>layoutParent</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###drawHorizontalDevider
<font color = #5f5f5f size = 3pt>
<i>
Draw a simple Horizontal devider into the dynUI. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>drawHorizontalDevider(MnsArgumentObj, layoutParent)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>QFrame (Horizontal line devider)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>MnsArgumentObj</b></li>
<li><b>layoutParent</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###drawIntSpinner
<font color = #5f5f5f size = 3pt>
<i>
Main dynamic 'int field' field and spinner UI draw. <br>
Creates an int QSpinBox widget, and a default button connected to it. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>drawIntSpinner(MnsArgumentObj, layoutParent)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>QSpinBox</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>MnsArgumentObj</b></li>
<li><b>layoutParent</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###drawModuleButton
<font color = #5f5f5f size = 3pt>
<i>
Main BLOCK dynamic build module buttom function draw. <br>
Builds a new QPushButoon for a given module, return the QPushButton created after connecting it to the given 'connectFunction'. <br>
The QPush buttom created will then to be inserted into a layout by the caller function. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>drawModuleButton(MnsBuildModuleObj, connectFunction)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td> QPushButton</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>MnsBuildModuleObj</b></li>
<li><b>connectFunction</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###drawOptionBox
<font color = #5f5f5f size = 3pt>
<i>
Main dynamic 'option box' draw. <br>
Drawing a new ob based on parameters within the MnsArgument object passed in. <br>
The QComboBox is inserted into the parent layout passed in. <br>
A default button and connection is made. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>drawOptionBox(MnsArgumentObj, layoutParent)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>QComboBox</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>MnsArgumentObj</b></li>
<li><b>layoutParent</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###drawPathField
<font color = #5f5f5f size = 3pt>
<i>
Main Path row draw <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>drawPathField(MnsArgumentObj, layoutParent)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>QLEdit</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>MnsArgumentObj</b></li>
<li><b>layoutParent</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###drawPrimaryButton
<font color = #5f5f5f size = 3pt>
<i>
Picker method- draw a generic picker button. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>drawPrimaryButton(plg, tabWidget, pickerBase, picker)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>plg</b></li>
<li><b>tabWidget</b></li>
<li><b>pickerBase</b></li>
<li><b>picker</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###drawSpacesBox
<font color = #5f5f5f size = 3pt>
<i>
Main dynamic 'draw spaces box' creation function. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>drawSpacesBox(MnsArgumentObj, layoutParent)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>QListWidget</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>MnsArgumentObj</b></li>
<li><b>layoutParent</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getColor
<font color = #5f5f5f size = 3pt>
<i>
Simple 'get color for a color PButton'. <br>
Creates a new QColorDialog asking the user for a color choice. <br>
When color selected sets the caller QPushButton color to the selected color <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getColor(btn, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>tuple[3] (color)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>btn</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
<td><ul>
<li><b>colOverrideCbx</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
</table></font>
<hr width = 100%>
###getColorArrayFromColorScheme
<font color = #5f5f5f size = 3pt>
<i>
Collect a normalized array of colors from a 'colorSceheme' enum attribute. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getColorArrayFromColorScheme(side, colorScheme)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>list (color sceheme)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>side</b></li>
<li><b>colorScheme</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getObjectScreenSpaceByFilmGate
<font color = #5f5f5f size = 3pt>
<i>
This method is used to 'project' a plg into the projection camera's film gate. <br>
Get the relative position of the plg to the camera film-gate's top left corener. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getObjectScreenSpaceByFilmGate(objectProj, cam)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>float, float (posX, posY)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>objectProj</b></li>
<li><b>cam</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getPathCommand
<font color = #5f5f5f size = 3pt>
<i>
Dyn UI path slot 'get path' command trigger. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getPathCommand(LEdit, mode = 0, fileTypes = [])</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>LEdit</b></li>
<li><b>mode</b>(<i>int</i>) ; [default: 0]</li>
<li><b>fileTypes</b>(<i>list</i>) ; [default: []]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getPlgPosition
<font color = #5f5f5f size = 3pt>
<i>
Get the relative position of the requested plg, based on the 'Picker Layout Base' Guide top left corner. <br>
Return the local bounding box size as well. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getPlgPosition(plg, pickerBase)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>float,float,float,float (posX,PosY,Width,Height)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>plg</b></li>
<li><b>pickerBase</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###get_maya_window
<font color = #5f5f5f size = 3pt>
<i>
Main maya window get for a global UI parent <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>get_maya_window()</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>qtWindow (main maya window as a qt window)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###listLoadCmd
<font color = #5f5f5f size = 3pt>
<i>
Load to list command trigger (dynUI) <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>listLoadCmd(QListWidget)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>QListWidget</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###listRemoveCommand
<font color = #5f5f5f size = 3pt>
<i>
Remove from list command trigger (dynUI) <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>listRemoveCommand(QListWidget)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>QListWidget</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###loadCmd
<font color = #5f5f5f size = 3pt>
<i>
Main text field 'load from scene' trigger command. <br>
This command will update the given QLEdit with members of the maya scene when triggered. <br>
Three main cases: <br>
1. Nothing is selected - if the field is empty- do nothing, else clear the field. <br>
2. objects are selected, without any CB selection - load the object names in, seperated by commas. <br>
3. Objects are selected and there is a CB selection as well - load all objects and chnnels in a 'object.channel' format, seperated by commas. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadCmd(LEdit)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>LEdit</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###load_ui_type
<font color = #5f5f5f size = 3pt>
<i>
This function converts a '.ui' file into a '.py' file live. <br>
This means that all UI's are derived from a QT designer ui files that are converted directly to form the UI. <br>
This keeps a live connection between the '.ui' file and the actul UI in maya. Meaning that any edit or a change to the UI base needs to be done only from the QT designer, without any further action by the user. <br>
It reruns a baseClass and a formClass to be used when creating any UI. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>load_ui_type(ui_file)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>baseClass, formClass</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>ui_file</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###setBooleanDefaultCmd
<font color = #5f5f5f size = 3pt>
<i>
'Set default' trigger for a QCheckBox item. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setBooleanDefaultCmd(cbx,default)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>cbx</b></li>
<li><b>default</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###setChennelControlDefaultCmd
<font color = #5f5f5f size = 3pt>
<i>
DynUI chennel control slot default command trigger. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setChennelControlDefaultCmd(cbxList, MnsArgumentObj)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>cbxList</b></li>
<li><b>MnsArgumentObj</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###setColorDefaultCmd
<font color = #5f5f5f size = 3pt>
<i>
A 'set color back to default command. <br>
A command to be triggered by an outside 'default' button, or when initializing to set the specified QPushButton color back to it's default value. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setColorDefaultCmd(btn, colorDef)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>btn</b></li>
<li><b>colorDef</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###setColorSchemeDefaultCmd
<font color = #5f5f5f size = 3pt>
<i>
DynUI color-scheme default command trigger. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setColorSchemeDefaultCmd(btnList, default)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>btnList</b></li>
<li><b>default</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###setFloatDefaultCmd
<font color = #5f5f5f size = 3pt>
<i>
'Set default' trigger for a QDoubleSpinBox item. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setFloatDefaultCmd(spinner,default)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>spinner</b></li>
<li><b>default</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###setIntDefaultCmd
<font color = #5f5f5f size = 3pt>
<i>
'Set deafult' command trigget for an int QSpinBox. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setIntDefaultCmd(spinner,default)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>spinner</b></li>
<li><b>default</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###setListWidgetDefaultCommand
<font color = #5f5f5f size = 3pt>
<i>
'Default' command trigger for a 'list' type synamic row (dynUI) <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setListWidgetDefaultCommand(QListWidget, default)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>QListWidget</b></li>
<li><b>default</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###setOtionBoxDefaultCmd
<font color = #5f5f5f size = 3pt>
<i>
A 'set default' command to be triggered for a combo box item. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setOtionBoxDefaultCmd(cbox, default)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>cbox</b></li>
<li><b>default</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###setStringDefaultCmd
<font color = #5f5f5f size = 3pt>
<i>
'Set default' command trigger from a text field <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setStringDefaultCmd(LEdit,default)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>LEdit</b></li>
<li><b>default</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###sideCBChangedTriggerCommand
<font color = #5f5f5f size = 3pt>
<i>
DynUI side combo box changed command trigger. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>sideCBChangedTriggerCommand(colorOverrideCbx, sideCB, ovverideBtnList, rigTop, ignoreOvverideCheckbox = False)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>colorOverrideCbx</b></li>
<li><b>sideCB</b></li>
<li><b>ovverideBtnList</b></li>
<li><b>rigTop</b></li>
<li><b>ignoreOvverideCheckbox</b>(<i>bool</i>) ; [default: False]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###tearOffWindow
<font color = #5f5f5f size = 3pt>
<i>
Create a new maya 'tear-off' panel. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>tearOffWindow(name, title, width, height, cameraToView)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>pymel.core.window (tear-off window)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>name</b></li>
<li><b>title</b></li>
<li><b>width</b></li>
<li><b>height</b></li>
<li><b>cameraToView</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
