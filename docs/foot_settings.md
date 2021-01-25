<body>
#foot Settings
<hr width = 100%>
##Attributes
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr>
<td>FKControlShape</td>
<td>cube</td>
<td>Toes FK controls shape</td>
</tr></td>
<tr>
<td>FKChannelControl</td>
<td>{'s': (True, True, True), 'r': (True, True, True), 't': (True, True, True)}</td>
<td>Toes FK controls channel-box settings</td>
</tr></td>
<tr>
<td>BKControlShape</td>
<td>diamond</td>
<td>BK (Backward Kinematics) controls shape</td>
</tr></td>
<tr>
<td>BKChannelControl</td>
<td>{'s': (False, False, False), 'r': (True, True, True), 't': (False, False, False)}</td>
<td>BK controls channel-box settings</td>
</tr></td>
<tr>
<td>bankControlShape</td>
<td>lightSphere</td>
<td>Bank controls shape</td>
</tr></td>
<tr>
<td>bankChannelControl</td>
<td>{'s': (False, False, False), 'r': (True, True, True), 't': (False, False, False)}</td>
<td>bank controls channel-box settings</td>
</tr></td>
<tr>
<td>doRollCtrl</td>
<td>True</td>
<td>If this is True, a foot Roll control will be created</td>
</tr></td>
<tr>
<td>rollControlShape</td>
<td>cylinder</td>
<td>Roll control channel-box settings</td>
</tr></td>
<tr>
<td>rollDefaultMaxAngle</td>
<td>30.0</td>
<td>Default Roll maximum limit angle. The roll control is used to roll the entire foot chain, and using an angle value to limit the roll of each section, before rolling the next section. This value will be used as default</td>
</tr></td>
<tr>
<td>doDynamicPivCtrl</td>
<td>True</td>
<td>This feature will create a control that will try to trace the desired foot shape with it's pivot when rotating it. When choosing to create this control, use the relevant guide's shape to trace the outline of your foot</td>
</tr></td>
<tr>
<td>dynamicPivControlShape</td>
<td>lightSphere</td>
<td>Dynamic roll control shape</td>
</tr></td>
<tr>
<td>mapRotXTo</td>
<td>2</td>
<td>as this feature uses local channels, it is essential to map input values correctly. Please map the correct axes based on the orientation of your guide</td>
</tr></td>
<tr>
<td>mapRotYTo</td>
<td>3</td>
<td>as this feature uses local channels, it is essential to map input values correctly. Please map the correct axes based on the orientation of your guide</td>
</tr></td>
<tr>
<td>mapRotZTo</td>
<td>6</td>
<td>as this feature uses local channels, it is essential to map input values correctly. Please map the correct axes based on the orientation of your guide</td>
</tr></td>
<tr>
<td>distRateMultiplier</td>
<td>5.0</td>
<td>This feature will use the translation of a run-away transform to acquire the best pivot location along the given outline shape. This value will dictate the speed of translation</td>
</tr></td>
<tr>
<td>dynamicPivChannelControl</td>
<td>{'s': (False, False, False), 'r': (True, True, False), 't': (False, False, False)}</td>
<td>Roll control channel-box settings</td>
</tr></td>
</table></font>
