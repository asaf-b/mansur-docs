<body>
#characterDefenitionUI
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur === <br>
This tool was created to assist users in creating humanIK character definitions. <br>
Also, in conjunction with Block, create an animation puppet for predifined skeleton templates. <br>
Use pre-existing prests, as well as create your own presets, to characterize any skeleton in seconds. <br>
Many workflows and scenrios are covered within this tool, please refer to Mansur-Rig's You-Tube channel for a full video guide demonstratig all of them. <br>
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
<li><b><a href="#connectSignalsTARGET">connectSignals </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#createHIKSlotsMenuTARGET">createHIKSlotsMenu </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#drawDataTARGET">drawData </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#editMenuTARGET">editMenu </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#exportPresetTARGET">exportPreset </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#filterViewTARGET">filterView </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#gatherCharDefDataTARGET">gatherCharDefData </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getNamespaceBasedOnModeTARGET">getNamespaceBasedOnMode </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#importFromFileTARGET">importFromFile </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#importPresetTARGET">importPreset </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#initPresetsTARGET">initPresets </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#initViewTARGET">initView </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#initializeUITARGET">initializeUI </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#linkHikMenuActionTARGET">linkHikMenuAction </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadHikSlotToSelectedCellsTARGET">loadHikSlotToSelectedCells </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadNameSpaceTARGET">loadNameSpace </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadSelectedToCellTARGET">loadSelectedToCell </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadWindowTARGET">loadWindow </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#removeRowFromTableTARGET">removeRowFromTable </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#resetUITARGET">resetUI </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setNameBoxStateBasedOnModeTARGET">setNameBoxStateBasedOnMode </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#updateNameSpaceVarsTARGET">updateNameSpaceVars </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#updateSceneSelectionBasedOnUIStateTARGET">updateSceneSelectionBasedOnUIState </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#valueEditTARGET">valueEdit </b></a> <font size = 2pt><i>[method]</i></font></li>
</ul>
</td>
</tr>
</table></font>
####MnsCharacterDefenitionUI  methods
<hr width = 50%>
<h5 id = "addRowToTableTARGET"></h5><font color = 464646 size = 3><b>addRowToTable <font size = 2pt> [<a href="#MnsCharacterDefenitionUI TARGET">MnsCharacterDefenitionUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Add a new empty row trigger.</i><br>
</font>
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
<font size = 2pt color= 595959><br>
<i>Clear cell trigger.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>clearCell(self, position)</td></tr>
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
<h5 id = "clearRowTARGET"></h5><font color = 464646 size = 3><b>clearRow <font size = 2pt> [<a href="#MnsCharacterDefenitionUI TARGET">MnsCharacterDefenitionUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Delete Row trigger.</i><br>
</font>
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
<h5 id = "createHIKSlotsMenuTARGET"></h5><font color = 464646 size = 3><b>createHIKSlotsMenu <font size = 2pt> [<a href="#MnsCharacterDefenitionUI TARGET">MnsCharacterDefenitionUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Create the predifined HIK context menu structure.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createHIKSlotsMenu(self, rootMenuItem, position)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>rootMenuItem</b></li>
<li><b>position</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "drawDataTARGET"></h5><font color = 464646 size = 3><b>drawData <font size = 2pt> [<a href="#MnsCharacterDefenitionUI TARGET">MnsCharacterDefenitionUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Draw gathered data into the UI.</i><br>
</font>
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
<h5 id = "editMenuTARGET"></h5><font color = 464646 size = 3><b>editMenu <font size = 2pt> [<a href="#MnsCharacterDefenitionUI TARGET">MnsCharacterDefenitionUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Right-Click/Context Menu open trigger.</i><br>
<i>Create a menu based on the right click position and column, and connect all actions to their related triggers.</i><br>
</font>
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
<h5 id = "exportPresetTARGET"></h5><font color = 464646 size = 3><b>exportPreset <font size = 2pt> [<a href="#MnsCharacterDefenitionUI TARGET">MnsCharacterDefenitionUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Export preset to file trigger.</i><br>
</font>
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
<font size = 2pt color= 595959><br>
<i>Search trigger. Filter the main treeWidget list based on the input filter text.</i><br>
</font>
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
<font size = 2pt color= 595959><br>
<i>Gather character definition data from UI into a python dict.</i><br>
</font>
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
<h5 id = "getNamespaceBasedOnModeTARGET"></h5><font color = 464646 size = 3><b>getNamespaceBasedOnMode <font size = 2pt> [<a href="#MnsCharacterDefenitionUI TARGET">MnsCharacterDefenitionUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Get relevant namespace inpit based on mode.</i><br>
<i>mode 0 = Block name-space</i><br>
<i>mode 1 = Target name-space.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getNamespaceBasedOnMode(self, mode = 0)</td></tr>
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
<h5 id = "importFromFileTARGET"></h5><font color = 464646 size = 3><b>importFromFile <font size = 2pt> [<a href="#MnsCharacterDefenitionUI TARGET">MnsCharacterDefenitionUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Import preset from file trigger.</i><br>
</font>
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
<h5 id = "importPresetTARGET"></h5><font color = 464646 size = 3><b>importPreset <font size = 2pt> [<a href="#MnsCharacterDefenitionUI TARGET">MnsCharacterDefenitionUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Import preset trigger.</i><br>
</font>
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
<h5 id = "initPresetsTARGET"></h5><font color = 464646 size = 3><b>initPresets <font size = 2pt> [<a href="#MnsCharacterDefenitionUI TARGET">MnsCharacterDefenitionUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Initialize existing Mansur-Rig presets that are delivered with the product and update the UI list.</i><br>
</font>
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
<font size = 2pt color= 595959><br>
<i>Initialize UI default display state.</i><br>
</font>
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
<font size = 2pt color= 595959><br>
<i>Initialize UI Data.</i><br>
</font>
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
<h5 id = "linkHikMenuActionTARGET"></h5><font color = 464646 size = 3><b>linkHikMenuAction <font size = 2pt> [<a href="#MnsCharacterDefenitionUI TARGET">MnsCharacterDefenitionUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Procedural menu items action linking to action.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>linkHikMenuAction(self, menuItem, position)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>menuItem</b></li>
<li><b>position</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "loadHikSlotToSelectedCellsTARGET"></h5><font color = 464646 size = 3><b>loadHikSlotToSelectedCells <font size = 2pt> [<a href="#MnsCharacterDefenitionUI TARGET">MnsCharacterDefenitionUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Load selected HIK slot into selected cell trigger.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadHikSlotToSelectedCells(self, text, position)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>text</b></li>
<li><b>position</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "loadNameSpaceTARGET"></h5><font color = 464646 size = 3><b>loadNameSpace <font size = 2pt> [<a href="#MnsCharacterDefenitionUI TARGET">MnsCharacterDefenitionUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Load selected namespace trigger.</i><br>
</font>
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
<font size = 2pt color= 595959><br>
<i>Load scene selection to cell trigger.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadSelectedToCell(self, position)</td></tr>
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
<h5 id = "removeRowFromTableTARGET"></h5><font color = 464646 size = 3><b>removeRowFromTable <font size = 2pt> [<a href="#MnsCharacterDefenitionUI TARGET">MnsCharacterDefenitionUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Remove Row trigger.</i><br>
</font>
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
<font size = 2pt color= 595959><br>
<i>Reset the UI to default state.</i><br>
</font>
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
<h5 id = "setNameBoxStateBasedOnModeTARGET"></h5><font color = 464646 size = 3><b>setNameBoxStateBasedOnMode <font size = 2pt> [<a href="#MnsCharacterDefenitionUI TARGET">MnsCharacterDefenitionUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>set the character name line-edit state base on the current UI state.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setNameBoxStateBasedOnMode(self)</td></tr>
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
<font size = 2pt color= 595959><br>
<i>Update the class member variables for both namespaces.</i><br>
</font>
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
<h5 id = "updateSceneSelectionBasedOnUIStateTARGET"></h5><font color = 464646 size = 3><b>updateSceneSelectionBasedOnUIState <font size = 2pt> [<a href="#MnsCharacterDefenitionUI TARGET">MnsCharacterDefenitionUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Update the current Maya scene selection based on the selected items in the UI.</i><br>
<i>In case the "update selection" checkbox isn't checked, this will not execute and selection will not be updated.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>updateSceneSelectionBasedOnUIState(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "valueEditTARGET"></h5><font color = 464646 size = 3><b>valueEdit <font size = 2pt> [<a href="#MnsCharacterDefenitionUI TARGET">MnsCharacterDefenitionUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>TreeWidget Edit trigger</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>valueEdit(self, item, column)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>item</b></li>
<li><b>column</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
##Defenitions
<hr width = 100%>
###loadCharacterDefenitionUI
<font color = #5f5f5f size = 3pt>
<i>
Load the Charecter Definition UI from globals, avoid UI duplication. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadCharacterDefenitionUI()</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
