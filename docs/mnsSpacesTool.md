<body>
#mnsSpacesTool
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur === <br>
This simple animation tool was created to allow animators to space switch and IK->FK switch easily. <br>
This tool is selection based. Please select controls to enable relevant capabilities. <br>
For spaces, simply select the controls you want to act upon, choose your target spaces, and press "switch". This will switch the space, while maintaining the controls's transforms, using keys created automatically. <br>
For Limbs, simple select any control/s for the limbs that you wish to act upon, and press the relevant button- To-IK or To-FK. <br>
This will switch the limb/controls to the selected state.  <br>
This tool also includes Auto-Key switches, as well as a sequence and bake modes.  <br>
 <br>
</font>
</i>
<hr width = 100%>
##Classes
<hr width = 100%>
<h5 id = "MnsSpacesTool TARGET"></h5>
###MnsSpacesTool [Class]
<font color = #5f5f5f size = 3pt>
<i>
Spaces Tool UI Class. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>MnsSpacesTool(<b>parent</b>(<i>str</i>) ; [default: mnsUIUtils.get_maya_window()])</td></tr>
<tr><td><b><font color = #4caf50>Inherits from:  </font></b></td><td>form_class, base_class</td></tr>
<tr><td><b><font color = #4caf50>Class Members:  </font></b></td>
<td><ul>
<ul>
<li>mayaSelectCallBack</li>
<li>mayaTimeChangedCallBack</li>
<li>limbs</li>
<li>spaceCtrls</li>
</ul>
</td></tr>
<tr><td><b><font color = #4caf50>Methods:  </font></b></td><td><ul>
<li><b><a href="#connectSignalsTARGET">connectSignals </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#eventFilterTARGET">eventFilter </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#fkIKSwitchTARGET">fkIKSwitch </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getFramesListFromUIStateTARGET">getFramesListFromUIState </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getSpaceEnumIndexByNameTARGET">getSpaceEnumIndexByName </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#initializeViewTARGET">initializeView </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#insertCallbacksTARGET">insertCallbacks </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadWindowTARGET">loadWindow </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#removeCallbacksTARGET">removeCallbacks </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#sceneSelectionChangedTARGET">sceneSelectionChanged </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#selectIKFKHostTARGET">selectIKFKHost </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setAutoKeyModeTARGET">setAutoKeyMode </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setAvailbleLimbsTARGET">setAvailbleLimbs </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setAvailbleSpacesTARGET">setAvailbleSpaces </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setIKFKViewTARGET">setIKFKView </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setSequenceModeTARGET">setSequenceMode </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setSequenceRangeTARGET">setSequenceRange </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setSpacesModeTARGET">setSpacesMode </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setSpacesViewTARGET">setSpacesView </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#spaceSwitchTARGET">spaceSwitch </b></a> <font size = 2pt><i>[method]</i></font></li>
</ul>
</td>
</tr>
</table></font>
####MnsSpacesTool  methods
<hr width = 50%>
<h5 id = "connectSignalsTARGET"></h5><font color = 464646 size = 3><b>connectSignals <font size = 2pt> [<a href="#MnsSpacesTool TARGET">MnsSpacesTool </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Connect all UI Signals.</i><br>
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
<h5 id = "eventFilterTARGET"></h5><font color = 464646 size = 3><b>eventFilter <font size = 2pt> [<a href="#MnsSpacesTool TARGET">MnsSpacesTool </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Override event filter to catch the close trigger to delete the callback</i><br>
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
<h5 id = "fkIKSwitchTARGET"></h5><font color = 464646 size = 3><b>fkIKSwitch <font size = 2pt> [<a href="#MnsSpacesTool TARGET">MnsSpacesTool </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>mode 0 - Match FK to IK</i><br>
<i>mode 1 - Match IK to FK</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>fkIKSwitch(self, mode = 0)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>mode</b>(<i>int</i>) ; [default: 0]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getFramesListFromUIStateTARGET"></h5><font color = 464646 size = 3><b>getFramesListFromUIState <font size = 2pt> [<a href="#MnsSpacesTool TARGET">MnsSpacesTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getFramesListFromUIState(self, hostCtrl = None, attrName = "")</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>hostCtrl</b>(<i>str</i>) ; [default: None]</li>
<li><b>attrName</b>(<i>str</i>) ; [default: ""]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getSpaceEnumIndexByNameTARGET"></h5><font color = 464646 size = 3><b>getSpaceEnumIndexByName <font size = 2pt> [<a href="#MnsSpacesTool TARGET">MnsSpacesTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getSpaceEnumIndexByName(self, node, attr, targetSpaceName)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>node</b></li>
<li><b>attr</b></li>
<li><b>targetSpaceName</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "initializeViewTARGET"></h5><font color = 464646 size = 3><b>initializeView <font size = 2pt> [<a href="#MnsSpacesTool TARGET">MnsSpacesTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>initializeView(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "insertCallbacksTARGET"></h5><font color = 464646 size = 3><b>insertCallbacks <font size = 2pt> [<a href="#MnsSpacesTool TARGET">MnsSpacesTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>insertCallbacks(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "loadWindowTARGET"></h5><font color = 464646 size = 3><b>loadWindow <font size = 2pt> [<a href="#MnsSpacesTool TARGET">MnsSpacesTool </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Show window method.</i><br>
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
<h5 id = "removeCallbacksTARGET"></h5><font color = 464646 size = 3><b>removeCallbacks <font size = 2pt> [<a href="#MnsSpacesTool TARGET">MnsSpacesTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>removeCallbacks(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "sceneSelectionChangedTARGET"></h5><font color = 464646 size = 3><b>sceneSelectionChanged <font size = 2pt> [<a href="#MnsSpacesTool TARGET">MnsSpacesTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>sceneSelectionChanged(self, dummy = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>dummy</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "selectIKFKHostTARGET"></h5><font color = 464646 size = 3><b>selectIKFKHost <font size = 2pt> [<a href="#MnsSpacesTool TARGET">MnsSpacesTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>selectIKFKHost(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setAutoKeyModeTARGET"></h5><font color = 464646 size = 3><b>setAutoKeyMode <font size = 2pt> [<a href="#MnsSpacesTool TARGET">MnsSpacesTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setAutoKeyMode(self, state)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>state</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setAvailbleLimbsTARGET"></h5><font color = 464646 size = 3><b>setAvailbleLimbs <font size = 2pt> [<a href="#MnsSpacesTool TARGET">MnsSpacesTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setAvailbleLimbs(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setAvailbleSpacesTARGET"></h5><font color = 464646 size = 3><b>setAvailbleSpaces <font size = 2pt> [<a href="#MnsSpacesTool TARGET">MnsSpacesTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setAvailbleSpaces(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setIKFKViewTARGET"></h5><font color = 464646 size = 3><b>setIKFKView <font size = 2pt> [<a href="#MnsSpacesTool TARGET">MnsSpacesTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setIKFKView(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setSequenceModeTARGET"></h5><font color = 464646 size = 3><b>setSequenceMode <font size = 2pt> [<a href="#MnsSpacesTool TARGET">MnsSpacesTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setSequenceMode(self, state)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>state</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setSequenceRangeTARGET"></h5><font color = 464646 size = 3><b>setSequenceRange <font size = 2pt> [<a href="#MnsSpacesTool TARGET">MnsSpacesTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setSequenceRange(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setSpacesModeTARGET"></h5><font color = 464646 size = 3><b>setSpacesMode <font size = 2pt> [<a href="#MnsSpacesTool TARGET">MnsSpacesTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setSpacesMode(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setSpacesViewTARGET"></h5><font color = 464646 size = 3><b>setSpacesView <font size = 2pt> [<a href="#MnsSpacesTool TARGET">MnsSpacesTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setSpacesView(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "spaceSwitchTARGET"></h5><font color = 464646 size = 3><b>spaceSwitch <font size = 2pt> [<a href="#MnsSpacesTool TARGET">MnsSpacesTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>spaceSwitch(self)</td></tr>
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
###loadSpacesTool
<font color = #5f5f5f size = 3pt>
<i>
Load the Def Serach UI from globals, avoid UI duplication. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadSpacesTool() </td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
