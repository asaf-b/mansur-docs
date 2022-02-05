<body>
#modulePresetEditor
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur === <br>
This tool was designed to manage module presets. <br>
As Mansur-Rig modules comatin many attrbiutes, it is sometimes more convenient to use a predefined preset to speed up the wrokflow. <br>
Mansur-Rig includes some module presets, although this was designed mainly to allow usesrs to create their own presets, essentially saving the module settings' state. <br>
 <br>
</font>
</i>
<hr width = 100%>
##Classes
<hr width = 100%>
<h5 id = "ExportPresetDialog TARGET"></h5>
###ExportPresetDialog [Class]
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>ExportPresetDialog(<b>parent</b>(<i>str</i>) ; [default: None])</td></tr>
<tr><td><b><font color = #4caf50>Inherits from:  </font></b></td><td>QtWidgets.QDialog</td></tr>
<tr><td><b><font color = #4caf50>Class Members:  </font></b></td>
<td><ul>
<ul>
<li>buttonBox</li>
<li>layout</li>
<li>author_le</li>
<li>description_te</li>
</ul>
</td></tr>
<tr><td><b><font color = #4caf50>Methods:  </font></b></td><td><ul>
<li><b><a href="#getInfoTARGET">getInfo </b></a> <font size = 2pt><i>[method]</i></font></li>
</ul>
</td>
</tr>
</table></font>
####ExportPresetDialog  methods
<hr width = 50%>
<h5 id = "getInfoTARGET"></h5><font color = 464646 size = 3><b>getInfo <font size = 2pt> [<a href="#ExportPresetDialog TARGET">ExportPresetDialog </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getInfo(self)</td></tr>
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
<h5 id = "MnsModulePresetEditor TARGET"></h5>
###MnsModulePresetEditor [Class]
<font color = #5f5f5f size = 3pt>
<i>
Module preset Tool UI Class. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>MnsModulePresetEditor(<b>parent</b>(<i>str</i>) ; [default: mnsUIUtils.get_maya_window()])</td></tr>
<tr><td><b><font color = #4caf50>Inherits from:  </font></b></td><td>form_class, base_class</td></tr>
<tr><td><b><font color = #4caf50>Class Members:  </font></b></td>
<td><ul>
<ul>
<li>iconsDir</li>
<li>rigTop</li>
<li>mnsModulePresetsDir</li>
<li>settingsWindowDynUI</li>
<li>moduleType</li>
<li>presetsDict</li>
<li>currentPreset</li>
</ul>
</td></tr>
<tr><td><b><font color = #4caf50>Methods:  </font></b></td><td><ul>
<li><b><a href="#loadPresetTARGET">loadPreset </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#connectSignalsTARGET">connectSignals </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#exportPresetTARGET">exportPreset </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#readCurrentModuleValuesTARGET">readCurrentModuleValues </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#importPresetTARGET">importPreset </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#gatherAdditionalModulePresetsPathsTARGET">gatherAdditionalModulePresetsPaths </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#initlizeUITARGET">initlizeUI </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#readPresetFileTARGET">readPresetFile </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#readPresetTARGET">readPreset </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadWindowTARGET">loadWindow </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#initializeViewTARGET">initializeView </b></a> <font size = 2pt><i>[method]</i></font></li>
</ul>
</td>
</tr>
</table></font>
####MnsModulePresetEditor  methods
<hr width = 50%>
<h5 id = "loadPresetTARGET"></h5><font color = 464646 size = 3><b>loadPreset <font size = 2pt> [<a href="#MnsModulePresetEditor TARGET">MnsModulePresetEditor </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Apply the selected preset onto the settings window</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadPreset(self, **kwargs)</td></tr>
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
<h5 id = "connectSignalsTARGET"></h5><font color = 464646 size = 3><b>connectSignals <font size = 2pt> [<a href="#MnsModulePresetEditor TARGET">MnsModulePresetEditor </a> class method] </font></font></b>
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
<h5 id = "exportPresetTARGET"></h5><font color = 464646 size = 3><b>exportPreset <font size = 2pt> [<a href="#MnsModulePresetEditor TARGET">MnsModulePresetEditor </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Export current settings window state as a preset.</i><br>
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
<h5 id = "readCurrentModuleValuesTARGET"></h5><font color = 464646 size = 3><b>readCurrentModuleValues <font size = 2pt> [<a href="#MnsModulePresetEditor TARGET">MnsModulePresetEditor </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>From the current preset, read the current UI state.</i><br>
<i>This method will return a formatted data assembly of all values and fields within the module-settings tab</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>readCurrentModuleValues(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "importPresetTARGET"></h5><font color = 464646 size = 3><b>importPreset <font size = 2pt> [<a href="#MnsModulePresetEditor TARGET">MnsModulePresetEditor </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Import a preset from file</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>importPreset(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "gatherAdditionalModulePresetsPathsTARGET"></h5><font color = 464646 size = 3><b>gatherAdditionalModulePresetsPaths <font size = 2pt> [<a href="#MnsModulePresetEditor TARGET">MnsModulePresetEditor </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Initialize any custom module presets paths that already exist within the data collect json.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>gatherAdditionalModulePresetsPaths(self, **kwargs)</td></tr>
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
<h5 id = "initlizeUITARGET"></h5><font color = 464646 size = 3><b>initlizeUI <font size = 2pt> [<a href="#MnsModulePresetEditor TARGET">MnsModulePresetEditor </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Initialize the UI display</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>initlizeUI(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "readPresetFileTARGET"></h5><font color = 464646 size = 3><b>readPresetFile <font size = 2pt> [<a href="#MnsModulePresetEditor TARGET">MnsModulePresetEditor </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Read a preset from the selected file input</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>readPresetFile(self, filePath = "")</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>filePath</b>(<i>str</i>) ; [default: ""]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "readPresetTARGET"></h5><font color = 464646 size = 3><b>readPreset <font size = 2pt> [<a href="#MnsModulePresetEditor TARGET">MnsModulePresetEditor </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Read the curretly selected preset</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>readPreset(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "loadWindowTARGET"></h5><font color = 464646 size = 3><b>loadWindow <font size = 2pt> [<a href="#MnsModulePresetEditor TARGET">MnsModulePresetEditor </a> class method] </font></font></b>
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
<h5 id = "initializeViewTARGET"></h5><font color = 464646 size = 3><b>initializeView <font size = 2pt> [<a href="#MnsModulePresetEditor TARGET">MnsModulePresetEditor </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>initialize data into the UI</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>initializeView(self, selection = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>selection</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
##Defenitions
<hr width = 100%>
###loadModulePresetEditor
<font color = #5f5f5f size = 3pt>
<i>
Load the module preset window, avoid UI duplication. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadModulePresetEditor(parent=mnsUIUtils.get_maya_window()) </td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>parent</b>(<i>str</i>) ; [default: mnsUIUtils.get_maya_window()]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
