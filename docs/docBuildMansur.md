<body>
#docBuildMansur
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur === <br>
Core procedural documentation build <br>
Process flow: <br>
Read a given directory <br>
Build a structure based on the os directory given and the folders to filter <br>
Filter only .py files <br>
For each py file: <br>
&nbsp;&nbsp;&nbsp;&nbsp;Extract Header (such as this one) <br>
&nbsp;&nbsp;&nbsp;&nbsp;Extract Defenition <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Extract Def name and constructor <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Extract Arguments, and Optional Arguments <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Extract return <br>
&nbsp;&nbsp;&nbsp;&nbsp;Extract Classes <br>
&nbsp;&nbsp;&nbsp;&nbsp;Extract Header <br>
&nbsp;&nbsp;&nbsp;&nbsp;Extract Name and constructor <br>
&nbsp;&nbsp;&nbsp;&nbsp;Extract inheritence <br>
&nbsp;&nbsp;&nbsp;&nbsp;Extract Class members <br>
&nbsp;&nbsp;&nbsp;&nbsp;Extract Methods <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Extract Header <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Extract Name and constructor <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Extract Arguments and Optional Arguments <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Extract return <br>
rebuild the yml file given <br>
write the files within the 'docs' directory <br>
 <br>
This procedural approach for a code documentation build ensures an up-to-date documentation based on code commenting. <br>
No additional actions are neccessery. <br>
This will yeild a readable commented code with will math the documentation 1-to-1. <br>
Also, this will yeild a very "easy to change" approach for the documentation generator of choice as well as a 100% cohirent documentation throuout. <br>
 <br>
