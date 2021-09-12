<body>
#lips Settings
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
</table></font>
###GlobalSettings
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>upperEdgeVerts</td>
<td>[' ']</td>
<td>These verticies will be used to build the joint structure for the upper section. Please select a sequence of vertices along the same loop, starting from the inner corner. First and last vertices should match between the upper and lower section, representing a single closed loop. Corner vertices will be present twice- once on the upper section, once on the lower section</td></tr>
<tr><td>lowerEdgeVerts</td>
<td>[' ']</td>
<td>These verticies will be used to build the joint structure for the lower section. Please select a sequence of vertices along the same loop, starting from the inner corner. First and last vertices should match between the upper and lower section, representing a single closed loop. Corner vertices will be present twice- once on the lower section, once on the lower section</td></tr>
<tr><td>upCurveOffset</td>
<td>1.0</td>
<td>Comment wasn't inserted</td></tr>
<tr><td>reverseCorners</td>
<td>False</td>
<td>Offset value for the up curve generation</td></tr>
<tr><td>aroundCenter</td>
<td>False</td>
<td>Around center will normalize the result vectors around a given center matrix (module root in this case). This will provide a better range of motion, tranlating the joints around a sphere (assumed from the center matrix). This can be changed and animated post-construction</td></tr>
<tr><td>curveResolution</td>
<td>24</td>
<td>Resample curve amount</td></tr>
<tr><td>midCurveHeight</td>
<td>0.5</td>
<td>This dictates the height of the Mid-Meet point between the upper and lower sections</td></tr>
<tr><td>jawRootGuide</td>
<td></td>
<td>In case this module is used for lips (main use), input the Jaw control root guide. This will implement the Jaw control within the setup and will result in a better behaving setup</td></tr>
</table></font>
###AlongSurface
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>doAlongSurface</td>
<td>False</td>
<td>In case it is desired, an internal surface(Nurbs)-follow mechanism is built in this module. In some cases, it is desired to model a pre-existing NurbsSurface that describes the range or limits of the joints related to this module. If a valid input is insrted, the setup will be created automatically. Remember that the follow controls will be pinned to the given surface, so remember to skin the surface to parent module which will follow the world position of the guide surface. Freezing transformation on the given setup is essential for this feature to behave as expected</td></tr>
<tr><td>inputSurface</td>
<td></td>
<td>Input surface (Nurbs) to follow</td></tr>
<tr><td>baseSurfaceJointFollow</td>
<td></td>
<td>It is recommended to use this attribute in conjunction with the alongSurface module. The alongSurface feature is stabler when a baseSurface is present. In order to create that base surface automatically, Block needs a joint to flood a skin to, in order to follow the world space position of the character. For example, if your input surface is skinned to the head joint and the jaw joint, the recommended input in this attribute will be the head joint. When this attribute is empty or invalid a base surface will not be created.</td></tr>
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
###TweakControls
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>doTweakControls</td>
<td>True</td>
<td>First layer tweakers</td></tr>
<tr><td>numTweakControlsPerSection</td>
<td>5</td>
<td>Number of tweak controls per section</td></tr>
<tr><td>cornersControlShape</td>
<td>diamond</td>
<td>Tweak coreners control shape</td></tr>
<tr><td>tweakersControlShape</td>
<td>lightSphere</td>
<td>Tweak controls shape</td></tr>
<tr><td>tweakCurvesInterpolation</td>
<td>4</td>
<td>First layer tweaks curve interpolation type</td></tr>
</table></font>
###LayerBCtrls
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>doLayerBCtrls</td>
<td>False</td>
<td>Second layer tweakers</td></tr>
<tr><td>numLayerBCtrlsPerSection</td>
<td>9</td>
<td>Number of tweak controls per section</td></tr>
<tr><td>layerBControlShape</td>
<td>cube</td>
<td>Second layer tweak controls shape</td></tr>
</table></font>
