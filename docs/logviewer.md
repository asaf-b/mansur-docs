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
<li>iconsDir</li>
<li>openedLog</li>
</ul>
</td></tr>
<tr><td><b><font color = #4caf50>Methods:  </font></b></td><td><ul>
<li><b><a href="#initViewTARGET">initView </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#collapseFolderTARGET">collapseFolder </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#expandFolderTARGET">expandFolder </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#validateItemToUIStateTARGET">validateItemToUIState </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#processLogLineTARGET">processLogLine </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#addFileItemTARGET">addFileItem </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#addFolderItemTARGET">addFolderItem </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadWindowTARGET">loadWindow </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#clearAllFlagsTARGET">clearAllFlags </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#clearSearchTARGET">clearSearch </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#connectSignalsTARGET">connectSignals </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#clearLogTARGET">clearLog </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#flagTARGET">flag </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadDirectoryLogsTARGET">loadDirectoryLogs </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadLibTARGET">loadLib </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#updateViewTARGET">updateView </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadLogTARGET">loadLog </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#openMenuTARGET">openMenu </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#searchCurrentTARGET">searchCurrent </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#uncheckAllSvrTARGET">uncheckAllSvr </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#checkAllSvrTARGET">checkAllSvr </b></a> <font size = 2pt><i>[method]</i></font></li>
</ul>
</td>
</tr>
</table></font>
####MnsLogViewer  methods
<hr width = 50%>
<h5 id = "initViewTARGET"></h5><font color = 464646 size = 3><b>initView <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>initView(self)</td></tr>
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
<h5 id = "validateItemToUIStateTARGET"></h5><font color = 464646 size = 3><b>validateItemToUIState <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>validateItemToUIState(self, item)</td></tr>
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
<h5 id = "processLogLineTARGET"></h5><font color = 464646 size = 3><b>processLogLine <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>processLogLine(self, line)</td></tr>
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
<h5 id = "addFileItemTARGET"></h5><font color = 464646 size = 3><b>addFileItem <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>addFileItem(self, parentItem, fullDirectory)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>parentItem</b></li>
<li><b>fullDirectory</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "addFolderItemTARGET"></h5><font color = 464646 size = 3><b>addFolderItem <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>addFolderItem(self, parentItem, fullDirectory)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>parentItem</b></li>
<li><b>fullDirectory</b></li>
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
<h5 id = "flagTARGET"></h5><font color = 464646 size = 3><b>flag <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Flag method.</i><br>
<i>This method will flag/unflag a given log item file directly, then update the view.</i><br>
<i>Instead of flaggin the item in view only (session based), the flagging is being done directly in the log file as a custom parameter.</i><br>
<i>After the flag is made or cleared an 'update view' is being triggered to reload the view, flagging items if neccessary within the UI for user display.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>flag(self, **kwargs) </td></tr>
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
<h5 id = "loadDirectoryLogsTARGET"></h5><font color = 464646 size = 3><b>loadDirectoryLogs <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Load directory finction trigger.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadDirectoryLogs(self, directory = None, parentItem = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>directory</b>(<i>str</i>) ; [default: None]</li>
<li><b>parentItem</b>(<i>str</i>) ; [default: None]</li>
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
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadLib(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
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
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>updateView(self, **kwargs)</td></tr>
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
<h5 id = "loadLogTARGET"></h5><font color = 464646 size = 3><b>loadLog <font size = 2pt> [<a href="#MnsLogViewer TARGET">MnsLogViewer </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Read a log file wrapper.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadLog(self, logQTreeWidgetItem)</td></tr>
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
