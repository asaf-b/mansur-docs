<body>
#mnsFacialMocapTool
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
<h5 id = "MnsFacialMocapTool TARGET"></h5>
###MnsFacialMocapTool [Class]
<font color = #5f5f5f size = 3pt>
<i>
Spaces Tool UI Class. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>MnsFacialMocapTool(<b>parent</b>(<i>str</i>) ; [default: mnsUIUtils.get_maya_window()])</td></tr>
<tr><td><b><font color = #4caf50>Inherits from:  </font></b></td><td>form_class, base_class</td></tr>
<tr><td><b><font color = #4caf50>Class Members:  </font></b></td>
<td><ul>
<ul>
<li>pbNodes</li>
<li>col_sourceAttr</li>
<li>col_weight</li>
<li>col_min</li>
<li>col_max</li>
<li>col_isStored</li>
<li>col_sourceAttrName</li>
<li>col_index</li>
<li>poseStorage</li>
<li>sbSliderPairing</li>
<li>widgetAttrPairing</li>
</ul>
</td></tr>
<tr><td><b><font color = #4caf50>Methods:  </font></b></td><td><ul>
<li><b><a href="#addSelectedCBSourceAttrsTARGET">addSelectedCBSourceAttrs </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#addSelectedTransformsToPBTARGET">addSelectedTransformsToPB </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#clearPoseStorageTARGET">clearPoseStorage </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#connectSignalsTARGET">connectSignals </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#copyPoseTARGET">copyPose </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#createMenuTARGET">createMenu </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#createNewDefinitionTARGET">createNewDefinition </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#createSourceRowTARGET">createSourceRow </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#deletePbNodeTARGET">deletePbNode </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#editTargetTransformsTARGET">editTargetTransforms </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getAllPoseBlendNodesTARGET">getAllPoseBlendNodes </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getAllTargetTransformsTARGET">getAllTargetTransforms </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getCurrentPbSelectionTARGET">getCurrentPbSelection </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getSelectedPbNodeTARGET">getSelectedPbNode </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getSelectedSourceAttrsTARGET">getSelectedSourceAttrs </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getSelectedTargetTransformsTARGET">getSelectedTargetTransforms </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getSelectedTragetTransformsTARGET">getSelectedTragetTransforms </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#importFMDataTARGET">importFMData </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#initCreateWidgetTARGET">initCreateWidget </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#initializeSelectedPbTARGET">initializeSelectedPb </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#initializeViewTARGET">initializeView </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#initializeWidgetsTARGET">initializeWidgets </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadWindowTARGET">loadWindow </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#pbNodesMenuTARGET">pbNodesMenu </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#removeSelectedSourceAttrsTARGET">removeSelectedSourceAttrs </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#removeSelectedTransformsFromPBTARGET">removeSelectedTransformsFromPB </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#selectPbNodeTARGET">selectPbNode </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#selectTargetTransformsTARGET">selectTargetTransforms </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setCreateWidgetsModeTARGET">setCreateWidgetsMode </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setFlagCbxStateNoSignalTARGET">setFlagCbxStateNoSignal </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setFlagsForPbNodeTARGET">setFlagsForPbNode </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setSbSliderValueTARGET">setSbSliderValue </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setSourceValuesTARGET">setSourceValues </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#sourceAttrsMenuTARGET">sourceAttrsMenu </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#switchEditUIStateTARGET">switchEditUIState </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#switchUIStatesTARGET">switchUIStates </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#targetTransformsMenuTARGET">targetTransformsMenu </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#toggleCbxFlagStateTARGET">toggleCbxFlagState </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#toggleTriggerTARGET">toggleTrigger </b></a> <font size = 2pt><i>[method]</i></font></li>
</ul>
</td>
</tr>
</table></font>
####MnsFacialMocapTool  methods
<hr width = 50%>
<h5 id = "addSelectedCBSourceAttrsTARGET"></h5><font color = 464646 size = 3><b>addSelectedCBSourceAttrs <font size = 2pt> [<a href="#MnsFacialMocapTool TARGET">MnsFacialMocapTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>addSelectedCBSourceAttrs(self, **kwargs)</td></tr>
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
<h5 id = "addSelectedTransformsToPBTARGET"></h5><font color = 464646 size = 3><b>addSelectedTransformsToPB <font size = 2pt> [<a href="#MnsFacialMocapTool TARGET">MnsFacialMocapTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>addSelectedTransformsToPB(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "clearPoseStorageTARGET"></h5><font color = 464646 size = 3><b>clearPoseStorage <font size = 2pt> [<a href="#MnsFacialMocapTool TARGET">MnsFacialMocapTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>clearPoseStorage(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "connectSignalsTARGET"></h5><font color = 464646 size = 3><b>connectSignals <font size = 2pt> [<a href="#MnsFacialMocapTool TARGET">MnsFacialMocapTool </a> class method] </font></font></b>
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
<h5 id = "copyPoseTARGET"></h5><font color = 464646 size = 3><b>copyPose <font size = 2pt> [<a href="#MnsFacialMocapTool TARGET">MnsFacialMocapTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>copyPose(self, flip = False)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>flip</b>(<i>bool</i>) ; [default: False]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "createMenuTARGET"></h5><font color = 464646 size = 3><b>createMenu <font size = 2pt> [<a href="#MnsFacialMocapTool TARGET">MnsFacialMocapTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createMenu(self, position)</td></tr>
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
<h5 id = "createNewDefinitionTARGET"></h5><font color = 464646 size = 3><b>createNewDefinition <font size = 2pt> [<a href="#MnsFacialMocapTool TARGET">MnsFacialMocapTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createNewDefinition(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "createSourceRowTARGET"></h5><font color = 464646 size = 3><b>createSourceRow <font size = 2pt> [<a href="#MnsFacialMocapTool TARGET">MnsFacialMocapTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createSourceRow(self, sourceAttr)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>sourceAttr</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "deletePbNodeTARGET"></h5><font color = 464646 size = 3><b>deletePbNode <font size = 2pt> [<a href="#MnsFacialMocapTool TARGET">MnsFacialMocapTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>deletePbNode(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "editTargetTransformsTARGET"></h5><font color = 464646 size = 3><b>editTargetTransforms <font size = 2pt> [<a href="#MnsFacialMocapTool TARGET">MnsFacialMocapTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>editTargetTransforms(self, mode = 0)</td></tr>
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
<h5 id = "getAllPoseBlendNodesTARGET"></h5><font color = 464646 size = 3><b>getAllPoseBlendNodes <font size = 2pt> [<a href="#MnsFacialMocapTool TARGET">MnsFacialMocapTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getAllPoseBlendNodes(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getAllTargetTransformsTARGET"></h5><font color = 464646 size = 3><b>getAllTargetTransforms <font size = 2pt> [<a href="#MnsFacialMocapTool TARGET">MnsFacialMocapTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getAllTargetTransforms(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getCurrentPbSelectionTARGET"></h5><font color = 464646 size = 3><b>getCurrentPbSelection <font size = 2pt> [<a href="#MnsFacialMocapTool TARGET">MnsFacialMocapTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getCurrentPbSelection(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getSelectedPbNodeTARGET"></h5><font color = 464646 size = 3><b>getSelectedPbNode <font size = 2pt> [<a href="#MnsFacialMocapTool TARGET">MnsFacialMocapTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getSelectedPbNode(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getSelectedSourceAttrsTARGET"></h5><font color = 464646 size = 3><b>getSelectedSourceAttrs <font size = 2pt> [<a href="#MnsFacialMocapTool TARGET">MnsFacialMocapTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getSelectedSourceAttrs(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getSelectedTargetTransformsTARGET"></h5><font color = 464646 size = 3><b>getSelectedTargetTransforms <font size = 2pt> [<a href="#MnsFacialMocapTool TARGET">MnsFacialMocapTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getSelectedTargetTransforms(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getSelectedTragetTransformsTARGET"></h5><font color = 464646 size = 3><b>getSelectedTragetTransforms <font size = 2pt> [<a href="#MnsFacialMocapTool TARGET">MnsFacialMocapTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getSelectedTragetTransforms(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "importFMDataTARGET"></h5><font color = 464646 size = 3><b>importFMData <font size = 2pt> [<a href="#MnsFacialMocapTool TARGET">MnsFacialMocapTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>importFMData(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "initCreateWidgetTARGET"></h5><font color = 464646 size = 3><b>initCreateWidget <font size = 2pt> [<a href="#MnsFacialMocapTool TARGET">MnsFacialMocapTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>initCreateWidget(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "initializeSelectedPbTARGET"></h5><font color = 464646 size = 3><b>initializeSelectedPb <font size = 2pt> [<a href="#MnsFacialMocapTool TARGET">MnsFacialMocapTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>initializeSelectedPb(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "initializeViewTARGET"></h5><font color = 464646 size = 3><b>initializeView <font size = 2pt> [<a href="#MnsFacialMocapTool TARGET">MnsFacialMocapTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>initializeView(self, **kwargs)</td></tr>
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
<h5 id = "initializeWidgetsTARGET"></h5><font color = 464646 size = 3><b>initializeWidgets <font size = 2pt> [<a href="#MnsFacialMocapTool TARGET">MnsFacialMocapTool </a> class method] </font></font></b>
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
<h5 id = "loadWindowTARGET"></h5><font color = 464646 size = 3><b>loadWindow <font size = 2pt> [<a href="#MnsFacialMocapTool TARGET">MnsFacialMocapTool </a> class method] </font></font></b>
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
<h5 id = "pbNodesMenuTARGET"></h5><font color = 464646 size = 3><b>pbNodesMenu <font size = 2pt> [<a href="#MnsFacialMocapTool TARGET">MnsFacialMocapTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>pbNodesMenu(self, position)</td></tr>
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
<h5 id = "removeSelectedSourceAttrsTARGET"></h5><font color = 464646 size = 3><b>removeSelectedSourceAttrs <font size = 2pt> [<a href="#MnsFacialMocapTool TARGET">MnsFacialMocapTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>removeSelectedSourceAttrs(self, **kwargs)</td></tr>
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
<h5 id = "removeSelectedTransformsFromPBTARGET"></h5><font color = 464646 size = 3><b>removeSelectedTransformsFromPB <font size = 2pt> [<a href="#MnsFacialMocapTool TARGET">MnsFacialMocapTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>removeSelectedTransformsFromPB(self, **kwargs)</td></tr>
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
<h5 id = "selectPbNodeTARGET"></h5><font color = 464646 size = 3><b>selectPbNode <font size = 2pt> [<a href="#MnsFacialMocapTool TARGET">MnsFacialMocapTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>selectPbNode(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "selectTargetTransformsTARGET"></h5><font color = 464646 size = 3><b>selectTargetTransforms <font size = 2pt> [<a href="#MnsFacialMocapTool TARGET">MnsFacialMocapTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>selectTargetTransforms(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setCreateWidgetsModeTARGET"></h5><font color = 464646 size = 3><b>setCreateWidgetsMode <font size = 2pt> [<a href="#MnsFacialMocapTool TARGET">MnsFacialMocapTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setCreateWidgetsMode(self, mode = 0)</td></tr>
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
<h5 id = "setFlagCbxStateNoSignalTARGET"></h5><font color = 464646 size = 3><b>setFlagCbxStateNoSignal <font size = 2pt> [<a href="#MnsFacialMocapTool TARGET">MnsFacialMocapTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setFlagCbxStateNoSignal(self, cbx, state)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>cbx</b></li>
<li><b>state</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setFlagsForPbNodeTARGET"></h5><font color = 464646 size = 3><b>setFlagsForPbNode <font size = 2pt> [<a href="#MnsFacialMocapTool TARGET">MnsFacialMocapTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setFlagsForPbNode(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setSbSliderValueTARGET"></h5><font color = 464646 size = 3><b>setSbSliderValue <font size = 2pt> [<a href="#MnsFacialMocapTool TARGET">MnsFacialMocapTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setSbSliderValue(self, newValue)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>newValue</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setSourceValuesTARGET"></h5><font color = 464646 size = 3><b>setSourceValues <font size = 2pt> [<a href="#MnsFacialMocapTool TARGET">MnsFacialMocapTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setSourceValues(self, currentItem, previousItem)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>currentItem</b></li>
<li><b>previousItem</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "sourceAttrsMenuTARGET"></h5><font color = 464646 size = 3><b>sourceAttrsMenu <font size = 2pt> [<a href="#MnsFacialMocapTool TARGET">MnsFacialMocapTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>sourceAttrsMenu(self, position)</td></tr>
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
<h5 id = "switchEditUIStateTARGET"></h5><font color = 464646 size = 3><b>switchEditUIState <font size = 2pt> [<a href="#MnsFacialMocapTool TARGET">MnsFacialMocapTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>switchEditUIState(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "switchUIStatesTARGET"></h5><font color = 464646 size = 3><b>switchUIStates <font size = 2pt> [<a href="#MnsFacialMocapTool TARGET">MnsFacialMocapTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>switchUIStates(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "targetTransformsMenuTARGET"></h5><font color = 464646 size = 3><b>targetTransformsMenu <font size = 2pt> [<a href="#MnsFacialMocapTool TARGET">MnsFacialMocapTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>targetTransformsMenu(self, position)</td></tr>
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
<h5 id = "toggleCbxFlagStateTARGET"></h5><font color = 464646 size = 3><b>toggleCbxFlagState <font size = 2pt> [<a href="#MnsFacialMocapTool TARGET">MnsFacialMocapTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>toggleCbxFlagState(self, state)</td></tr>
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
<h5 id = "toggleTriggerTARGET"></h5><font color = 464646 size = 3><b>toggleTrigger <font size = 2pt> [<a href="#MnsFacialMocapTool TARGET">MnsFacialMocapTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>toggleTrigger(self)</td></tr>
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
###loadFacialMocapTool
<font color = #5f5f5f size = 3pt>
<i>
Load the Def Serach UI from globals, avoid UI duplication. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadFacialMocapTool() </td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
