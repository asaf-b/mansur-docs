<body>
#lipsB Settings
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
Author: Asaf Ben-Zur <br>
Best used for: Lips <br>
This module was designed around lips behaviour. <br>
This module has a few layers that will allow general as well as extremely fiddle control (based on parameters) over the lips deformation. <br>
Some of the main features in this module include: Macro corner controls, Along Surface feature, Around Center Feature, Jaw connections, Global "Full-Lips" control, Zip Controls, Curve meet controls, Tweak controls, Cheek Raise connection,  and much more. <br>
The joint structure of this module will be dictated by input vertices on a given mesh. <br>
</i>
<br>
</font>
<hr width = 100%>
##Attributes
<tr><td>isFacial</td>
<td>True</td>
<td>Comment wasn't inserted</td></tr>
<tr><td>postSymmetryJntStruct</td>
<td>True</td>
<td>Comment wasn't inserted</td></tr>
<tr><td>alongSurface</td>
<td></td>
<td>Comment wasn't inserted</td></tr>
<tr><td>symmetryType</td>
<td>1</td>
<td>Choose the mirror type for right side controls</td></tr>
</table></font>
###GlobalSettings
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>upperEdgeVerts</td>
<td>[' ']</td>
<td>These verticies will be used to build the joint structure for the upper section. Please select a sequence of vertices along the same loop, starting from the inner corner. First and last vertices should match between the upper and lower section, representing a single closed loop. Corner vertices will be present twice- once on the upper section, once on the lower section</td></tr>
<tr><td>lowerEdgeVerts</td>
<td>[' ']</td>
<td>These verticies will be used to build the joint structure for the lower section. Please select a sequence of vertices along the same loop, starting from the inner corner. First and last vertices should match between the upper and lower section, representing a single closed loop. Corner vertices will be present twice- once on the lower section, once on the lower section</td></tr>
<tr><td>midsPosition</td>
<td>0</td>
<td>In case this setting is set to custom, once the settings are updated, 4 new locator guides will become visible- 2 for the upper lip, and 2 for the lower lip. These locators can be manually set to a custom mid-lip position. In some cases, based on the models geometry, the mid-lip automatic control position may not be calculated correctly. If this is your case, turn this setting on and set the guide locators to the required mid-lip position for both upper and lower lips</td></tr>
</table></font>
###ctrlShapes
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>cornerControlShape</td>
<td>fourArrow</td>
<td>Main corenr controls shape</td></tr>
<tr><td>upperLowerControlShape</td>
<td>squareRound</td>
<td>Main upper and lower controls shape</td></tr>
<tr><td>midsControlShape</td>
<td>circle</td>
<td>Main mid controls shape</td></tr>
</table></font>
###JawConnection
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>connectJaw</td>
<td>True</td>
<td>In case this attribute is off, the jaw connection will not be created.</td></tr>
<tr><td>jawRootGuide</td>
<td></td>
<td>In case this module is used for lips (main use), input the Jaw control root guide. This will implement the Jaw control within the setup and will result in a better behaving setup</td></tr>
<tr><td>connectUpMotionRot</td>
<td>True</td>
<td>In case this attribute is ON, the up rotation of the jaw will affect the upper lip.</td></tr>
<tr><td>upMotionRotAxis</td>
<td>-x</td>
<td>Rotation axis axis to connect the up motion to. This is based on the selected orientation for te jaw.</td></tr>
<tr><td>connectUpMotionTran</td>
<td>True</td>
<td>In case this attribute is ON, the up translation of the jaw will affect the upper lip.</td></tr>
<tr><td>upMotionTranAxis</td>
<td>y</td>
<td>Rotation axis axis to connect the up motion to. This is based on the selected orientation for te jaw.</td></tr>
</table></font>
###LayerBCtrls
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>doLayerBCtrls</td>
<td>True</td>
<td>Second layer tweakers</td></tr>
<tr><td>numLayerBCtrlsPerSection</td>
<td>9</td>
<td>Number of tweak controls per section</td></tr>
<tr><td>layerBSamplingMode</td>
<td>2</td>
<td>Second layer tweak sampling mode.</td></tr>
<tr><td>layerBInterpolation</td>
<td>1</td>
<td>Second layer tweak interpolation type.</td></tr>
<tr><td>layerBControlShape</td>
<td>cube</td>
<td>Second layer tweak controls shape</td></tr>
</table></font>
###CheekRaise
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>doCheekRaise</td>
<td>False</td>
<td>when dealing with joint based facial deformation, and using this module as a lips setup, it is sometimes desired to incorporate another control that represents the cheek to achive a more lively deformation. Use this feature to do just that. Plug in the rootGuide of the cheeck control you wish to drive, then control the raise and push values based on your preferences or requirements</td></tr>
<tr><td>l_CheekRaiseRoot</td>
<td></td>
<td>Left side cheeck Root Guide</td></tr>
<tr><td>r_CheekRaiseRoot</td>
<td></td>
<td>Right side cheeck Root Guide</td></tr>
<tr><td>raiseValue</td>
<td>0.5</td>
<td>Raise default value</td></tr>
<tr><td>connectRaiseToAxis</td>
<td>y</td>
<td>Raise channel connection axis</td></tr>
<tr><td>pushValue</td>
<td>0.5</td>
<td>Push-Out default value</td></tr>
<tr><td>connectPushToAxis</td>
<td>z</td>
<td>Raise channel connection axis</td></tr>
</table></font>
