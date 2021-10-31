<body>
#volumeJointsUI
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
<h5 id = "DragDoubleSpinBox TARGET"></h5>
###DragDoubleSpinBox [Class]
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>DragDoubleSpinBox(<b>parent</b>(<i>str</i>) ; [default: None])</td></tr>
<tr><td><b><font color = #4caf50>Inherits from:  </font></b></td><td>QtWidgets.QDoubleSpinBox</td></tr>
<tr><td><b><font color = #4caf50>Class Members:  </font></b></td>
<td><ul>
<ul>
<li>mouseStartPosX</li>
<li>startValue</li>
<li>inDrag</li>
<li>le</li>
</ul>
</td></tr>
<tr><td><b><font color = #4caf50>Methods:  </font></b></td><td><ul>
<li><b><a href="#mouseDragTARGET">mouseDrag </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#mouseDragEndTARGET">mouseDragEnd </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#mouseDragStartTARGET">mouseDragStart </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#eventFilterTARGET">eventFilter </b></a> <font size = 2pt><i>[method]</i></font></li>
</ul>
</td>
</tr>
</table></font>
####DragDoubleSpinBox  methods
<hr width = 50%>
<h5 id = "mouseDragTARGET"></h5><font color = 464646 size = 3><b>mouseDrag <font size = 2pt> [<a href="#DragDoubleSpinBox TARGET">DragDoubleSpinBox </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>mouseDrag(self, event)</td></tr>
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
<h5 id = "mouseDragEndTARGET"></h5><font color = 464646 size = 3><b>mouseDragEnd <font size = 2pt> [<a href="#DragDoubleSpinBox TARGET">DragDoubleSpinBox </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>mouseDragEnd(self, event)</td></tr>
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
<h5 id = "mouseDragStartTARGET"></h5><font color = 464646 size = 3><b>mouseDragStart <font size = 2pt> [<a href="#DragDoubleSpinBox TARGET">DragDoubleSpinBox </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>mouseDragStart(self, event)</td></tr>
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
<h5 id = "eventFilterTARGET"></h5><font color = 464646 size = 3><b>eventFilter <font size = 2pt> [<a href="#DragDoubleSpinBox TARGET">DragDoubleSpinBox </a> class method] </font></font></b>
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
<hr width = 100%>
<h5 id = "MnsVolumeJointsUI TARGET"></h5>
###MnsVolumeJointsUI [Class]
<font color = #5f5f5f size = 3pt>
<i>
Main UI Class <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>MnsVolumeJointsUI(<b>parent</b>(<i>str</i>) ; [default: mnsUIUtils.get_maya_window()])</td></tr>
<tr><td><b><font color = #4caf50>Inherits from:  </font></b></td><td>form_class, base_class</td></tr>
<tr><td><b><font color = #4caf50>Class Members:  </font></b></td>
<td><ul>
<ul>
<li>allCollapsible</li>
<li>allEditableWidgets</li>
<li>mayaSelectCallBack</li>
<li>blockSceneSelectCallback</li>
<li>cbxSBRelations</li>
<li>currentVJnt</li>
<li>currentVJntNode</li>
<li>currentIndex</li>
<li>currentVJntSym</li>
<li>currentVJntNodeSym</li>
<li>currentIndexSym</li>
<li>symmetryDelta</li>
<li>attrMapping</li>
</ul>
</td></tr>
<tr><td><b><font color = #4caf50>Methods:  </font></b></td><td><ul>
<li><b><a href="#createVJntTARGET">createVJnt </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#deleteVJntTARGET">deleteVJnt </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#duplicateVJntTARGET">duplicateVJnt </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#initializeUITARGET">initializeUI </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setCollapsibleWidgetsBehaviourTARGET">setCollapsibleWidgetsBehaviour </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setRestPoseForAllTARGET">setRestPoseForAll </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#symmetrizeAllTriggerTARGET">symmetrizeAllTrigger </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#symmetrizeVJTriggerTARGET">symmetrizeVJTrigger </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#updateAllEditValuesTARGET">updateAllEditValues </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#updateAnglesStateTARGET">updateAnglesState </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#drawAngleSectionTARGET">drawAngleSection </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#drawGeneralSectionTARGET">drawGeneralSection </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#refreshViewTARGET">refreshView </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#selectionChangedTriggerTARGET">selectionChangedTrigger </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setCurrentStateAsRestPoseTARGET">setCurrentStateAsRestPose </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setSymmetryVarsTARGET">setSymmetryVars </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#sceneSelectionChangedTriggerTARGET">sceneSelectionChangedTrigger </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#toggleAllCollapsedTARGET">toggleAllCollapsed </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setCurrentSBToMinOrMaxTARGET">setCurrentSBToMinOrMax </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#allEditTriggersTARGET">allEditTriggers </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#connectSignalsTARGET">connectSignals </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadWindowTARGET">loadWindow </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#eventFilterTARGET">eventFilter </b></a> <font size = 2pt><i>[method]</i></font></li>
</ul>
</td>
</tr>
</table></font>
####MnsVolumeJointsUI  methods
<hr width = 50%>
<h5 id = "createVJntTARGET"></h5><font color = 464646 size = 3><b>createVJnt <font size = 2pt> [<a href="#MnsVolumeJointsUI TARGET">MnsVolumeJointsUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createVJnt(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "deleteVJntTARGET"></h5><font color = 464646 size = 3><b>deleteVJnt <font size = 2pt> [<a href="#MnsVolumeJointsUI TARGET">MnsVolumeJointsUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>deleteVJnt(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "duplicateVJntTARGET"></h5><font color = 464646 size = 3><b>duplicateVJnt <font size = 2pt> [<a href="#MnsVolumeJointsUI TARGET">MnsVolumeJointsUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>duplicateVJnt(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "initializeUITARGET"></h5><font color = 464646 size = 3><b>initializeUI <font size = 2pt> [<a href="#MnsVolumeJointsUI TARGET">MnsVolumeJointsUI </a> class method] </font></font></b>
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
<h5 id = "setCollapsibleWidgetsBehaviourTARGET"></h5><font color = 464646 size = 3><b>setCollapsibleWidgetsBehaviour <font size = 2pt> [<a href="#MnsVolumeJointsUI TARGET">MnsVolumeJointsUI </a> class method] </font></font></b>
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
<h5 id = "setRestPoseForAllTARGET"></h5><font color = 464646 size = 3><b>setRestPoseForAll <font size = 2pt> [<a href="#MnsVolumeJointsUI TARGET">MnsVolumeJointsUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setRestPoseForAll(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "symmetrizeAllTriggerTARGET"></h5><font color = 464646 size = 3><b>symmetrizeAllTrigger <font size = 2pt> [<a href="#MnsVolumeJointsUI TARGET">MnsVolumeJointsUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>symmetrizeAllTrigger(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "symmetrizeVJTriggerTARGET"></h5><font color = 464646 size = 3><b>symmetrizeVJTrigger <font size = 2pt> [<a href="#MnsVolumeJointsUI TARGET">MnsVolumeJointsUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>symmetrizeVJTrigger(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "updateAllEditValuesTARGET"></h5><font color = 464646 size = 3><b>updateAllEditValues <font size = 2pt> [<a href="#MnsVolumeJointsUI TARGET">MnsVolumeJointsUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>updateAllEditValues(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "updateAnglesStateTARGET"></h5><font color = 464646 size = 3><b>updateAnglesState <font size = 2pt> [<a href="#MnsVolumeJointsUI TARGET">MnsVolumeJointsUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>updateAnglesState(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "drawAngleSectionTARGET"></h5><font color = 464646 size = 3><b>drawAngleSection <font size = 2pt> [<a href="#MnsVolumeJointsUI TARGET">MnsVolumeJointsUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>drawAngleSection(self, **kwargs)</td></tr>
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
<h5 id = "drawGeneralSectionTARGET"></h5><font color = 464646 size = 3><b>drawGeneralSection <font size = 2pt> [<a href="#MnsVolumeJointsUI TARGET">MnsVolumeJointsUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>drawGeneralSection(self, **kwargs)</td></tr>
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
<h5 id = "refreshViewTARGET"></h5><font color = 464646 size = 3><b>refreshView <font size = 2pt> [<a href="#MnsVolumeJointsUI TARGET">MnsVolumeJointsUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>refreshView(self, **kwargs)</td></tr>
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
<h5 id = "selectionChangedTriggerTARGET"></h5><font color = 464646 size = 3><b>selectionChangedTrigger <font size = 2pt> [<a href="#MnsVolumeJointsUI TARGET">MnsVolumeJointsUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>selectionChangedTrigger(self, **kwargs)</td></tr>
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
<h5 id = "setCurrentStateAsRestPoseTARGET"></h5><font color = 464646 size = 3><b>setCurrentStateAsRestPose <font size = 2pt> [<a href="#MnsVolumeJointsUI TARGET">MnsVolumeJointsUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setCurrentStateAsRestPose(self, **kwargs)</td></tr>
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
<h5 id = "setSymmetryVarsTARGET"></h5><font color = 464646 size = 3><b>setSymmetryVars <font size = 2pt> [<a href="#MnsVolumeJointsUI TARGET">MnsVolumeJointsUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setSymmetryVars(self, **kwargs)</td></tr>
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
<h5 id = "sceneSelectionChangedTriggerTARGET"></h5><font color = 464646 size = 3><b>sceneSelectionChangedTrigger <font size = 2pt> [<a href="#MnsVolumeJointsUI TARGET">MnsVolumeJointsUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>sceneSelectionChangedTrigger(self, dummy = None)</td></tr>
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
<h5 id = "toggleAllCollapsedTARGET"></h5><font color = 464646 size = 3><b>toggleAllCollapsed <font size = 2pt> [<a href="#MnsVolumeJointsUI TARGET">MnsVolumeJointsUI </a> class method] </font></font></b>
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
<h5 id = "setCurrentSBToMinOrMaxTARGET"></h5><font color = 464646 size = 3><b>setCurrentSBToMinOrMax <font size = 2pt> [<a href="#MnsVolumeJointsUI TARGET">MnsVolumeJointsUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setCurrentSBToMinOrMax(self, sourceWidget, targetWidget)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>sourceWidget</b></li>
<li><b>targetWidget</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "allEditTriggersTARGET"></h5><font color = 464646 size = 3><b>allEditTriggers <font size = 2pt> [<a href="#MnsVolumeJointsUI TARGET">MnsVolumeJointsUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>allEditTriggers(self, widget = None, value = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>widget</b>(<i>str</i>) ; [default: None]</li>
<li><b>value</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "connectSignalsTARGET"></h5><font color = 464646 size = 3><b>connectSignals <font size = 2pt> [<a href="#MnsVolumeJointsUI TARGET">MnsVolumeJointsUI </a> class method] </font></font></b>
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
<h5 id = "loadWindowTARGET"></h5><font color = 464646 size = 3><b>loadWindow <font size = 2pt> [<a href="#MnsVolumeJointsUI TARGET">MnsVolumeJointsUI </a> class method] </font></font></b>
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
<h5 id = "eventFilterTARGET"></h5><font color = 464646 size = 3><b>eventFilter <font size = 2pt> [<a href="#MnsVolumeJointsUI TARGET">MnsVolumeJointsUI </a> class method] </font></font></b>
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
<hr width = 100%>
##Defenitions
<hr width = 100%>
###loadVolumeJointsUI
<font color = #5f5f5f size = 3pt>
<i>
Load the cns tool UI from globals, avoid UI duplication. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadVolumeJointsUI()</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###volJointStateChangedCB
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>volJointStateChangedCB(msg, plug, otherPlug, clientData, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>msg</b></li>
<li><b>plug</b></li>
<li><b>otherPlug</b></li>
<li><b>clientData</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
