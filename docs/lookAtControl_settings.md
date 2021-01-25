<body>
#lookAtControl Settings
<hr width = 100%>
##Attributes
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr>
<td>slaveControlShape</td>
<td>lightSphere</td>
<td>Origin slave control shape</td>
</tr></td>
<tr>
<td>targetControlShape</td>
<td>circle</td>
<td>Main control shape</td>
</tr></td>
<tr>
<td>channelControl</td>
<td>{'s': (True, True, True), 'r': (True, True, True), 't': (True, True, True)}</td>
<td>Main control channel-box settings</td>
</tr></td>
<tr>
<td>pupilDilateAttribute</td>
<td></td>
<td>Input bland-shape attribute to connect pupil dialation control to</td>
</tr></td>
<tr>
<td>pupilContractAttribute</td>
<td></td>
<td>Input bland-shape attribute to connect pupil contaction control to</td>
</tr></td>
<tr>
<td>irisDilateAttribute</td>
<td></td>
<td>Input bland-shape attribute to connect iris dialation control to</td>
</tr></td>
<tr>
<td>irisContractAttribute</td>
<td></td>
<td>Input bland-shape attribute to connect iris contaction control to</td>
</tr></td>
<tr>
<td>combinedAttributeHost</td>
<td></td>
<td>If this is set to True, a global attribute for the above pupil and iris controls will be created on the specified attribute host. This feature is mainly to combine two different eye shapes controls into one single control, or moving the location of this attribute to a diffent module in case the eye meshs are combined</td>
</tr></td>
</table></font>