</font>
</i>
<hr width = 100%>
##Defenitions
<hr width = 100%>
###appendMayaPluginsToYml
<font color = #5f5f5f size = 3pt>
<i>
Append the Maya-Plugins documentation page into the existing yml struct. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>appendMayaPluginsToYml(ymlPath, parentPageName)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>ymlPath</b></li>
<li><b>parentPageName</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###buildDocItems
<font color = #5f5f5f size = 3pt>
<i>
Main dir build recursive function. <br>
The function builds only directory items, which in turn will be searched for '.py' files, and will be added to the structure only if in contains a direct '.py' within,  <br>
or if a directory within comatins one, recursively. <br>
Depth independent. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>buildDocItems(dir, rootDir, level, ymlPath, fileLines)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>list (yml new file lines)   </td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>dir</b></li>
<li><b>rootDir</b></li>
<li><b>level</b></li>
<li><b>ymlPath</b></li>
<li><b>fileLines</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###buildDocsForDir
<font color = #5f5f5f size = 3pt>
<i>
Main build wrapper and the yml file writer wrapper function. <br>
Calls 'buildDocItems' within which in turn build the actual html files within the 'docs' directory. <br>
Finally re-writes the yml file using 'rebuildYmlFile' according to the file structure acquired <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>buildDocsForDir(mkDocksYmlPath, parentPageName, directory, folders, level = 0) </td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>mkDocksYmlPath</b></li>
<li><b>parentPageName</b></li>
<li><b>directory</b></li>
<li><b>folders</b></li>
<li><b>level</b>(<i>int</i>) ; [default: 0]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###buildFileDoc
<font color = #5f5f5f size = 3pt>
<i>
Main file def. <br>
This is a wrapped def as well as a function one. <br>
Compiles all needed documentation from a given file path. <br>
Will compile Classes, methods, defenitions (icluding all relevant information for each) <br>
This is also the main WRITE defenition. After info assembly the info will be written as a new file, overriding existing ones, to create a new doc page. <br>
Any file doc 'display' is contained within this def. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>buildFileDoc(path, ymlPath)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>path</b></li>
<li><b>ymlPath</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###buildMansurDocs
<font color = #5f5f5f size = 3pt>
<i>
Main wrapper call for the MANSUR directory doc build.  <br>
Contains the requested folders within, hard-coded for safety. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>buildMansurDocs() </td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###buildReleaseNotesPage
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>buildReleaseNotesPage()</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###buildSubItemsDir
<font color = #5f5f5f size = 3pt>
<i>
Last level recursive function. <br>
This function will call the documentation file build as well as build the last meanu item within the structure. <br>
The final pythonLib item is passed in, as well as the root directory and the current level and the yml path in order to write the new yml lines correctly, depending on the file's level position. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>buildSubItemsDir(rootDir, pyLib, level, ymlPath, fileLines)  </td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>list (fileLines)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rootDir</b></li>
<li><b>pyLib</b></li>
<li><b>level</b></li>
<li><b>ymlPath</b></li>
<li><b>fileLines</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###collectHeaderFromCppFile
<font color = #5f5f5f size = 3pt>
<i>
For the given cpp file, extract the header comment. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>collectHeaderFromCppFile(cppFullPath = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>cppFullPath</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###commitAndDeployDocumentation
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>commitAndDeployDocumentation(rootDrive = "d", relativeDirectory = "mansurProject\\mansur-docs", **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rootDrive</b>(<i>str</i>) ; [default: "d"]</li>
<li><b>relativeDirectory</b>(<i>str</i>) ; [default: "mansurProject\\mansur-docs"]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###createPluginDocFile
<font color = #5f5f5f size = 3pt>
<i>
Create the Maya-Plugins attributes documentation page. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createPluginDocFile(rootBuildPath = "D/mansurProject/mayaPlugins", ymlPath = "D/mansurProject/mansur-docs/mkdocs.yml")</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rootBuildPath</b>(<i>str</i>) ; [default: "D:/mansurProject/mayaPlugins"]</li>
<li><b>ymlPath</b>(<i>str</i>) ; [default: "D:/mansurProject/mansur-docs/mkdocs.yml"]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###extractAttributeDefenitionsFromCppFile
<font color = #5f5f5f size = 3pt>
<i>
From the given cpp path given, extract all attribute information. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>extractAttributeDefenitionsFromCppFile(cppFullPath = None, buildName = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td> list (inuput attributes), list (output attributes)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>cppFullPath</b>(<i>str</i>) ; [default: None]</li>
<li><b>buildName</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###extractClassMembersFromInitSrc
<font color = #5f5f5f size = 3pt>
<i>
Extracts class members from a Class' init method source as list <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>extractClassMembersFromInitSrc(src = [])</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>list (class members names)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>src</b>(<i>list</i>) ; [default: []]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###extractConstructorValuesForClass
<font color = #5f5f5f size = 3pt>
<i>
Extracts constructor related values from a class source as list. <br>
Wrapper def. <br>
Extracts both Arguments (flattened) and class members <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>extractConstructorValuesForClass(src = [])</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>string (constructor), list (class members)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>src</b>(<i>list</i>) ; [default: []]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###extractDocsForClass
<font color = #5f5f5f size = 3pt>
<i>
Wrapped def. <br>
Extracts full documentation from a given class source. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>extractDocsForClass(classSrc = [])</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>string (title), list (header), string (sontructor), string (inherit object), list (class members), string (return) </td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>classSrc</b>(<i>list</i>) ; [default: []]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###extractDocsForDef
<font color = #5f5f5f size = 3pt>
<i>
Wrapper def for a full doc extraction for a given file souce as list. <br>
extracts return statement, title, header, arguments and optionalArguments <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>extractDocsForDef(defSrc = [])</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>string(title), list(header), list(arguments), list(optionalArguments, string(return statement)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>defSrc</b>(<i>list</i>) ; [default: []]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###extractHeaderFromSrc
<font color = #5f5f5f size = 3pt>
<i>
Extracts a header if exsits from a given elemnt src (Class/Def/Method) as list <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>extractHeaderFromSrc(src = [] )</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>list (header lines)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>src</b>(<i>list</i>) ; [default: []]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###extractMethodsfromClassSrc
<font color = #5f5f5f size = 3pt>
<i>
Splits a given class source to orginized dict containing it's methods sources <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>extractMethodsfromClassSrc(src = [])</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>dict (methodName: methodSource)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>src</b>(<i>list</i>) ; [default: []]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###extractParametersFromDefSrc
<font color = #5f5f5f size = 3pt>
<i>
Extract parametrs from a given def source as list <br>
   Extracts arguments and optional arguments <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>extractParametersFromDefSrc(src = [])</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>list (arguments) , list(optionalArguments)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>src</b>(<i>list</i>) ; [default: []]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###gatherPluginDocumentation
<font color = #5f5f5f size = 3pt>
<i>
From the build directory given, extract attributes data directly from the cpp files. <br>
compile the data into input/uotput lists containing dict info for all attributes. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>gatherPluginDocumentation(rootBuildPath = "D/mansurProject/mayaPlugins")</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>list (build list containing extracted attributes data)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rootBuildPath</b>(<i>str</i>) ; [default: "D:/mansurProject/mayaPlugins"]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getParameterForMnsArg
<font color = #5f5f5f size = 3pt>
<i>
Extracts arguments from a given def source lines as list <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getParameterForMnsArg(arg)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>string (flattened combined arguments)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>arg</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getPyLibForDir
<font color = #5f5f5f size = 3pt>
<i>
This is a complex recursive function that will assemble a file structure from a given path directory. <br>
The assembly will filter ONLY folders that contain at least one '.py' file, and ONLY '.py' files. <br>
This function returns a dictionary containing the file and folder structure as keys "dirs" and "files" respectively. <br>
As this is a recusrsive depth independent function, the return will be a complex compound dict, which contains instances of the same dict structure within. <br>
This is dependent of depth obviously-  <br>
if a directory contains another directory within- which contains a '.py' the first item "dirs" key will contain another dictionary containing a "dirs" key and a "files" key. <br>
Ultimatly, the first dict "dirs" key should contain a single complex dict element. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getPyLibForDir(root)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>dict (complex library dict)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>root</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###rebuildYmlFile
<font color = #5f5f5f size = 3pt>
<i>
yml writer function. <br>
Writes the given yml file passed, with the new 'lines' passed. <br>
The yml 'parentPageName' is passed as an argument - the new 'lines' build is constructed underneeth. <br>
Existing required info is preserved by calculating the parent item indentation level, keeping every item with lower or matching level. <br>
Every item under the parent item passed in a higher level is removed or reconstructed. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>rebuildYmlFile(ymlPath, parentPageName, lines)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>ymlPath</b></li>
<li><b>parentPageName</b></li>
<li><b>lines</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
