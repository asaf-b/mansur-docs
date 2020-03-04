<body>
#buildModules
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur === <br>
This is the core BLOCK Build-Modules class library. <br>
This package contains the three main classes for BLOCK: <br>
- MnsBuildModuleBtn <br>
- MnsRig <br>
- MnsBuildModule <br>
 <br>
Most core function are defined within the classes, although any external functionality is maintained in 'blockUtility' py module. <br>
The objective of these classes are mainly effeciant data gathering, constructing and deconstructing modules within a rig group. <br>
 <br>
</font>
</i>
<hr width = 100%>
##Classes
<hr width = 100%>
<h5 id = "MnsBuildModule TARGET"></h5>
###MnsBuildModule [Class]
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>MnsBuildModule(<b>MnsBuildModuleButton</b>,<b>**kwargs</b>)</td></tr>
<tr><td><b><font color = #4caf50>Inherits from:  </font></b></td><td>MnsRig</td></tr>
<tr><td><b><font color = #4caf50>Class Members:  </font></b></td>
<td><ul>
<ul>
<li>MnsBuildModuleButton</li>
<li>sidePlaceHolder</li>
<li>builtGuides</li>
<li>rigTop</li>
<li>rootGuide</li>
<li>rootCtrl</li>
<li>guideControls</li>
<li>cGuideControls</li>
<li>pureParent</li>
<li>moduleTop</li>
<li>extraSpaces</li>
<li>pureTops</li>
<li>spaceSwitchCtrls</li>
<li>controls</li>
<li>allControls</li>
<li>puppetTopCtrl</li>
</ul>
</td></tr>
<tr><td><b><font color = #4caf50>Methods:  </font></b></td><td><ul>
<li><b><a href="#connectVisChannelsTARGET">connectVisChannels </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#constructTARGET">construct </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#constructSpacesTARGET">constructSpaces </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#gatherAllDependeciesTARGET">gatherAllDependecies </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#gatherRelatedCtrlsTARGET">gatherRelatedCtrls </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#gatherRelatedGuidesTARGET">gatherRelatedGuides </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getRigTopTARGET">getRigTop </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#reCollectControlsFromLocalsTARGET">reCollectControlsFromLocals </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#buildGuideObjectsTARGET">buildGuideObjects </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#deconstructTARGET">deconstruct </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#updateCreationArgsToSymmetryModeTARGET">updateCreationArgsToSymmetryMode </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#createGuidesTARGET">createGuides </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#buildGuidesTARGET">buildGuides </b></a> <font size = 2pt><i>[method]</i></font></li>
</ul>
</td>
</tr>
</table></font>
####MnsBuildModule  methods
<hr width = 50%>
<h5 id = "connectVisChannelsTARGET"></h5><font color = 464646 size = 3><b>connectVisChannels <font size = 2pt> [<a href="#MnsBuildModule TARGET">MnsBuildModule </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>connectVisChannels(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "constructTARGET"></h5><font color = 464646 size = 3><b>construct <font size = 2pt> [<a href="#MnsBuildModule TARGET">MnsBuildModule </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>construct(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "constructSpacesTARGET"></h5><font color = 464646 size = 3><b>constructSpaces <font size = 2pt> [<a href="#MnsBuildModule TARGET">MnsBuildModule </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>constructSpaces(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "gatherAllDependeciesTARGET"></h5><font color = 464646 size = 3><b>gatherAllDependecies <font size = 2pt> [<a href="#MnsBuildModule TARGET">MnsBuildModule </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>gatherAllDependecies(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "gatherRelatedCtrlsTARGET"></h5><font color = 464646 size = 3><b>gatherRelatedCtrls <font size = 2pt> [<a href="#MnsBuildModule TARGET">MnsBuildModule </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>gatherRelatedCtrls(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "gatherRelatedGuidesTARGET"></h5><font color = 464646 size = 3><b>gatherRelatedGuides <font size = 2pt> [<a href="#MnsBuildModule TARGET">MnsBuildModule </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>gatherRelatedGuides(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getRigTopTARGET"></h5><font color = 464646 size = 3><b>getRigTop <font size = 2pt> [<a href="#MnsBuildModule TARGET">MnsBuildModule </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getRigTop(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "reCollectControlsFromLocalsTARGET"></h5><font color = 464646 size = 3><b>reCollectControlsFromLocals <font size = 2pt> [<a href="#MnsBuildModule TARGET">MnsBuildModule </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>reCollectControlsFromLocals(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "buildGuideObjectsTARGET"></h5><font color = 464646 size = 3><b>buildGuideObjects <font size = 2pt> [<a href="#MnsBuildModule TARGET">MnsBuildModule </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>buildGuideObjects(self, **kwargs)</td></tr>
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
<h5 id = "deconstructTARGET"></h5><font color = 464646 size = 3><b>deconstruct <font size = 2pt> [<a href="#MnsBuildModule TARGET">MnsBuildModule </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>deconstruct(self, mnsRig)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>mnsRig</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "updateCreationArgsToSymmetryModeTARGET"></h5><font color = 464646 size = 3><b>updateCreationArgsToSymmetryMode <font size = 2pt> [<a href="#MnsBuildModule TARGET">MnsBuildModule </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>updateCreationArgsToSymmetryMode(self, optArgs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>optArgs</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "createGuidesTARGET"></h5><font color = 464646 size = 3><b>createGuides <font size = 2pt> [<a href="#MnsBuildModule TARGET">MnsBuildModule </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createGuides(self, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
<td><ul>
<li><b>blkSide</b>(<i>str</i>) ; [default: center]</li>
<li><b>body</b>(<i>str</i>) ; [default: guideCtrl]</li>
<li><b>alpha</b>(<i>str</i>) ; [default: A]</li>
</ul></td>
</tr>
</table></font>
<h5 id = "buildGuidesTARGET"></h5><font color = 464646 size = 3><b>buildGuides <font size = 2pt> [<a href="#MnsBuildModule TARGET">MnsBuildModule </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>buildGuides(self, MnsBuildModuleButton, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>MnsBuildModuleButton</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
<td><ul>
<li><b>skipUI</b>(<i>bool</i>)</li>
<li><b>settingsHolder</b>(<i>str</i>) ; [default: None]</li>
<li><b>symmetrize</b>(<i>bool</i>)</li>
</ul></td>
</tr>
</table></font>
<hr width = 100%>
<h5 id = "MnsBuildModuleBtn TARGET"></h5>
###MnsBuildModuleBtn [Class]
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>MnsBuildModuleBtn(<b>path</b>,<b>**kwargs</b>)</td></tr>
<tr><td><b><font color = #4caf50>Inherits from:  </font></b></td><td>object</td></tr>
<tr><td><b><font color = #4caf50>Class Members:  </font></b></td>
<td><ul>
<ul>
<li>layoutParent</li>
<li>path</li>
<li>moduleName</li>
<li>groupType</li>
<li>shortName</li>
<li>mayaNative</li>
<li>moduleUISettings</li>
</ul>
</td></tr>
</tr>
</table></font>
<hr width = 100%>
<h5 id = "MnsRig TARGET"></h5>
###MnsRig [Class]
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>MnsRig(<b>callerSubClass</b>(<i>str</i>) ; [default: None],<b>**kwargs</b>)</td></tr>
<tr><td><b><font color = #4caf50>Inherits from:  </font></b></td><td>object</td></tr>
<tr><td><b><font color = #4caf50>Class Members:  </font></b></td>
<td><ul>
<ul>
<li>rigTop</li>
<li>callerSubClass</li>
<li>modules</li>
<li>buildModulesBtns</li>
<li>puppetBase</li>
<li>baseGuide</li>
<li>rootJnt</li>
<li>loadSettingsWindow</li>
</ul>
</td></tr>
<tr><td><b><font color = #4caf50>Methods:  </font></b></td><td><ul>
<li><b><a href="#cunstructRigSpacesTARGET">cunstructRigSpaces </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#destroyPuppetRootCtrlTARGET">destroyPuppetRootCtrl </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getGlobalConstructionStateTARGET">getGlobalConstructionState </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setConstructionModeTARGET">setConstructionMode </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setVisChannelsBasedOnCunstructModeTARGET">setVisChannelsBasedOnCunstructMode </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#collectBuildModulesTARGET">collectBuildModules </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#constructRigTARGET">constructRig </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#createNewRigTopTARGET">createNewRigTop </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#deconstructRigTARGET">deconstructRig </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadSettingsWindowTARGET">loadSettingsWindow </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#createSubGrpsForRigTopTARGET">createSubGrpsForRigTop </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#createPickerLayoutBaseTARGET">createPickerLayoutBase </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#createPuppetRootCtrlTARGET">createPuppetRootCtrl </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#createPickerProjectionCamTARGET">createPickerProjectionCam </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#createPickerCamTARGET">createPickerCam </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#createPickerGuideGrpTARGET">createPickerGuideGrp </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#createPickerTitleGrpTARGET">createPickerTitleGrp </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#createRootGuideTARGET">createRootGuide </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#createVisEnumAndConnectTARGET">createVisEnumAndConnect </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#createSubGroupForRigTopTARGET">createSubGroupForRigTop </b></a> <font size = 2pt><i>[method]</i></font></li>
</ul>
</td>
</tr>
</table></font>
####MnsRig  methods
<hr width = 50%>
<h5 id = "cunstructRigSpacesTARGET"></h5><font color = 464646 size = 3><b>cunstructRigSpaces <font size = 2pt> [<a href="#MnsRig TARGET">MnsRig </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>cunstructRigSpaces(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "destroyPuppetRootCtrlTARGET"></h5><font color = 464646 size = 3><b>destroyPuppetRootCtrl <font size = 2pt> [<a href="#MnsRig TARGET">MnsRig </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>destroyPuppetRootCtrl(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getGlobalConstructionStateTARGET"></h5><font color = 464646 size = 3><b>getGlobalConstructionState <font size = 2pt> [<a href="#MnsRig TARGET">MnsRig </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getGlobalConstructionState(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setConstructionModeTARGET"></h5><font color = 464646 size = 3><b>setConstructionMode <font size = 2pt> [<a href="#MnsRig TARGET">MnsRig </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setConstructionMode(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setVisChannelsBasedOnCunstructModeTARGET"></h5><font color = 464646 size = 3><b>setVisChannelsBasedOnCunstructMode <font size = 2pt> [<a href="#MnsRig TARGET">MnsRig </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setVisChannelsBasedOnCunstructMode(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "collectBuildModulesTARGET"></h5><font color = 464646 size = 3><b>collectBuildModules <font size = 2pt> [<a href="#MnsRig TARGET">MnsRig </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>collectBuildModules(self, **kwargs)</td></tr>
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
<h5 id = "constructRigTARGET"></h5><font color = 464646 size = 3><b>constructRig <font size = 2pt> [<a href="#MnsRig TARGET">MnsRig </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>constructRig(self, **kwargs)</td></tr>
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
<h5 id = "createNewRigTopTARGET"></h5><font color = 464646 size = 3><b>createNewRigTop <font size = 2pt> [<a href="#MnsRig TARGET">MnsRig </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createNewRigTop(self, **kwargs)</td></tr>
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
<h5 id = "deconstructRigTARGET"></h5><font color = 464646 size = 3><b>deconstructRig <font size = 2pt> [<a href="#MnsRig TARGET">MnsRig </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>deconstructRig(self, **kwargs)</td></tr>
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
<h5 id = "loadSettingsWindowTARGET"></h5><font color = 464646 size = 3><b>loadSettingsWindow <font size = 2pt> [<a href="#MnsRig TARGET">MnsRig </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadSettingsWindow(self, **kwargs)</td></tr>
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
<h5 id = "createSubGrpsForRigTopTARGET"></h5><font color = 464646 size = 3><b>createSubGrpsForRigTop <font size = 2pt> [<a href="#MnsRig TARGET">MnsRig </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createSubGrpsForRigTop(self, rigTop)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>rigTop</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "createPickerLayoutBaseTARGET"></h5><font color = 464646 size = 3><b>createPickerLayoutBase <font size = 2pt> [<a href="#MnsRig TARGET">MnsRig </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createPickerLayoutBase(self, rigTop, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>rigTop</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "createPuppetRootCtrlTARGET"></h5><font color = 464646 size = 3><b>createPuppetRootCtrl <font size = 2pt> [<a href="#MnsRig TARGET">MnsRig </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createPuppetRootCtrl(self, rigTop, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>rigTop</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "createPickerProjectionCamTARGET"></h5><font color = 464646 size = 3><b>createPickerProjectionCam <font size = 2pt> [<a href="#MnsRig TARGET">MnsRig </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createPickerProjectionCam(self, rigTop, pickerLayoutBase)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>rigTop</b></li>
<li><b>pickerLayoutBase</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "createPickerCamTARGET"></h5><font color = 464646 size = 3><b>createPickerCam <font size = 2pt> [<a href="#MnsRig TARGET">MnsRig </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createPickerCam(self, rigTop, pickerLayoutBase, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>rigTop</b></li>
<li><b>pickerLayoutBase</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "createPickerGuideGrpTARGET"></h5><font color = 464646 size = 3><b>createPickerGuideGrp <font size = 2pt> [<a href="#MnsRig TARGET">MnsRig </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createPickerGuideGrp(self, rigTop, pickerLayoutBase, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>rigTop</b></li>
<li><b>pickerLayoutBase</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "createPickerTitleGrpTARGET"></h5><font color = 464646 size = 3><b>createPickerTitleGrp <font size = 2pt> [<a href="#MnsRig TARGET">MnsRig </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createPickerTitleGrp(self, rigTop, pickerLayoutBase,**kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>rigTop</b></li>
<li><b>pickerLayoutBase</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "createRootGuideTARGET"></h5><font color = 464646 size = 3><b>createRootGuide <font size = 2pt> [<a href="#MnsRig TARGET">MnsRig </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createRootGuide(self, rigTopNameStd, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>rigTopNameStd</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "createVisEnumAndConnectTARGET"></h5><font color = 464646 size = 3><b>createVisEnumAndConnect <font size = 2pt> [<a href="#MnsRig TARGET">MnsRig </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createVisEnumAndConnect(self, masterStd, slaveStd, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>masterStd</b></li>
<li><b>slaveStd</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
<td><ul>
<li><b>default</b>(<i>int</i>) ; [default: 1]</li>
</ul></td>
</tr>
</table></font>
<h5 id = "createSubGroupForRigTopTARGET"></h5><font color = 464646 size = 3><b>createSubGroupForRigTop <font size = 2pt> [<a href="#MnsRig TARGET">MnsRig </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createSubGroupForRigTop(self, rigTopNameStd, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>rigTopNameStd</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
<td><ul>
<li><b>subGrpType</b>(<i>str</i>)</li>
<li><b>default</b>(<i>int</i>) ; [default: 1]</li>
</ul></td>
</tr>
</table></font>
