<body>
#logviewer
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur === <br>
Core Mns log viewer class UI. <br>
This is a core utility UI to allow an admin or a user to read any mns log item in a readable manner. <br>
This UI allows many filtering abilities to nicely view a log, which by itself is human unredablble. <br>
 <br>
Features: <br>
- log tree view tab to manipulate/remove/add/reload files and directories. <br>
- 'Depth View' option to cascade the log view based on log depth. <br>
- log items flagging and commenting <br>
- Search ability <br>
- Filtering : <br>
&nbsp;&nbsp;&nbsp;&nbsp;- Time based filtering <br>
&nbsp;&nbsp;&nbsp;&nbsp;- Flag based filtering <br>
&nbsp;&nbsp;&nbsp;&nbsp;- Severity based filtering <br>
- log exporting <br>
- log clearing <br>
- flag scroll feature <br>
 <br>
IMPORTANT NOTE: <br>
Log files are being created automatically within the core logger based on project settings. <br>
There is a core log-file size management within the logger NOT whithin this module. <br>
The max-log file size can be changed through the global mns settings. <br>
File management is being handled when writing logs- the logger will check whether the curent file to write has passed it's limit before writing. <br>
If found that it does, before writing the new log a set number of lines will be automatically deleted from the beggening of the log file. <br>
In order to maintain preformance more then one line is being deleted each time, as re-reading and re-writing of the log will be quite slow in case of the need to do so each time a new log line needs to be entered when the file size has passed it's limit. <br>
When deleting multiple lines the logger only needs to do so every once for every x (50-100) logs entered when file size is approaching it's limit. <br>
</font>
</i>
<hr width = 100%>
##Classes
<hr width = 100%>
<h5 id = "MnsLogViewer TARGET"></h5>
###MnsLogViewer [Class]
<font color = #5f5f5f size = 3pt>
<i>
Main UI class <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>MnsLogViewer(<b>parent</b>(<i>str</i>) ; [default: mnsUIUtils.get_maya_window()])</td></tr>
<tr><td><b><font color = #4caf50>Inherits from:  </font></b></td><td>form_class, base_class</td></tr>
<tr><td><b><font color = #4caf50>Class Members:  </font></b></td>
<td><ul>
<ul>
<li>currentOpenedWidgetIndex</li>
<li>thread</li>
<li>threadLock</li>
<li>currentProject</li>
<li>selfDir</li>
<li>iconsDir</li>
<li>allDirs</li>
<li>openedLog</li>
<li>absPathesLib</li>
<li>markedItems</li>
<li>svrList</li>
<li>itemList</li>
<li>currentLineCount</li>
<li>timeStart</li>
<li>timeEnd</li>
<li>dateStart</li>
<li>dateEnd</li>
<li>startDateTime</li>
<li>endDateTime</li>
<li>timeDateList</li>
</ul>
</td></tr>
<tr><td><b><font color = #4caf50>Methods:  </font></b></td><td><ul>
<li><b><a href="#scrollFlagDownTARGET">scrollFlagDown </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#scrollFlagUpTARGET">scrollFlagUp </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#collapseFolderTARGET">collapseFolder </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#expandFolderTARGET">expandFolder </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#findTopLevelItemForChildTARGET">findTopLevelItemForChild </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getDateTimeFromLineTARGET">getDateTimeFromLine </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#resetTimeSlidersTARGET">resetTimeSliders </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadWindowTARGET">loadWindow </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setItemHiddenTARGET">setItemHidden </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#clearAllFlagsTARGET">clearAllFlags </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#clearSearchTARGET">clearSearch </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#clearLogViewTARGET">clearLogView </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#connectSignalsTARGET">connectSignals </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#clearLogTARGET">clearLog </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#clearLibLogsTARGET">clearLibLogs </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getParentItemForLogTARGET">getParentItemForLog </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#expandItemToMaxTARGET">expandItemToMax </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#extractTimeFromSliderValueTARGET">extractTimeFromSliderValue </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#extractValueFromTimeTARGET">extractValueFromTime </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#flagTARGET">flag </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getLibTARGET">getLib </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#createThreadTARGET">createThread </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#runThreadTARGET">runThread </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#load_logStructTARGET">load_logStruct </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadLibsTARGET">loadLibs </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadLibTARGET">loadLib </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#updateViewTARGET">updateView </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#markFlaggedViewOnlyTARGET">markFlaggedViewOnly </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#matchEndDteToSliderTARGET">matchEndDteToSlider </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#matchEndSliderToDteTARGET">matchEndSliderToDte </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#matchStartDteToSliderTARGET">matchStartDteToSlider </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#matchStartSliderToDteTARGET">matchStartSliderToDte </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadLogTARGET">loadLog </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#readLogTARGET">readLog </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#refreshLogTARGET">refreshLog </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#reloadLibTARGET">reloadLib </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#remove_logStructTARGET">remove_logStruct </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#removeLibTARGET">removeLib </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#openMenuTARGET">openMenu </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#searchCurrentTARGET">searchCurrent </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#uncheckAllSvrTARGET">uncheckAllSvr </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#checkAllSvrTARGET">checkAllSvr </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getFileNumLinesTARGET">getFileNumLines </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#toggleThreadTARGET">toggleThread </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#updateCommentTARGET">updateComment </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#updateLineEditCommentTARGET">updateLineEditComment </b></a> <font size = 2pt><i>[method]</i></font></li>
</ul>
</td>
</tr>
</table></font>
####MnsLogViewer  methods
<hr width = 50%>
<h5 id = "scrollFlagDownTARGET"></h5><font color = 464646 size = 3><b>scrollFlagDown <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>scrollFlagDown(self) </td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "scrollFlagUpTARGET"></h5><font color = 464646 size = 3><b>scrollFlagUp <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>scrollFlagUp(self) </td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "collapseFolderTARGET"></h5><font color = 464646 size = 3><b>collapseFolder <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>collapseFolder(self, QTreeWidgetItem)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>QTreeWidgetItem</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "expandFolderTARGET"></h5><font color = 464646 size = 3><b>expandFolder <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>expandFolder(self, QTreeWidgetItem)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>QTreeWidgetItem</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "findTopLevelItemForChildTARGET"></h5><font color = 464646 size = 3><b>findTopLevelItemForChild <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>findTopLevelItemForChild(self, item)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>item</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getDateTimeFromLineTARGET"></h5><font color = 464646 size = 3><b>getDateTimeFromLine <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getDateTimeFromLine(self, line)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>line</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "resetTimeSlidersTARGET"></h5><font color = 464646 size = 3><b>resetTimeSliders <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>resetTimeSliders(self, qBtn = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>qBtn</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "loadWindowTARGET"></h5><font color = 464646 size = 3><b>loadWindow <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i> Main window load.</i><br>
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
<h5 id = "setItemHiddenTARGET"></h5><font color = 464646 size = 3><b>setItemHidden <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Aid method for filtering- set an inut QItem as hidden.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setItemHidden(self, item, hidden = False)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>item</b></li>
<li><b>hidden</b>(<i>bool</i>) ; [default: False]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "clearAllFlagsTARGET"></h5><font color = 464646 size = 3><b>clearAllFlags <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Clear all flags in the log file wrapper method trigger.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>clearAllFlags(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "clearSearchTARGET"></h5><font color = 464646 size = 3><b>clearSearch <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Clear search field method trigger.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>clearSearch(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "clearLogViewTARGET"></h5><font color = 464646 size = 3><b>clearLogView <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Clear the log view wrapper</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>clearLogView(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "connectSignalsTARGET"></h5><font color = 464646 size = 3><b>connectSignals <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Connect all the UI signals</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>connectSignals(self) </td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "clearLogTARGET"></h5><font color = 464646 size = 3><b>clearLog <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Delete a selected log file.</i><br>
<i>Prompt dialog confirm dependent.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>clearLog(self, item)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>item</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "clearLibLogsTARGET"></h5><font color = 464646 size = 3><b>clearLibLogs <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Delete all log files within the selected directory.</i><br>
<i>Prompt dialog confirm dependent.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>clearLibLogs(self, item)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>item</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getParentItemForLogTARGET"></h5><font color = 464646 size = 3><b>getParentItemForLog <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Depth view aid method.</i><br>
<i>On update request, for each item created find it's parent item based on current depth and previous depth.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getParentItemForLog(self, prevQTreeWidgetItem, currentDepth, lineCount)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>prevQTreeWidgetItem</b></li>
<li><b>currentDepth</b></li>
<li><b>lineCount</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "expandItemToMaxTARGET"></h5><font color = 464646 size = 3><b>expandItemToMax <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Expand a log directory item to max-level trigger method.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>expandItemToMax(self, topLevelItem)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>topLevelItem</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "extractTimeFromSliderValueTARGET"></h5><font color = 464646 size = 3><b>extractTimeFromSliderValue <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Extract time stemp formatt from a timeDate menu items method trigger.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>extractTimeFromSliderValue(self, value)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>value</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "extractValueFromTimeTARGET"></h5><font color = 464646 size = 3><b>extractValueFromTime <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Extract value from time wrapper.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>extractValueFromTime(self, time)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>time</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "flagTARGET"></h5><font color = 464646 size = 3><b>flag <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Flag method.</i><br>
<i>This method will flag/unflag a given log item file directly, then update the view.</i><br>
<i>Instead of flaggin the item in view only (session based), the flagging is being done directly in the log file as a custom parameter.</i><br>
<i>After the flag is made or cleared an 'update view' is being triggered to reload the view, flagging items if neccessary within the UI for user display.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>flag(self, item = None) </td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>item</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getLibTARGET"></h5><font color = 464646 size = 3><b>getLib <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Get a custom log directory method trigger</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getLib(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "createThreadTARGET"></h5><font color = 464646 size = 3><b>createThread <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Live update thread creation</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createThread(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "runThreadTARGET"></h5><font color = 464646 size = 3><b>runThread <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Live update thread run command</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>runThread(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "load_logStructTARGET"></h5><font color = 464646 size = 3><b>load_logStruct <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Load directory finction trigger.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>load_logStruct(self, startpath, tree)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>startpath</b></li>
<li><b>tree</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "loadLibsTARGET"></h5><font color = 464646 size = 3><b>loadLibs <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Load libraries wrapper</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadLibs(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "loadLibTARGET"></h5><font color = 464646 size = 3><b>loadLib <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Load library method trigger.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadLib(self, logsDir, tree)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>logsDir</b></li>
<li><b>tree</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "updateViewTARGET"></h5><font color = 464646 size = 3><b>updateView <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Log view update wrapper.</i><br>
<i>Update the log view depending on the UI state</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>updateView(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "markFlaggedViewOnlyTARGET"></h5><font color = 464646 size = 3><b>markFlaggedViewOnly <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Mark flag in view only when reading a file wrapper method trigger.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>markFlaggedViewOnly(self, item) </td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>item</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "matchEndDteToSliderTARGET"></h5><font color = 464646 size = 3><b>matchEndDteToSlider <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Match end calander widget to date-time slider method trigger.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>matchEndDteToSlider(self, value)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>value</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "matchEndSliderToDteTARGET"></h5><font color = 464646 size = 3><b>matchEndSliderToDte <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Match end time date slider to calander widget method trigger.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>matchEndSliderToDte(self, qDateTime)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>qDateTime</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "matchStartDteToSliderTARGET"></h5><font color = 464646 size = 3><b>matchStartDteToSlider <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Match start calander widget to date-time slider method trigger.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>matchStartDteToSlider(self, value)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>value</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "matchStartSliderToDteTARGET"></h5><font color = 464646 size = 3><b>matchStartSliderToDte <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Match start time date slider to calander widget method trigger.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>matchStartSliderToDte(self, qDateTime)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>qDateTime</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "loadLogTARGET"></h5><font color = 464646 size = 3><b>loadLog <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Read a log Item wrapper.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadLog(self, QTreeWidgetIndex)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>QTreeWidgetIndex</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "readLogTARGET"></h5><font color = 464646 size = 3><b>readLog <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Read a log file wrapper.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>readLog(self, logQTreeWidgetItem)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>logQTreeWidgetItem</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "refreshLogTARGET"></h5><font color = 464646 size = 3><b>refreshLog <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Refresh log wrapper.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>refreshLog(self, refreshNoChange)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>refreshNoChange</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "reloadLibTARGET"></h5><font color = 464646 size = 3><b>reloadLib <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Reload log library (directory) method trigger.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>reloadLib(self, item) </td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>item</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "remove_logStructTARGET"></h5><font color = 464646 size = 3><b>remove_logStruct <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Remove a log-tree struct from the log-files tree view</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>remove_logStruct(self, startpath)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>startpath</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "removeLibTARGET"></h5><font color = 464646 size = 3><b>removeLib <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Remove log library wrapper.</i><br>
<i>Remove from the UI view, delete the QItem as well as remove from the class instance class members list</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>removeLib(self, item)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>item</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "openMenuTARGET"></h5><font color = 464646 size = 3><b>openMenu <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Right click context menu command for the log-files tree view.</i><br>
</font>
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
<h5 id = "searchCurrentTARGET"></h5><font color = 464646 size = 3><b>searchCurrent <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Search current double clicked item method trigger.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>searchCurrent(self) </td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "uncheckAllSvrTARGET"></h5><font color = 464646 size = 3><b>uncheckAllSvr <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Set all severity check-box items to False wrapper.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>uncheckAllSvr(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "checkAllSvrTARGET"></h5><font color = 464646 size = 3><b>checkAllSvr <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Set all severity check-box items to True wrapper.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>checkAllSvr(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getFileNumLinesTARGET"></h5><font color = 464646 size = 3><b>getFileNumLines <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Simple file line count gather.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getFileNumLines(self, file)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>file</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "toggleThreadTARGET"></h5><font color = 464646 size = 3><b>toggleThread <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Thread lock toggle.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>toggleThread(self, state)</td></tr>
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
<h5 id = "updateCommentTARGET"></h5><font color = 464646 size = 3><b>updateComment <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Update log comment method trigger</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>updateComment(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "updateLineEditCommentTARGET"></h5><font color = 464646 size = 3><b>updateLineEditComment <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Update the LEdit widget depending on selected log item selected</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>updateLineEditComment(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
