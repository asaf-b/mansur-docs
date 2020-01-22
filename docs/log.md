<body>
#log
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur === <br>
Core mns logger. <br>
This module contains the mns logger which will construct a log based on given parametrs. <br>
All logs are written to the defined log file dectated by the project globals. <br>
In case a log doesn't exists it will be automatically created. <br>
</font>
</i>
<hr width = 100%>
##Defenitions
<hr width = 100%>
###log
<font color = #5f5f5f size = 3pt>
<i>
Core logger function. <br>
Given a message line and a severity parameter, log the line into the log file. <br>
In case the log file doesn't exist, create one. <br>
In case the directory doesn't exist, create one. <br>
An output message is printed into the consule based on the severity. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>log(msg = "", **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>msg</b>(<i>str</i>) ; [default: ""]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
<td><ul>
<li><b>svr</b>(<i>int</i>) - set the sevarity of the log message</li>
</ul></td>
</tr>
</table></font>
