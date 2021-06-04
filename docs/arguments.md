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
<li>pathMode</li>
<li>pathFileTypes</li>
<li>blockCreationOnly</li>
<li>jntStructMember</li>
<li>jntStructSoftMod</li>
<li>lockOffAttributes</li>
<li>simpleDivider</li>
<li>meshComponents</li>
<li>disabled</li>
</ul>
</td></tr>
<tr><td><b><font color = #4caf50>Methods:  </font></b></td><td><ul>
<li><b><a href="#formatCommentToToolTipTARGET">formatCommentToToolTip </b></a> <font size = 2pt><i>[method]</i></font></li>
</ul>
</td>
</tr>
</table></font>
####MnsArgument  methods
<hr width = 50%>
<h5 id = "formatCommentToToolTipTARGET"></h5><font color = 464646 size = 3><b>formatCommentToToolTip <font size = 2pt> [<a href="#MnsArgument TARGET">MnsArgument </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>formatCommentToToolTip(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
