<body>
#LODsTool
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
<h5 id = "MnsLodsTool TARGET"></h5>
###MnsLodsTool [Class]
<font color = #5f5f5f size = 3pt>
<i>
Spaces Tool UI Class. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>MnsLodsTool(<b>parent</b>(<i>str</i>) ; [default: mnsUIUtils.get_maya_window()])</td></tr>
<tr><td><b><font color = #4caf50>Inherits from:  </font></b></td><td>form_class, base_class</td></tr>
<tr><td><b><font color = #4caf50>Class Members:  </font></b></td>
<td><ul>
<ul>
<li>rigTops</li>
<li>rigTop</li>
<li>puppetRoot</li>
<li>namespace</li>
<li>rootGuide</li>
<li>lodVisAttr</li>
</ul>
</td></tr>
<tr><td><b><font color = #4caf50>Methods:  </font></b></td><td><ul>
<li><b><a href="#addLodTARGET">addLod </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#addSelectedItemsTARGET">addSelectedItems </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#clearALLLodsTARGET">clearALLLods </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#connectSignalsTARGET">connectSignals </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#convertLodsDictKeysToIntsTARGET">convertLodsDictKeysToInts </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#deleteLODTARGET">deleteLOD </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#drawLODsViewTARGET">drawLODsView </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#initializeUITARGET">initializeUI </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#initializeViewTARGET">initializeView </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadWindowTARGET">loadWindow </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#openMenuTARGET">openMenu </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#readDataFromUITARGET">readDataFromUI </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#removeSlectedItemsTARGET">removeSlectedItems </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setAttrHostTARGET">setAttrHost </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setLodStyleTARGET">setLodStyle </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setRigTopTARGET">setRigTop </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setSelectedItemsTARGET">setSelectedItems </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#updateLODAttrStateTARGET">updateLODAttrState </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#writeDataTARGET">writeData </b></a> <font size = 2pt><i>[method]</i></font></li>
</ul>
</td>
</tr>
</table></font>
####MnsLodsTool  methods
<hr width = 50%>
<h5 id = "addLodTARGET"></h5><font color = 464646 size = 3><b>addLod <font size = 2pt> [<a href="#MnsLodsTool TARGET">MnsLodsTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>addLod(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "addSelectedItemsTARGET"></h5><font color = 464646 size = 3><b>addSelectedItems <font size = 2pt> [<a href="#MnsLodsTool TARGET">MnsLodsTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>addSelectedItems(self, index = 0)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>index</b>(<i>int</i>) ; [default: 0]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "clearALLLodsTARGET"></h5><font color = 464646 size = 3><b>clearALLLods <font size = 2pt> [<a href="#MnsLodsTool TARGET">MnsLodsTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>clearALLLods(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "connectSignalsTARGET"></h5><font color = 464646 size = 3><b>connectSignals <font size = 2pt> [<a href="#MnsLodsTool TARGET">MnsLodsTool </a> class method] </font></font></b>
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
<h5 id = "convertLodsDictKeysToIntsTARGET"></h5><font color = 464646 size = 3><b>convertLodsDictKeysToInts <font size = 2pt> [<a href="#MnsLodsTool TARGET">MnsLodsTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>convertLodsDictKeysToInts(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "deleteLODTARGET"></h5><font color = 464646 size = 3><b>deleteLOD <font size = 2pt> [<a href="#MnsLodsTool TARGET">MnsLodsTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>deleteLOD(self, index = 0)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>index</b>(<i>int</i>) ; [default: 0]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "drawLODsViewTARGET"></h5><font color = 464646 size = 3><b>drawLODsView <font size = 2pt> [<a href="#MnsLodsTool TARGET">MnsLodsTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>drawLODsView(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "initializeUITARGET"></h5><font color = 464646 size = 3><b>initializeUI <font size = 2pt> [<a href="#MnsLodsTool TARGET">MnsLodsTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>initializeUI(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "initializeViewTARGET"></h5><font color = 464646 size = 3><b>initializeView <font size = 2pt> [<a href="#MnsLodsTool TARGET">MnsLodsTool </a> class method] </font></font></b>
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
<h5 id = "loadWindowTARGET"></h5><font color = 464646 size = 3><b>loadWindow <font size = 2pt> [<a href="#MnsLodsTool TARGET">MnsLodsTool </a> class method] </font></font></b>
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
<h5 id = "openMenuTARGET"></h5><font color = 464646 size = 3><b>openMenu <font size = 2pt> [<a href="#MnsLodsTool TARGET">MnsLodsTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>openMenu(self, position)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>position</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "readDataFromUITARGET"></h5><font color = 464646 size = 3><b>readDataFromUI <font size = 2pt> [<a href="#MnsLodsTool TARGET">MnsLodsTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>readDataFromUI(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "removeSlectedItemsTARGET"></h5><font color = 464646 size = 3><b>removeSlectedItems <font size = 2pt> [<a href="#MnsLodsTool TARGET">MnsLodsTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>removeSlectedItems(self, index = 0)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>index</b>(<i>int</i>) ; [default: 0]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setAttrHostTARGET"></h5><font color = 464646 size = 3><b>setAttrHost <font size = 2pt> [<a href="#MnsLodsTool TARGET">MnsLodsTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setAttrHost(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setLodStyleTARGET"></h5><font color = 464646 size = 3><b>setLodStyle <font size = 2pt> [<a href="#MnsLodsTool TARGET">MnsLodsTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setLodStyle(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setRigTopTARGET"></h5><font color = 464646 size = 3><b>setRigTop <font size = 2pt> [<a href="#MnsLodsTool TARGET">MnsLodsTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setRigTop(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setSelectedItemsTARGET"></h5><font color = 464646 size = 3><b>setSelectedItems <font size = 2pt> [<a href="#MnsLodsTool TARGET">MnsLodsTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setSelectedItems(self, index = 0)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>index</b>(<i>int</i>) ; [default: 0]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "updateLODAttrStateTARGET"></h5><font color = 464646 size = 3><b>updateLODAttrState <font size = 2pt> [<a href="#MnsLodsTool TARGET">MnsLodsTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>updateLODAttrState(self, index = 0)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>index</b>(<i>int</i>) ; [default: 0]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "writeDataTARGET"></h5><font color = 464646 size = 3><b>writeData <font size = 2pt> [<a href="#MnsLodsTool TARGET">MnsLodsTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>writeData(self)</td></tr>
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
###loadLodsTool
<font color = #5f5f5f size = 3pt>
<i>
Load the Def Serach UI from globals, avoid UI duplication. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadLodsTool() </td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
