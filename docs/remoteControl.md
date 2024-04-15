<body>
#remoteControl
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
Author: Asaf Ben-Zur <br>
Best used for: Blend Shape Targets, Facial-Remotes, General Extra-Setups <br>
This moudle, upon construction, will create a remote-control style control. <br>
It will create a frame, with a control within, limited to that frame. <br>
The frame range is dictated by the settings below. <br>
Use the min-max values for both vertical and horizontal directions to create the remote that best fitting to your needs. <br>
You can freely use both vertical and horizontal directions in combination. <br>
This type of control is often seen when creating a blend-shape-based facial rig, with an adjacent remote control to easily and visually animate the targets instead of using the channel box directly. <br>
Also, you can control the target value range for your control. <br>
That means that the control and target ranges can differ. <br>
For example, a blend shape target with values between 0 and 1 is needed to be controlled. <br>
You can set the control range between 0 and 5, while keeping the target range between 0 and 1, which will result in a slower behaving control for more fidelity. <br>
The target connection is handled post-construction so connecting to constructed objects is also possible. <br>
Multiple targets can be input into the same target. Simply select multiple targets and input. Alternatively manually input the targets, separated by commas. <br>
Module build assumptions/requisites: <br>
- targetMin < targetMax <br>
- rangeMin < rangeMax <br>
- A target can be shared within a direction minimum and maximum <br>
- Output ranges between 0.0 and TargetMax given 0.0 and range Max <br>
- Output ranges between 0.0 and TargetMin given 0.0 and range Min <br>
- AKA the module assumes 0.0 as a default value for both input range and target range <br>
 <br>
</font>
</i>
<hr width = 100%>
##Defenitions
<hr width = 100%>
###construct
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>construct(mansur, MnsBuildModule, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td> list (controls), dict (internalSpaces)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>mansur</b></li>
<li><b>MnsBuildModule</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###jointStructure
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>jointStructure(mansur, guides, mnsBuildModule = None, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>mansur</b></li>
<li><b>guides</b></li>
<li><b>mnsBuildModule</b>(<i>str</i>) ; [default: None]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###postConstruct
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>postConstruct(mansur, MnsBuildModule, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>mansur</b></li>
<li><b>MnsBuildModule</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
