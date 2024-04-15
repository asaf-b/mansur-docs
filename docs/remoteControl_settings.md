<body>
#remoteControl Settings
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
 <br>
Also, you can control the target value range for your control. <br>
That means that the control and target ranges can differ. <br>
For example, a blend shape target with values between 0 and 1 is needed to be controlled. <br>
You can set the control range between 0 and 5, while keeping the target range between 0 and 1, which will result in a slower behaving control for more fidelity. <br>
 <br>
The target connection is handled post-construction so connecting to constructed objects is also possible. <br>
Multiple targets can be input into the same target. Simply select multiple targets and input. Alternatively manually input the targets, separated by commas. <br>
 <br>
Module build assumptions/requisites: <br>
- targetMin < targetMax <br>
- rangeMin < rangeMax <br>
- A target can be shared within a direction minimum and maximum <br>
- Output ranges between 0.0 and TargetMax given 0.0 and range Max <br>
- Output ranges between 0.0 and TargetMin given 0.0 and range Min <br>
- AKA the module assumes 0.0 as a default value for both input range and target range <br>
</i>
<br>
</font>
<hr width = 100%>
##Attributes
<tr><td>symmetryType</td>
<td>0</td>
<td>Choose the mirror type for right side controls</td></tr>
<tr><td>doAttributeHostCtrl</td>
<td>False</td>
<td>Comment wasn't inserted</td></tr>
<tr><td>attributeHostControlShape</td>
<td>plus</td>
<td>Comment wasn't inserted</td></tr>
<tr><td>attrHostSpace</td>
<td></td>
<td>Comment wasn't inserted</td></tr>
</table></font>
###GlobalSettings
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>controlScale</td>
<td>1.0</td>
<td>Size of the remote created</td></tr>
<tr><td>textScale</td>
<td>1.0</td>
<td>Size of the text label, relative to the control scale</td></tr>
<tr><td>upTraget</td>
<td></td>
<td>Attribute. Select the target attribute in the main channel-box, then click the input arrow to the right of the field box to insert it</td></tr>
<tr><td>downTraget</td>
<td></td>
<td>Attribute. Select the target attribute in the main channel-box, then click the input arrow to the right of the field box to insert it</td></tr>
<tr><td>leftTraget</td>
<td></td>
<td>Attribute. Select the target attribute in the main channel-box, then click the input arrow to the right of the field box to insert it</td></tr>
<tr><td>rightTraget</td>
<td></td>
<td>Attribute. Select the target attribute in the main channel-box, then click the input arrow to the right of the field box to insert it</td></tr>
</table></font>
###RemoteRange
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>verticalMinimum</td>
<td>0.0</td>
<td>Vertical range minimum</td></tr>
<tr><td>verticalMaximum</td>
<td>1.0</td>
<td>Vertical range maximum</td></tr>
<tr><td>verticalDefault</td>
<td>0.0</td>
<td>Vertical range default</td></tr>
<tr><td>horizontalMinimum</td>
<td>0.0</td>
<td>Horizontal range minimum</td></tr>
<tr><td>horizontalMaximum</td>
<td>0.0</td>
<td>Horizontal range maximum</td></tr>
<tr><td>horizontalDefault</td>
<td>0.0</td>
<td>Horizontal range default</td></tr>
</table></font>
###RemoteTragetValues
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>verticalTargetMinimum</td>
<td>0.0</td>
<td>Vertical target minimum</td></tr>
<tr><td>verticalTargetMaximum</td>
<td>1.0</td>
<td>Vertical target maximum</td></tr>
<tr><td>horizontalTargetMinimum</td>
<td>0.0</td>
<td>Horizontal target minimum</td></tr>
<tr><td>horizontalTargetMaximumm</td>
<td>1.0</td>
<td>Horizontal target maximum</td></tr>
</table></font>
