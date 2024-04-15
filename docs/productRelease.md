<body>
#productRelease
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
<h5 id = "MnsProductRelease TARGET"></h5>
###MnsProductRelease [Class]
<font color = #5f5f5f size = 3pt>
<i>
Main UI class <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>MnsProductRelease(<b>parent</b>(<i>str</i>) ; [default: mnsUIUtils.get_maya_window()])</td></tr>
<tr><td><b><font color = #4caf50>Inherits from:  </font></b></td><td>form_class, base_class</td></tr>
<tr><td><b><font color = #4caf50>Class Members:  </font></b></td>
<td><ul>
<ul>
<li>pluginReleaseDir</li>
<li>existingPluginVerLib</li>
<li>releaseRootDir</li>
<li>existingProductVerLib</li>
<li>latestVerList</li>
<li>releaseExclustions</li>
</ul>
</td></tr>
<tr><td><b><font color = #4caf50>Methods:  </font></b></td><td><ul>
<li><b><a href="#connectSignalsTARGET">connectSignals </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#createCopyrightHeaderInPythonFileTARGET">createCopyrightHeaderInPythonFile </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#gatherExistingPluginVersionsTARGET">gatherExistingPluginVersions </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#gatherExistingProductVersionsTARGET">gatherExistingProductVersions </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getNextReleaseVersionTARGET">getNextReleaseVersion </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadWindowTARGET">loadWindow </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#releaseVersionTARGET">releaseVersion </b></a> <font size = 2pt><i>[method]</i></font></li>
</ul>
</td>
</tr>
</table></font>
####MnsProductRelease  methods
<hr width = 50%>
<h5 id = "connectSignalsTARGET"></h5><font color = 464646 size = 3><b>connectSignals <font size = 2pt> [<a href="#MnsProductRelease TARGET">MnsProductRelease </a> class method] </font></font></b>
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
<h5 id = "createCopyrightHeaderInPythonFileTARGET"></h5><font color = 464646 size = 3><b>createCopyrightHeaderInPythonFile <font size = 2pt> [<a href="#MnsProductRelease TARGET">MnsProductRelease </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createCopyrightHeaderInPythonFile(self, filePath = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>filePath</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "gatherExistingPluginVersionsTARGET"></h5><font color = 464646 size = 3><b>gatherExistingPluginVersions <font size = 2pt> [<a href="#MnsProductRelease TARGET">MnsProductRelease </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>gatherExistingPluginVersions(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "gatherExistingProductVersionsTARGET"></h5><font color = 464646 size = 3><b>gatherExistingProductVersions <font size = 2pt> [<a href="#MnsProductRelease TARGET">MnsProductRelease </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>gatherExistingProductVersions(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getNextReleaseVersionTARGET"></h5><font color = 464646 size = 3><b>getNextReleaseVersion <font size = 2pt> [<a href="#MnsProductRelease TARGET">MnsProductRelease </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getNextReleaseVersion(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "loadWindowTARGET"></h5><font color = 464646 size = 3><b>loadWindow <font size = 2pt> [<a href="#MnsProductRelease TARGET">MnsProductRelease </a> class method] </font></font></b>
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
<h5 id = "releaseVersionTARGET"></h5><font color = 464646 size = 3><b>releaseVersion <font size = 2pt> [<a href="#MnsProductRelease TARGET">MnsProductRelease </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>releaseVersion(self)</td></tr>
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
###loadProductRelease
<font color = #5f5f5f size = 3pt>
<i>
Load the Log Viewer UI from globals, avoid UI duplication. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadProductRelease()</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
