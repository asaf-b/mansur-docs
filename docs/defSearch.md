<body>
#defSearch
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur === <br>
Core MNS Utility UI <br>
This UI will allow the user to search though all available function within a given library and build a dynamic UI for it, based on it's arguments and keyword arguments drawen as 'type' QObjects into a new UI window. <br>
This UI class will search thorugh the default library (mns), although has functionallity to add any library into the search. <br>
IMPORTANT: Any given custom library needs to follow the mns code structure convension in order to work and sraw properly. Please refer to some code examples. <br>
The main process of this UI class is: <br>
- Load the UI <br>
- procedurally look through the given libraries and add any found python defenition into the UI list. <br>
- Uppon a 'UI creation' call (via the button or souble-click): <br>
&nbsp;&nbsp;&nbsp;&nbsp;- Deconstruct the selected defenition into mandatory arguments and keyword arguments <br>
&nbsp;&nbsp;&nbsp;&nbsp;- Build a new UI based on the parameters got. <br>
- Uppon a 'Run' call: <br>
&nbsp;&nbsp;&nbsp;&nbsp;- Re-construct the function's argument based on the UI fields and recompile into a string <br>
&nbsp;&nbsp;&nbsp;&nbsp;- Call the selected function using the complied arguent string <br>
Features: <br>
- Prefs tab to control the UI's behavior. <br>
- Directory addition <br>
- Indepentent custom '.py' files add <br>
- Library reload <br>
- 'Default Prefs restore' <br>
- Settings export/import <br>
- Function 'pinning' (Global, session independent) <br>
- UI features - Search, Case-Sensative display, Pinned view only, clear all pinns <br>
- 'dev mode': <br>
&nbsp;&nbsp;&nbsp;&nbsp;- When set to False (default) the UI call will create a new UI only if it han't been created before-  <br>
&nbsp;&nbsp;&nbsp;&nbsp;meaning that the UI objects are kept within the UI class, and when closed will not lose their user-set values.  <br>
&nbsp;&nbsp;&nbsp;&nbsp;When called again, the UI will simply re-load- not re-create to keep previous set values. The function will not be read again to build. <br>
&nbsp;&nbsp;&nbsp;&nbsp;When set to True, instead of re-loading of a previously created UI- it will be deleted- and recreated, READING THE FUNCTION AGAIN. <br>
&nbsp;&nbsp;&nbsp;&nbsp;This allows the user to re-read a function every time the UI is called- that means that all previous value set will be lost- as the UI rebuilds it will set all items to default value. <br>
&nbsp;&nbsp;&nbsp;&nbsp;This gives a very fast way of developing a function- not needing to re-load maya after edit- <br>
&nbsp;&nbsp;&nbsp;&nbsp;The UI will rebuild based on any change made to the defenition code, adding any new items or running a different fuctionallity every run call. <br>
&nbsp;&nbsp;&nbsp;&nbsp;Use this feature when writing or developing a new fuction. <br>
</font>
</i>
<hr width = 100%>
##Classes
<hr width = 100%>
<h5 id = "MnsDefSearch TARGET"></h5>
###MnsDefSearch [Class]
<font color = #5f5f5f size = 3pt>
<i>
Main UI Class <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>MnsDefSearch(<b>parent</b>(<i>str</i>) ; [default: mnsUIUtils.get_maya_window()])</td></tr>
<tr><td><b><font color = #4caf50>Inherits from:  </font></b></td><td>form_class, base_class</td></tr>
<tr><td><b><font color = #4caf50>Class Members:  </font></b></td>
<td><ul>
<ul>
<li>pinnedFilePath</li>
</ul>
</td></tr>
<tr><td><b><font color = #4caf50>Methods:  </font></b></td><td><ul>
<li><b><a href="#initializePinnedDirTARGET">initializePinnedDir </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#clearResultsTARGET">clearResults </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#clearPinsTARGET">clearPins </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#connectSignalsTARGET">connectSignals </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#importModulesTARGET">importModules </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadWindowTARGET">loadWindow </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#updateResultsTARGET">updateResults </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#createUITARGET">createUI </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadListTARGET">loadList </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#addModuleToResultsTARGET">addModuleToResults </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#addPackageToResultsTARGET">addPackageToResults </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#pinTARGET">pin </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#pinnedOnlyViewTARGET">pinnedOnlyView </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#import_submodulesTARGET">import_submodules </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#reloadResultsTARGET">reloadResults </b></a> <font size = 2pt><i>[method]</i></font></li>
</ul>
</td>
</tr>
</table></font>
####MnsDefSearch  methods
<hr width = 50%>
<h5 id = "initializePinnedDirTARGET"></h5><font color = 464646 size = 3><b>initializePinnedDir <font size = 2pt> [<a href="#MnsDefSearch TARGET">MnsDefSearch </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>initializePinnedDir(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "clearResultsTARGET"></h5><font color = 464646 size = 3><b>clearResults <font size = 2pt> [<a href="#MnsDefSearch TARGET">MnsDefSearch </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Clear Serach method trigger.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>clearResults(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "clearPinsTARGET"></h5><font color = 464646 size = 3><b>clearPins <font size = 2pt> [<a href="#MnsDefSearch TARGET">MnsDefSearch </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Clear all pinns method trigger.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>clearPins(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "connectSignalsTARGET"></h5><font color = 464646 size = 3><b>connectSignals <font size = 2pt> [<a href="#MnsDefSearch TARGET">MnsDefSearch </a> class method] </font></font></b>
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
<h5 id = "importModulesTARGET"></h5><font color = 464646 size = 3><b>importModules <font size = 2pt> [<a href="#MnsDefSearch TARGET">MnsDefSearch </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Import modules wrapper.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>importModules(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "loadWindowTARGET"></h5><font color = 464646 size = 3><b>loadWindow <font size = 2pt> [<a href="#MnsDefSearch TARGET">MnsDefSearch </a> class method] </font></font></b>
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
<h5 id = "updateResultsTARGET"></h5><font color = 464646 size = 3><b>updateResults <font size = 2pt> [<a href="#MnsDefSearch TARGET">MnsDefSearch </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Main UI view update method trigger.</i><br>
<i>The UI list will be updated from this method based on the current UI state and prefs</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>updateResults(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "createUITARGET"></h5><font color = 464646 size = 3><b>createUI <font size = 2pt> [<a href="#MnsDefSearch TARGET">MnsDefSearch </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Main dynamic UI creation method trigger based on current selection.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createUI(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "loadListTARGET"></h5><font color = 464646 size = 3><b>loadList <font size = 2pt> [<a href="#MnsDefSearch TARGET">MnsDefSearch </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Main list load method.</i><br>
<i>A wrapper to filter all functions based on prefs selected and update the UI.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadList(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "addModuleToResultsTARGET"></h5><font color = 464646 size = 3><b>addModuleToResults <font size = 2pt> [<a href="#MnsDefSearch TARGET">MnsDefSearch </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Module add method trigger.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>addModuleToResults(self, module) </td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>module</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "addPackageToResultsTARGET"></h5><font color = 464646 size = 3><b>addPackageToResults <font size = 2pt> [<a href="#MnsDefSearch TARGET">MnsDefSearch </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Package addition method trigger.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>addPackageToResults(self, package)   </td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>package</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "pinTARGET"></h5><font color = 464646 size = 3><b>pin <font size = 2pt> [<a href="#MnsDefSearch TARGET">MnsDefSearch </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Pin call method trigger based on current selection.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>pin(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "pinnedOnlyViewTARGET"></h5><font color = 464646 size = 3><b>pinnedOnlyView <font size = 2pt> [<a href="#MnsDefSearch TARGET">MnsDefSearch </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Pinned only view trigger method.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>pinnedOnlyView(self, state)</td></tr>
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
<h5 id = "import_submodulesTARGET"></h5><font color = 464646 size = 3><b>import_submodules <font size = 2pt> [<a href="#MnsDefSearch TARGET">MnsDefSearch </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Recursive method to walk thorugh a given package and sub-packages to store all sub-directories within.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>import_submodules(self, package, recursive=True)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>dict</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>package</b></li>
<li><b>recursive</b>(<i>bool</i>) ; [default: True]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "reloadResultsTARGET"></h5><font color = 464646 size = 3><b>reloadResults <font size = 2pt> [<a href="#MnsDefSearch TARGET">MnsDefSearch </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Wrapper re-load method.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>reloadResults(self)</td></tr>
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
###loadDefSearch
<font color = #5f5f5f size = 3pt>
<i>
Load the Def Serach UI from globals, avoid UI duplication. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadDefSearch()</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
