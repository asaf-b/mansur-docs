<body>
#preferences
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur === <br>
A Simple global UI class to handle global setting within the package. <br>
All global changeable variables should be inserted into this UI. <br>
Handeling is semi-procedural, drawing and retreiving all setting procedurally, although the implementation will look for specific widget names to handle the settings. <br>
"restore factory defaults" is also contained within this UI, actual implementation is within mnsUtils. <br>
 <br>
</font>
</i>
<hr width = 100%>
##Classes
<hr width = 100%>
<h5 id = "MnsPreferences TARGET"></h5>
###MnsPreferences [Class]
<font color = #5f5f5f size = 3pt>
<i>
Main UI class <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>MnsPreferences(<b>parent</b>(<i>str</i>) ; [default: mnsUIUtils.get_maya_window()])</td></tr>
<tr><td><b><font color = #4caf50>Inherits from:  </font></b></td><td>form_class, base_class</td></tr>
<tr><td><b><font color = #4caf50>Class Members:  </font></b></td>
<td><ul>
<ul>
<li>currentPrefs</li>
</ul>
</td></tr>
<tr><td><b><font color = #4caf50>Methods:  </font></b></td><td><ul>
<li><b><a href="#connectSignalsTARGET">connectSignals </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#initViewTARGET">initView </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadCategoryPrefsTARGET">loadCategoryPrefs </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadPathTARGET">loadPath </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadWindowTARGET">loadWindow </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#restoreDefaultsTARGET">restoreDefaults </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#saveSettingTARGET">saveSetting </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#updateColorValueTARGET">updateColorValue </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#updateLineEditValueTARGET">updateLineEditValue </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#updateValueTARGET">updateValue </b></a> <font size = 2pt><i>[method]</i></font></li>
</ul>
</td>
</tr>
</table></font>
####MnsPreferences  methods
<hr width = 50%>
<h5 id = "connectSignalsTARGET"></h5><font color = 464646 size = 3><b>connectSignals <font size = 2pt> [<a href="#MnsPreferences TARGET">MnsPreferences </a> class method] </font></font></b>
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
<h5 id = "initViewTARGET"></h5><font color = 464646 size = 3><b>initView <font size = 2pt> [<a href="#MnsPreferences TARGET">MnsPreferences </a> class method] </font></font></b>
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
<h5 id = "loadCategoryPrefsTARGET"></h5><font color = 464646 size = 3><b>loadCategoryPrefs <font size = 2pt> [<a href="#MnsPreferences TARGET">MnsPreferences </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadCategoryPrefs(self, currentItem, previousItem)</td></tr>
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
<h5 id = "loadPathTARGET"></h5><font color = 464646 size = 3><b>loadPath <font size = 2pt> [<a href="#MnsPreferences TARGET">MnsPreferences </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadPath(self, lineEditWidget)</td></tr>
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
<h5 id = "loadWindowTARGET"></h5><font color = 464646 size = 3><b>loadWindow <font size = 2pt> [<a href="#MnsPreferences TARGET">MnsPreferences </a> class method] </font></font></b>
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
<h5 id = "restoreDefaultsTARGET"></h5><font color = 464646 size = 3><b>restoreDefaults <font size = 2pt> [<a href="#MnsPreferences TARGET">MnsPreferences </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>restoreDefaults(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "saveSettingTARGET"></h5><font color = 464646 size = 3><b>saveSetting <font size = 2pt> [<a href="#MnsPreferences TARGET">MnsPreferences </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>saveSetting(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "updateColorValueTARGET"></h5><font color = 464646 size = 3><b>updateColorValue <font size = 2pt> [<a href="#MnsPreferences TARGET">MnsPreferences </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>updateColorValue(self, colBtn, settingCat, setting)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>colBtn</b></li>
<li><b>settingCat</b></li>
<li><b>setting</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "updateLineEditValueTARGET"></h5><font color = 464646 size = 3><b>updateLineEditValue <font size = 2pt> [<a href="#MnsPreferences TARGET">MnsPreferences </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>updateLineEditValue(self, setWid, settingCat, setting, text)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>setWid</b></li>
<li><b>settingCat</b></li>
<li><b>setting</b></li>
<li><b>text</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "updateValueTARGET"></h5><font color = 464646 size = 3><b>updateValue <font size = 2pt> [<a href="#MnsPreferences TARGET">MnsPreferences </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>updateValue(self, settingCat, setting, setWid, dummyA = None, dummyB = None, dummyC = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>settingCat</b></li>
<li><b>setting</b></li>
<li><b>setWid</b></li>
<li><b>dummyA</b>(<i>str</i>) ; [default: None]</li>
<li><b>dummyB</b>(<i>str</i>) ; [default: None]</li>
<li><b>dummyC</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
##Defenitions
<hr width = 100%>
###loadPreferences
<font color = #5f5f5f size = 3pt>
<i>
Load the Preferences UI from globals, avoid UI duplication. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadPreferences()</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
