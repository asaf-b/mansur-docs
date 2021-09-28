<body>
#pluginRelease
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
PluginRelease UI Class. <br>
=== Author: Assaf Ben Zur === <br>
This admin util is used to procedurally release the mnsPlugins library and version control it. <br>
The UI will find c++ projects based on a directory (which can be changed), and will allow the user (admin) to add it to the next build. <br>
On top of that, the UI will find the latest released version and extract the existing library within it, and update the release colums accordingly. <br>
In case a plugin build exists in the latest version, but it's build project isn't available, the plugin will add to the release option with a flag "[version]"- <br>
This means that the plugin can only be copied from the version selected to the next release- it cannot bild. <br>
Of course this behaviour means that the internal version of the plugin will not change (expected behaviour) to inform the user of the ACTUAL plugin version. <br>
 <br>
This Tool is meant to BUILD the project on each release as opposed to getting a copy of n .mll file. <br>
This means that the VS project will have to be maintained (expected) in order to be released- hence keeping up to date with maya's releases. <br>
 <br>
The tool contains a version release choice between patch/minor/major and none. <br>
All mnsReleases, including this tool will mark a version with a suffix of the path version . a dateTime stamp. <br>
 <br>
This tool also includes a maya version choice for release which will access a different build configuration within the VS project. <br>
The tool accesses the version parameter using a custom macro inserted into the VS project- which will be written with the user version choice- in order for the user to see the correct version when using the plugin-manager "info". <br>
 <br>
