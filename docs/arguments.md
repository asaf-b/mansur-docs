<body>
#arguments
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur === <br>
MNS main arguments core functions and Classes. <br>
This module holds the MnsArgument class as well as all argument handeling functions. <br>
This module was designed to procedurally handle function arguments in order to manipulate them, generate dynamic UI's from them, and pass them along back to their creator function as an execute. <br>
</font>
</i>
<hr width = 100%>
##Classes
<hr width = 100%>
<h5 id = "MnsArgument TARGET"></h5>
###MnsArgument [Class]
<font color = #5f5f5f size = 3pt>
<i>
MnsArgument Convieniency Class. <br>
A class instance holds all relevant information regarding an extracted single function argument. <br>
These class members will dectate any behavior derived from an actual function object or a method object. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>MnsArgument(<b>**kwargs</b>)</td></tr>
<tr><td><b><font color = #4caf50>Inherits from:  </font></b></td><td>object</td></tr>
<tr><td><b><font color = #4caf50>Class Members:  </font></b></td>
<td><ul>
<ul>
<li>name</li>
<li>type</li>
<li>default</li>
<li>min</li>
<li>max</li>
<li>comment</li>
<li>ob</li>
<li>side</li>
<li>blockCreationOnly</li>
<li>jntStructMember</li>
</ul>
</td></tr>
</tr>
</table></font>
<hr width = 100%>
##Defenitions
<hr width = 100%>
###extractArgsFromDef
<font color = #5f5f5f size = 3pt>
<i>
This function will extract all arguments and optional arguments from a given function object. <br>
Returns two lists containing MnsArgument instances. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>extractArgsFromDef(defenition)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>list (arguments MnsArgument list), list (optional arguments MnsArgument list)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>defenition</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###extractArgsFromSource
<font color = #5f5f5f size = 3pt>
<i>
This function will extract all arguments and optional arguments from a given function source. <br>
Returns two lists containing MnsArgument instances. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>extractArgsFromSource(src)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>list (arguments MnsArgument list), list (optional arguments MnsArgument list)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>src</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###extractChennelControlDefaultFromLine
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>extractChennelControlDefaultFromLine(line = "", argAame = "")</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td> dict</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>line</b>(<i>str</i>) ; [default: ""]</li>
<li><b>argAame</b>(<i>str</i>) ; [default: ""]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###extractColorSchemeDefaultFromLine
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>extractColorSchemeDefaultFromLine(line = "", argAame = "")</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>line</b>(<i>str</i>) ; [default: ""]</li>
<li><b>argAame</b>(<i>str</i>) ; [default: ""]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###formatArgumetsAsDict
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>formatArgumetsAsDict(mnsArgsList = [])</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>mnsArgsList</b>(<i>list</i>) ; [default: []]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###recompileArgumetsAsString
<font color = #5f5f5f size = 3pt>
<i>
A reverse function to the 'extractArgsFromDef'. <br>
In order to pass any arguments back to it's creator, comes a need to re-compile an argument list into a single callable formatted string. <br>
This function covers this need. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>recompileArgumetsAsString(defenition, arguments, optArgs, values)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>string (re-compiled arguments as string)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>defenition</b></li>
<li><b>arguments</b></li>
<li><b>optArgs</b></li>
<li><b>values</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###returnValueAndTypeFromArgString
<font color = #5f5f5f size = 3pt>
<i>
This function will return a value (as its actual type) and a type (as a type object) from a given extracted argument string <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>returnValueAndTypeFromArgString(argString = "")</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>value (Dynamic type), type (type object)     </td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>argString</b>(<i>str</i>) ; [default: ""]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###splitStringToArg
<font color = #5f5f5f size = 3pt>
<i>
This function return a MnsArgument object from a given argument string. <br>
It will split the argument string into actual elemnts and values and directly ingest them into the class members. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>splitStringToArg(argAsString)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsArgument</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>argAsString</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
