<body>
#lips Settings
<hr width = 100%>
##Attributes
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr>
<td>upperEdgeVerts</td>
<td>[' ']</td>
<td>These verticies will be used to build the joint structure for the upper section. Please select a sequence of vertices along the same loop, starting from the inner corner. First and last vertices should match between the upper and lower section, representing a single closed loop. Corner vertices will be present twice- once on the upper section, once on the lower section</td>
</tr></td>
<tr>
<td>lowerEdgeVerts</td>
<td>[' ']</td>
<td>These verticies will be used to build the joint structure for the lower section. Please select a sequence of vertices along the same loop, starting from the inner corner. First and last vertices should match between the upper and lower section, representing a single closed loop. Corner vertices will be present twice- once on the lower section, once on the lower section</td>
</tr></td>
<tr>
<td>upCurveOffset</td>
<td>1.0</td>
<td>Comment wasn't inserted</td>
</tr></td>
<tr>
<td>reverseCorners</td>
<td>False</td>
<td>Offset value for the up curve generation</td>
</tr></td>
<tr>
<td>aroundCenter</td>
<td>False</td>
<td>Around center will normalize the result vectors around a given center matrix (module root in this case). This will provide a better range of motion, tranlating the joints around a sphere (assumed from the center matrix). This can be changed and animated post-construction</td>
</tr></td>
<tr>
<td>curveResolution</td>
<td>24</td>
<td>Resample curve amount</td>
</tr></td>
<tr>
<td>midCurveHeight</td>
<td>0.5</td>
<td>This dictates the height of the Mid-Meet point between the upper and lower sections</td>
</tr></td>
<tr>
<td>jawRootGuide</td>
<td></td>
<td>In case this module is used for lips (main use), input the Jaw control root guide. This will implement the Jaw control within the setup and will result in a better behaving setup</td>
</tr></td>
<tr>
<td>doAlongSurface</td>
<td>False</td>
<td>In case it is desired, an internal surface(Nurbs)-follow mechanism is built in this module. In some cases, it is desired to model a pre-existing NurbsSurface that describes the range or limits of the joints related to this module. If a valid input is insrted, the setup will be created automatically. Remember that the follow controls will be pinned to the given surface, so remember to skin the surface to parent module which will follow the world position of the guide surface. Freezing transformation on the given setup is essential for this feature to behave as expected</td>
</tr></td>
<tr>
<td>inputSurface</td>
<td></td>
<td>Input surface (Nurbs) to follow</td>
</tr></td>
<tr>
<td>doCheekRaise</td>
<td>False</td>
<td>when dealing with joint based facial deformation, and using this module as a lips setup, it is sometimes desired to incorporate another control that represents the cheek to achive a more lively deformation. Use this feature to do just that. Plug in the rootGuide of the cheeck control you wish to drive, then control the raise and push values based on your preferences or requirements</td>
</tr></td>
<tr>
<td>l_CheekRaiseRoot</td>
<td></td>
<td>Left side cheeck Root Guide</td>
</tr></td>
<tr>
<td>r_CheekRaiseRoot</td>
<td></td>
<td>Right side cheeck Root Guide</td>
</tr></td>
<tr>
<td>raiseValue</td>
<td>0.5</td>
<td>Raise default value</td>
</tr></td>
<tr>
<td>pushValue</td>
<td>0.5</td>
<td>Push-Out default value</td>
</tr></td>
<tr>
<td>doTweakControls</td>
<td>True</td>
<td>First layer tweakers</td>
</tr></td>
<tr>
<td>numTweakControlsPerSection</td>
<td>5</td>
<td>Number of tweak controls per section</td>
</tr></td>
<tr>
<td>cornersControlShape</td>
<td>triangle</td>
<td>Tweak coreners control shape</td>
</tr></td>
<tr>
<td>tweakersControlShape</td>
<td>lightSphere</td>
<td>Tweak controls shape</td>
</tr></td>
<tr>
<td>tweakCurvesInterpolation</td>
<td>4</td>
<td>First layer tweaks curve interpolation type</td>
</tr></td>
<tr>
<td>doLayerBCtrls</td>
<td>True</td>
<td>Second layer tweakers</td>
</tr></td>
<tr>
<td>numLayerBCtrlsPerSection</td>
<td>9</td>
<td>Number of tweak controls per section</td>
</tr></td>
<tr>
<td>layerBControlShape</td>
<td>cube</td>
<td>Second layer tweak controls shape</td>
</tr></td>
</table></font>