</font>
</i>
<hr width = 100%>
##Classes
<hr width = 100%>
<h5 id = "MnsPluginBuild TARGET"></h5>
###MnsPluginBuild [Class]
<font color = #5f5f5f size = 3pt>
<i>
MnsPluginBuild Class. A conviniency class. <br>
This class will contain eixsting plugin builds. <br>
Should contain a plugin name, directory, buildAvailable (bool), and a prevVerDirectory if a build is not available" <br>
Used to access information in a clean manner. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>MnsPluginBuild(<b>name</b>(<i>str</i>) ; [default: ""],<b>direct</b>(<i>str</i>) ; [default: ""],<b>buildAvailable</b>(<i>bool</i>) ; [default: False],<b>prevVerDirectory</b>(<i>str</i>) ; [default: ""])</td></tr>
<tr><td><b><font color = #4caf50>Inherits from:  </font></b></td><td>object</td></tr>
<tr><td><b><font color = #4caf50>Class Members:  </font></b></td>
<td><ul>
<ul>
<li>pluginName</li>
<li>pluginDirectory</li>
<li>buildAvailable</li>
<li>prevVerDirectory</li>
</ul>
</td></tr>
</tr>
</table></font>
<hr width = 100%>
<h5 id = "MnsPluginRelease TARGET"></h5>
###MnsPluginRelease [Class]
<font color = #5f5f5f size = 3pt>
<i>
pluginRelease UI class <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>MnsPluginRelease(<b>parent</b>(<i>str</i>) ; [default: mnsUIUtils.get_maya_window()])</td></tr>
<tr><td><b><font color = #4caf50>Inherits from:  </font></b></td><td>form_class, base_class</td></tr>
<tr><td><b><font color = #4caf50>Class Members:  </font></b></td>
<td><ul>
<ul>
<li>pluginBuilds</li>
<li>existingPluginNames</li>
<li>existingVersionsFoundNames</li>
<li>latestVersionPath</li>
</ul>
</td></tr>
<tr><td><b><font color = #4caf50>Methods:  </font></b></td><td><ul>
<li><b><a href="#getCMakeBaseDirTARGET">getCMakeBaseDir </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#buildPluginTARGET">buildPlugin </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#linux_mnsLicDigest_addExtraCMakeLinesTARGET">linux_mnsLicDigest_addExtraCMakeLines </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#selectDevDirTARGET">selectDevDir </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#selectRelDirTARGET">selectRelDir </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#connectSignalsTARGET">connectSignals </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getNewVerStringTARGET">getNewVerString </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getVersionsForBuildTARGET">getVersionsForBuild </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getLastestReleaseVerTARGET">getLastestReleaseVer </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#initExistingDirsTARGET">initExistingDirs </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#releasePluginVerTARGET">releasePluginVer </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#releasePluginVer_legacyTARGET">releasePluginVer_legacy </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadWindowTARGET">loadWindow </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#sortListsTARGET">sortLists </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#dirChangedTARGET">dirChanged </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#splitVerStringToListTARGET">splitVerStringToList </b></a> <font size = 2pt><i>[method]</i></font></li>
</ul>
</td>
</tr>
</table></font>
####MnsPluginRelease  methods
<hr width = 50%>
<h5 id = "getCMakeBaseDirTARGET"></h5><font color = 464646 size = 3><b>getCMakeBaseDir <font size = 2pt> [<a href="#MnsPluginRelease TARGET">MnsPluginRelease </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getCMakeBaseDir(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "buildPluginTARGET"></h5><font color = 464646 size = 3><b>buildPlugin <font size = 2pt> [<a href="#MnsPluginRelease TARGET">MnsPluginRelease </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>buildPlugin(self, MnsPluginBuild = None, cMakeDir = None, newVersionRootDir = None, plat = "win", versionString = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>MnsPluginBuild</b>(<i>str</i>) ; [default: None]</li>
<li><b>cMakeDir</b>(<i>str</i>) ; [default: None]</li>
<li><b>newVersionRootDir</b>(<i>str</i>) ; [default: None]</li>
<li><b>plat</b>(<i>str</i>) ; [default: "win"]</li>
<li><b>versionString</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "linux_mnsLicDigest_addExtraCMakeLinesTARGET"></h5><font color = 464646 size = 3><b>linux_mnsLicDigest_addExtraCMakeLines <font size = 2pt> [<a href="#MnsPluginRelease TARGET">MnsPluginRelease </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>linux_mnsLicDigest_addExtraCMakeLines(self, cmakeListsFile = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>cmakeListsFile</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "selectDevDirTARGET"></h5><font color = 464646 size = 3><b>selectDevDir <font size = 2pt> [<a href="#MnsPluginRelease TARGET">MnsPluginRelease </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Change dev directory trigger action.</i><br>
<i>Prompts a directory-select dialog for the user to change the dev directory.</i><br>
<i>A directory change will trigger a 'text-changed' signal emit.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>selectDevDir(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "selectRelDirTARGET"></h5><font color = 464646 size = 3><b>selectRelDir <font size = 2pt> [<a href="#MnsPluginRelease TARGET">MnsPluginRelease </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Change release directory trigger action.</i><br>
<i>Prompts a directory-select dialog for the user to change the release directory.</i><br>
<i>A directory change will trigger a 'text-changed' signal emit.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>selectRelDir(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "connectSignalsTARGET"></h5><font color = 464646 size = 3><b>connectSignals <font size = 2pt> [<a href="#MnsPluginRelease TARGET">MnsPluginRelease </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Connect all the UI signals</i><br>
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
<h5 id = "getNewVerStringTARGET"></h5><font color = 464646 size = 3><b>getNewVerString <font size = 2pt> [<a href="#MnsPluginRelease TARGET">MnsPluginRelease </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Get a new vesrtion string based on user version element upgrade. Return as a string.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getNewVerString(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td> string (new version id as string)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getVersionsForBuildTARGET"></h5><font color = 464646 size = 3><b>getVersionsForBuild <font size = 2pt> [<a href="#MnsPluginRelease TARGET">MnsPluginRelease </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Get all valid maya versions for the plugin build directory passed.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getVersionsForBuild(self, buildDir)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>list (compatibleVersions)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>buildDir</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getLastestReleaseVerTARGET"></h5><font color = 464646 size = 3><b>getLastestReleaseVer <font size = 2pt> [<a href="#MnsPluginRelease TARGET">MnsPluginRelease </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Get the latest version for the build directory</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getLastestReleaseVer(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "initExistingDirsTARGET"></h5><font color = 464646 size = 3><b>initExistingDirs <font size = 2pt> [<a href="#MnsPluginRelease TARGET">MnsPluginRelease </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Initialize existing directory.</i><br>
<i>Find all available builds for the selected directory.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>initExistingDirs(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "releasePluginVerTARGET"></h5><font color = 464646 size = 3><b>releasePluginVer <font size = 2pt> [<a href="#MnsPluginRelease TARGET">MnsPluginRelease </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Main version release button trigger.</i><br>
<i>Compiles all needed information based on user UI slections, and triggers a new version build.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>releasePluginVer(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "releasePluginVer_legacyTARGET"></h5><font color = 464646 size = 3><b>releasePluginVer_legacy <font size = 2pt> [<a href="#MnsPluginRelease TARGET">MnsPluginRelease </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Main version release button trigger.</i><br>
<i>Compiles all needed information based on user UI slections, and triggers a new version build.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>releasePluginVer_legacy(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "loadWindowTARGET"></h5><font color = 464646 size = 3><b>loadWindow <font size = 2pt> [<a href="#MnsPluginRelease TARGET">MnsPluginRelease </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Main window load</i><br>
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
<h5 id = "sortListsTARGET"></h5><font color = 464646 size = 3><b>sortLists <font size = 2pt> [<a href="#MnsPluginRelease TARGET">MnsPluginRelease </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Simple function to re-sort both culomn items.</i><br>
<i>Used Throughout to simply update the display</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>sortLists(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "dirChangedTARGET"></h5><font color = 464646 size = 3><b>dirChanged <font size = 2pt> [<a href="#MnsPluginRelease TARGET">MnsPluginRelease </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>User directory changed trigger action</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>dirChanged(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "splitVerStringToListTARGET"></h5><font color = 464646 size = 3><b>splitVerStringToList <font size = 2pt> [<a href="#MnsPluginRelease TARGET">MnsPluginRelease </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>split version string to a path/minor/major/timestamp elements</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>splitVerStringToList(self, versionString)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>list (versionString)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>versionString</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
##Defenitions
<hr width = 100%>
###loadPluginRelease
<font color = #5f5f5f size = 3pt>
<i>
Load the plugin Release UI from globals, avoid UI duplication. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadPluginRelease()</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
