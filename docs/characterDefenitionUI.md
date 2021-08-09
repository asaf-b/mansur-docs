<body>
#characterDefenitionUI
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
<h5 id = "MnsCharacterDefenitionUI TARGET"></h5>
###MnsCharacterDefenitionUI [Class]
<font color = #5f5f5f size = 3pt>
<i>
Main UI Class <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>MnsCharacterDefenitionUI(<b>parent</b>(<i>str</i>) ; [default: mnsUIUtils.get_maya_window()])</td></tr>
<tr><td><b><font color = #4caf50>Inherits from:  </font></b></td><td>form_class, base_class</td></tr>
<tr><td><b><font color = #4caf50>Class Members:  </font></b></td>
<td><ul>
<ul>
<li>presetsDir</li>
<li>charDefPresets</li>
<li>charDefData</li>
<li>blockNameSpace</li>
<li>targetNameSpace</li>
</ul>
</td></tr>
<tr><td><b><font color = #4caf50>Methods:  </font></b></td><td><ul>
<li><b><a href="#addRowToTableTARGET">addRowToTable </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#clearCellTARGET">clearCell </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#clearRowTARGET">clearRow </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#drawDataTARGET">drawData </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#exportPresetTARGET">exportPreset </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#filterViewTARGET">filterView </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#gatherCharDefDataTARGET">gatherCharDefData </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#importFromFileTARGET">importFromFile </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#initPresetsTARGET">initPresets </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#initViewTARGET">initView </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#initializeUITARGET">initializeUI </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadNameSpaceTARGET">loadNameSpace </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadSelectedToCellTARGET">loadSelectedToCell </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#removeRowFromTableTARGET">removeRowFromTable </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#resetUITARGET">resetUI </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#updateNameSpaceVarsTARGET">updateNameSpaceVars </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#importPresetTARGET">importPreset </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#linkHikMenuActionTARGET">linkHikMenuAction </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#editMenuTARGET">editMenu </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#createHIKSlotsMenuTARGET">createHIKSlotsMenu </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadHikSlotToSelectedCellsTARGET">loadHikSlotToSelectedCells </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#connectSignalsTARGET">connectSignals </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadWindowTARGET">loadWindow </b></a> <font size = 2pt><i>[method]</i></font></li>
</ul>
</td>
</tr>
</table></font>
####MnsCharacterDefenitionUI  methods
<hr width = 50%>
<h5 id = "addRowToTableTARGET"></h5><font color = 464646 size = 3><b>addRowToTable <font size = 2pt> [<a href="#MnsCharacterDefenitionUI TARGET">MnsCharacterDefenitionUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>addRowToTable(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "clearCellTARGET"></h5><font color = 464646 size = 3><b>clearCell <font size = 2pt> [<a href="#MnsCharacterDefenitionUI TARGET">MnsCharacterDefenitionUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>clearCell(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "clearRowTARGET"></h5><font color = 464646 size = 3><b>clearRow <font size = 2pt> [<a href="#MnsCharacterDefenitionUI TARGET">MnsCharacterDefenitionUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>clearRow(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "drawDataTARGET"></h5><font color = 464646 size = 3><b>drawData <font size = 2pt> [<a href="#MnsCharacterDefenitionUI TARGET">MnsCharacterDefenitionUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>drawData(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "exportPresetTARGET"></h5><font color = 464646 size = 3><b>exportPreset <font size = 2pt> [<a href="#MnsCharacterDefenitionUI TARGET">MnsCharacterDefenitionUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>exportPreset(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "filterViewTARGET"></h5><font color = 464646 size = 3><b>filterView <font size = 2pt> [<a href="#MnsCharacterDefenitionUI TARGET">MnsCharacterDefenitionUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>filterView(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "gatherCharDefDataTARGET"></h5><font color = 464646 size = 3><b>gatherCharDefData <font size = 2pt> [<a href="#MnsCharacterDefenitionUI TARGET">MnsCharacterDefenitionUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>gatherCharDefData(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "importFromFileTARGET"></h5><font color = 464646 size = 3><b>importFromFile <font size = 2pt> [<a href="#MnsCharacterDefenitionUI TARGET">MnsCharacterDefenitionUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>importFromFile(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "initPresetsTARGET"></h5><font color = 464646 size = 3><b>initPresets <font size = 2pt> [<a href="#MnsCharacterDefenitionUI TARGET">MnsCharacterDefenitionUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>initPresets(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "initViewTARGET"></h5><font color = 464646 size = 3><b>initView <font size = 2pt> [<a href="#MnsCharacterDefenitionUI TARGET">MnsCharacterDefenitionUI </a> class method] </font></font></b>
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
<h5 id = "initializeUITARGET"></h5><font color = 464646 size = 3><b>initializeUI <font size = 2pt> [<a href="#MnsCharacterDefenitionUI TARGET">MnsCharacterDefenitionUI </a> class method] </font></font></b>
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
<h5 id = "loadNameSpaceTARGET"></h5><font color = 464646 size = 3><b>loadNameSpace <font size = 2pt> [<a href="#MnsCharacterDefenitionUI TARGET">MnsCharacterDefenitionUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadNameSpace(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "loadSelectedToCellTARGET"></h5><font color = 464646 size = 3><b>loadSelectedToCell <font size = 2pt> [<a href="#MnsCharacterDefenitionUI TARGET">MnsCharacterDefenitionUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadSelectedToCell(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "removeRowFromTableTARGET"></h5><font color = 464646 size = 3><b>removeRowFromTable <font size = 2pt> [<a href="#MnsCharacterDefenitionUI TARGET">MnsCharacterDefenitionUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>removeRowFromTable(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "resetUITARGET"></h5><font color = 464646 size = 3><b>resetUI <font size = 2pt> [<a href="#MnsCharacterDefenitionUI TARGET">MnsCharacterDefenitionUI </a> class method] </font></font></b>
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
<h5 id = "updateNameSpaceVarsTARGET"></h5><font color = 464646 size = 3><b>updateNameSpaceVars <font size = 2pt> [<a href="#MnsCharacterDefenitionUI TARGET">MnsCharacterDefenitionUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>updateNameSpaceVars(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "importPresetTARGET"></h5><font color = 464646 size = 3><b>importPreset <font size = 2pt> [<a href="#MnsCharacterDefenitionUI TARGET">MnsCharacterDefenitionUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>importPreset(self, **kwargs)</td></tr>
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
<h5 id = "linkHikMenuActionTARGET"></h5><font color = 464646 size = 3><b>linkHikMenuAction <font size = 2pt> [<a href="#MnsCharacterDefenitionUI TARGET">MnsCharacterDefenitionUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>linkHikMenuAction(self, menuItem)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>menuItem</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "editMenuTARGET"></h5><font color = 464646 size = 3><b>editMenu <font size = 2pt> [<a href="#MnsCharacterDefenitionUI TARGET">MnsCharacterDefenitionUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>editMenu(self, position)</td></tr>
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
<h5 id = "createHIKSlotsMenuTARGET"></h5><font color = 464646 size = 3><b>createHIKSlotsMenu <font size = 2pt> [<a href="#MnsCharacterDefenitionUI TARGET">MnsCharacterDefenitionUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createHIKSlotsMenu(self, rootMenuItem = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>rootMenuItem</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "loadHikSlotToSelectedCellsTARGET"></h5><font color = 464646 size = 3><b>loadHikSlotToSelectedCells <font size = 2pt> [<a href="#MnsCharacterDefenitionUI TARGET">MnsCharacterDefenitionUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadHikSlotToSelectedCells(self, text = "")</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>text</b>(<i>str</i>) ; [default: ""]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "connectSignalsTARGET"></h5><font color = 464646 size = 3><b>connectSignals <font size = 2pt> [<a href="#MnsCharacterDefenitionUI TARGET">MnsCharacterDefenitionUI </a> class method] </font></font></b>
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
<h5 id = "loadWindowTARGET"></h5><font color = 464646 size = 3><b>loadWindow <font size = 2pt> [<a href="#MnsCharacterDefenitionUI TARGET">MnsCharacterDefenitionUI </a> class method] </font></font></b>
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
