<body>
#prefixSuffix
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur === <br>
All global prefix and suffix declerations. <br>
All global Mns pre-defined dictionaries creation (i.e.  mnsTypeDict/mnsSidesDict/mnsBuildObjectTypes) <br>
This module also holds the MnsTypeStd class and the MnsNameStd class. <br>
This module holds any global dict creation defenitions used in MNS. <br>
</font>
</i>
<hr width = 100%>
##Classes
<hr width = 100%>
<h5 id = "MnsNameStd TARGET"></h5>
###MnsNameStd [Class]
<font color = #5f5f5f size = 3pt>
<i>
This class holds simple attributes to extend pythos's 'node' object in order to preserve additional information regarding a node. <br>
Any name related methods are held by this class. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>MnsNameStd(<b>**kwargs</b>)</td></tr>
<tr><td><b><font color = #4caf50>Inherits from:  </font></b></td><td>object</td></tr>
<tr><td><b><font color = #4caf50>Class Members:  </font></b></td>
<td><ul>
<ul>
<li>node</li>
<li>side</li>
<li>body</li>
<li>type</li>
<li>id</li>
<li>alpha</li>
<li>suffix</li>
<li>name</li>
<li>namespace</li>
<li>comment</li>
</ul>
</td></tr>
<tr><td><b><font color = #4caf50>Methods:  </font></b></td><td><ul>
<li><b><a href="#setNodeNameTARGET">setNodeName </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#buildNameTARGET">buildName </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#findNextAlphaIncrementTARGET">findNextAlphaIncrement </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#findNextIncrementTARGET">findNextIncrement </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#splitNameTARGET">splitName </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#splitDefinedNameTARGET">splitDefinedName </b></a> <font size = 2pt><i>[method]</i></font></li>
</ul>
</td>
</tr>
</table></font>
####MnsNameStd  methods
<hr width = 50%>
<h5 id = "setNodeNameTARGET"></h5><font color = 464646 size = 3><b>setNodeName <font size = 2pt> [<a href="#MnsNameStd TARGET">MnsNameStd </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setNodeName(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "buildNameTARGET"></h5><font color = 464646 size = 3><b>buildName <font size = 2pt> [<a href="#MnsNameStd TARGET">MnsNameStd </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Build the instance's name based on the current class members defenitions.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>buildName(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "findNextAlphaIncrementTARGET"></h5><font color = 464646 size = 3><b>findNextAlphaIncrement <font size = 2pt> [<a href="#MnsNameStd TARGET">MnsNameStd </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Recursive.</i><br>
<i>Find next available Alpha id increment</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>findNextAlphaIncrement(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "findNextIncrementTARGET"></h5><font color = 464646 size = 3><b>findNextIncrement <font size = 2pt> [<a href="#MnsNameStd TARGET">MnsNameStd </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Recursive.</i><br>
<i>Find next available id increment</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>findNextIncrement(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "splitNameTARGET"></h5><font color = 464646 size = 3><b>splitName <font size = 2pt> [<a href="#MnsNameStd TARGET">MnsNameStd </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>This function splits a given node name as string into an MnsNameStd object</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>splitName(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "splitDefinedNameTARGET"></h5><font color = 464646 size = 3><b>splitDefinedName <font size = 2pt> [<a href="#MnsNameStd TARGET">MnsNameStd </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>This function splits a given object name as string into an MnsNameStd object</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>splitDefinedName(self)</td></tr>
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
<h5 id = "MnsTypeStd TARGET"></h5>
###MnsTypeStd [Class]
<font color = #5f5f5f size = 3pt>
<i>
This class holds simple attributes to extend pythos's 'type' object in order to preserve additional information regarding a node's type. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>MnsTypeStd(<b>**kwargs</b>)</td></tr>
<tr><td><b><font color = #4caf50>Inherits from:  </font></b></td><td>object</td></tr>
<tr><td><b><font color = #4caf50>Class Members:  </font></b></td>
<td><ul>
<ul>
<li>name</li>
<li>suffix</li>
<li>createName</li>
<li>comment</li>
</ul>
</td></tr>
</tr>
</table></font>
<hr width = 100%>
##Defenitions
<hr width = 100%>
###buildMultKeysDict
<font color = #5f5f5f size = 3pt>
<i>
Build a multy key dict for the given item list <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>buildMultKeysDict(items = [])</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>dict</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>items</b>(<i>list</i>) ; [default: []]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###buildOptionArrayFromDict
<font color = #5f5f5f size = 3pt>
<i>
Construct an option list from the given dictionary <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>buildOptionArrayFromDict(dict = {}, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td> list</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>dict</b>(<i>dict</i>) ; [default: {}]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###buildTypeDict
<font color = #5f5f5f size = 3pt>
<i>
Build a dictionary for a given list, adding index (int) key and an index (string) key for each item <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>buildTypeDict(namesArray = [])</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>dict</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>namesArray</b>(<i>list</i>) ; [default: []]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
