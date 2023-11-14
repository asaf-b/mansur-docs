<body>
#mnsAnimationExporter
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
<h5 id = "ExtraAttributesListWidget TARGET"></h5>
###ExtraAttributesListWidget [Class]
<font color = #5f5f5f size = 3pt>
<i>
A simple QPushButton re-implementation. <br>
This reimplementation is used to control the button's mouse events, used in 'Edit' mode. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>ExtraAttributesListWidget(<b>parent</b>(<i>str</i>) ; [default: None],<b>default_extraAttrs</b>(<i>list</i>) ; [default: []],<b>**kwargs</b>)</td></tr>
<tr><td><b><font color = #4caf50>Inherits from:  </font></b></td><td>QtWidgets.QListWidget</td></tr>
<tr><td><b><font color = #4caf50>Class Members:  </font></b></td>
<td><ul>
<ul>
<li>parent</li>
<li>acceptedAttributeTypes</li>
</ul>
</td></tr>
<tr><td><b><font color = #4caf50>Methods:  </font></b></td><td><ul>
<li><b><a href="#copyListTARGET">copyList </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getItemsTARGET">getItems </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#removeSelectedItemsTARGET">removeSelectedItems </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#addAttributesToListTARGET">addAttributesToList </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#pasteListTARGET">pasteList </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#validateAttributeTARGET">validateAttribute </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#openExtraAttrsMenuTARGET">openExtraAttrsMenu </b></a> <font size = 2pt><i>[method]</i></font></li>
</ul>
</td>
</tr>
</table></font>
####ExtraAttributesListWidget  methods
<hr width = 50%>
<h5 id = "copyListTARGET"></h5><font color = 464646 size = 3><b>copyList <font size = 2pt> [<a href="#ExtraAttributesListWidget TARGET">ExtraAttributesListWidget </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>copyList(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getItemsTARGET"></h5><font color = 464646 size = 3><b>getItems <font size = 2pt> [<a href="#ExtraAttributesListWidget TARGET">ExtraAttributesListWidget </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getItems(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "removeSelectedItemsTARGET"></h5><font color = 464646 size = 3><b>removeSelectedItems <font size = 2pt> [<a href="#ExtraAttributesListWidget TARGET">ExtraAttributesListWidget </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>removeSelectedItems(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "addAttributesToListTARGET"></h5><font color = 464646 size = 3><b>addAttributesToList <font size = 2pt> [<a href="#ExtraAttributesListWidget TARGET">ExtraAttributesListWidget </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>addAttributesToList(self, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "pasteListTARGET"></h5><font color = 464646 size = 3><b>pasteList <font size = 2pt> [<a href="#ExtraAttributesListWidget TARGET">ExtraAttributesListWidget </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>pasteList(self, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "validateAttributeTARGET"></h5><font color = 464646 size = 3><b>validateAttribute <font size = 2pt> [<a href="#ExtraAttributesListWidget TARGET">ExtraAttributesListWidget </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>validateAttribute(self, node, attributeName)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>node</b></li>
<li><b>attributeName</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "openExtraAttrsMenuTARGET"></h5><font color = 464646 size = 3><b>openExtraAttrsMenu <font size = 2pt> [<a href="#ExtraAttributesListWidget TARGET">ExtraAttributesListWidget </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>openExtraAttrsMenu(self, position)</td></tr>
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
<hr width = 100%>
<h5 id = "MnsAnimationExporter TARGET"></h5>
###MnsAnimationExporter [Class]
<font color = #5f5f5f size = 3pt>
<i>
Spaces Tool UI Class. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>MnsAnimationExporter(<b>parent</b>(<i>str</i>) ; [default: mnsUIUtils.get_maya_window()])</td></tr>
<tr><td><b><font color = #4caf50>Inherits from:  </font></b></td><td>form_class, base_class</td></tr>
<tr><td><b><font color = #4caf50>Class Members:  </font></b></td>
<td><ul>
<ul>
<li>infoNode</li>
<li>ranges_vs</li>
<li>extraAttrsClipboard</li>
</ul>
</td></tr>
<tr><td><b><font color = #4caf50>Methods:  </font></b></td><td><ul>
<li><b><a href="#deleteRangeTARGET">deleteRange </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#exportTARGET">export </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#gatherDataTARGET">gatherData </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#initializeViewTARGET">initializeView </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#initializeWidgetsTARGET">initializeWidgets </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadUIInfoTARGET">loadUIInfo </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#random_colorTARGET">random_color </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#resetUITARGET">resetUI </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#validateUIInfoNodeTARGET">validateUIInfoNode </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#addRangeTARGET">addRange </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadWSAnimDataTARGET">loadWSAnimData </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#writeDefaultDataTARGET">writeDefaultData </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#saveWSAnimDataTARGET">saveWSAnimData </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getRangePathTARGET">getRangePath </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getSkinnedMeshesFromJntHeirarchyTARGET">getSkinnedMeshesFromJntHeirarchy </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#extractSkeletonFromRigTopTARGET">extractSkeletonFromRigTop </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#bakeExtraAttributesTARGET">bakeExtraAttributes </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getUnusedJointsTARGET">getUnusedJoints </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#restructureJointHeirarchyTARGET">restructureJointHeirarchy </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setRangeModeTARGET">setRangeMode </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#connectSignalsTARGET">connectSignals </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadWindowTARGET">loadWindow </b></a> <font size = 2pt><i>[method]</i></font></li>
</ul>
</td>
</tr>
</table></font>
####MnsAnimationExporter  methods
<hr width = 50%>
<h5 id = "deleteRangeTARGET"></h5><font color = 464646 size = 3><b>deleteRange <font size = 2pt> [<a href="#MnsAnimationExporter TARGET">MnsAnimationExporter </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>deleteRange(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "exportTARGET"></h5><font color = 464646 size = 3><b>export <font size = 2pt> [<a href="#MnsAnimationExporter TARGET">MnsAnimationExporter </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>export(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "gatherDataTARGET"></h5><font color = 464646 size = 3><b>gatherData <font size = 2pt> [<a href="#MnsAnimationExporter TARGET">MnsAnimationExporter </a> class method] </font></font></b>
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
<h5 id = "initializeViewTARGET"></h5><font color = 464646 size = 3><b>initializeView <font size = 2pt> [<a href="#MnsAnimationExporter TARGET">MnsAnimationExporter </a> class method] </font></font></b>
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
<h5 id = "initializeWidgetsTARGET"></h5><font color = 464646 size = 3><b>initializeWidgets <font size = 2pt> [<a href="#MnsAnimationExporter TARGET">MnsAnimationExporter </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>initializeWidgets(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "loadUIInfoTARGET"></h5><font color = 464646 size = 3><b>loadUIInfo <font size = 2pt> [<a href="#MnsAnimationExporter TARGET">MnsAnimationExporter </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadUIInfo(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "random_colorTARGET"></h5><font color = 464646 size = 3><b>random_color <font size = 2pt> [<a href="#MnsAnimationExporter TARGET">MnsAnimationExporter </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>random_color(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "resetUITARGET"></h5><font color = 464646 size = 3><b>resetUI <font size = 2pt> [<a href="#MnsAnimationExporter TARGET">MnsAnimationExporter </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>resetUI(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "validateUIInfoNodeTARGET"></h5><font color = 464646 size = 3><b>validateUIInfoNode <font size = 2pt> [<a href="#MnsAnimationExporter TARGET">MnsAnimationExporter </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>validateUIInfoNode(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "addRangeTARGET"></h5><font color = 464646 size = 3><b>addRange <font size = 2pt> [<a href="#MnsAnimationExporter TARGET">MnsAnimationExporter </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>addRange(self, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "loadWSAnimDataTARGET"></h5><font color = 464646 size = 3><b>loadWSAnimData <font size = 2pt> [<a href="#MnsAnimationExporter TARGET">MnsAnimationExporter </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadWSAnimData(self, animData)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>animData</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "writeDefaultDataTARGET"></h5><font color = 464646 size = 3><b>writeDefaultData <font size = 2pt> [<a href="#MnsAnimationExporter TARGET">MnsAnimationExporter </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>writeDefaultData(self, exportRanges)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>exportRanges</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "saveWSAnimDataTARGET"></h5><font color = 464646 size = 3><b>saveWSAnimData <font size = 2pt> [<a href="#MnsAnimationExporter TARGET">MnsAnimationExporter </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>saveWSAnimData(self, joints, rangeMin, rangeMax)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>joints</b></li>
<li><b>rangeMin</b></li>
<li><b>rangeMax</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getRangePathTARGET"></h5><font color = 464646 size = 3><b>getRangePath <font size = 2pt> [<a href="#MnsAnimationExporter TARGET">MnsAnimationExporter </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getRangePath(self, lineEditWidget)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>lineEditWidget</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getSkinnedMeshesFromJntHeirarchyTARGET"></h5><font color = 464646 size = 3><b>getSkinnedMeshesFromJntHeirarchy <font size = 2pt> [<a href="#MnsAnimationExporter TARGET">MnsAnimationExporter </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getSkinnedMeshesFromJntHeirarchy(self, origRootJnt)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>origRootJnt</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "extractSkeletonFromRigTopTARGET"></h5><font color = 464646 size = 3><b>extractSkeletonFromRigTop <font size = 2pt> [<a href="#MnsAnimationExporter TARGET">MnsAnimationExporter </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>extractSkeletonFromRigTop(self, rigTop, extractMode, rotToJointOrient, includeMeshes, messageLog)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>rigTop</b></li>
<li><b>extractMode</b></li>
<li><b>rotToJointOrient</b></li>
<li><b>includeMeshes</b></li>
<li><b>messageLog</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "bakeExtraAttributesTARGET"></h5><font color = 464646 size = 3><b>bakeExtraAttributes <font size = 2pt> [<a href="#MnsAnimationExporter TARGET">MnsAnimationExporter </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>bakeExtraAttributes(self, rng, host)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>rng</b></li>
<li><b>host</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getUnusedJointsTARGET"></h5><font color = 464646 size = 3><b>getUnusedJoints <font size = 2pt> [<a href="#MnsAnimationExporter TARGET">MnsAnimationExporter </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getUnusedJoints(self, rootJnt, skinData)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>rootJnt</b></li>
<li><b>skinData</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "restructureJointHeirarchyTARGET"></h5><font color = 464646 size = 3><b>restructureJointHeirarchy <font size = 2pt> [<a href="#MnsAnimationExporter TARGET">MnsAnimationExporter </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>restructureJointHeirarchy(self, rootJnt, unusedInfluences)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>rootJnt</b></li>
<li><b>unusedInfluences</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setRangeModeTARGET"></h5><font color = 464646 size = 3><b>setRangeMode <font size = 2pt> [<a href="#MnsAnimationExporter TARGET">MnsAnimationExporter </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setRangeMode(self, widgets, isAsset)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>widgets</b></li>
<li><b>isAsset</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "connectSignalsTARGET"></h5><font color = 464646 size = 3><b>connectSignals <font size = 2pt> [<a href="#MnsAnimationExporter TARGET">MnsAnimationExporter </a> class method] </font></font></b>
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
<h5 id = "loadWindowTARGET"></h5><font color = 464646 size = 3><b>loadWindow <font size = 2pt> [<a href="#MnsAnimationExporter TARGET">MnsAnimationExporter </a> class method] </font></font></b>
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
<hr width = 100%>
##Defenitions
<hr width = 100%>
###loadAnimationExporter
<font color = #5f5f5f size = 3pt>
<i>
Load the Def Serach UI from globals, avoid UI duplication. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadAnimationExporter() </td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
