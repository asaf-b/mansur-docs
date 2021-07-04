<body>
#curveZipB Settings
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
Author: Asaf Ben-Zur <br>
Best used for: Eyelids, Eyelashes <br>
This facial module was created to allow adavnced control over eyelids and eyelashes. <br>
Based on settings, this module will create a very flexible control over eyelids, and if choosen (Attachment Curves) to eyelashes on top of the eyelids as well. <br>
The main features of this modules are: Joint positions based on a center matrix (Around the eye), Blink controls, Blink height control, Eyelid tweak controls (dynamic), Zip controls, and much more. <br>
The joint structure of this module will be dictated by input vertices on a given mesh. <br>
Note: Please select upper and lower vertices along a single closed loop, selecting each section from inner corener to outer corenr. <br>
</i>
<br>
</font>
<hr width = 100%>
##Attributes
</table></font>
###GlobalSettings
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>upperEdgeVerts</td>
<td>[' ']</td>
<td>These verticies will be used to build the joint structure for the upper section. Please select a sequence of vertices along the same loop, starting from the inner corner. First and last vertices should match between the upper and lower section, representing a single closed loop. Corner vertices will be present twice- once on the upper section, once on the lower section</td></tr>
<tr><td>lowerEdgeVerts</td>
<td>[' ']</td>
<td>These verticies will be used to build the joint structure for the lower section. Please select a sequence of vertices along the same loop, starting from the inner corner. First and last vertices should match between the upper and lower section, representing a single closed loop. Corner vertices will be present twice- once on the upper section, once on the lower section</td></tr>
<tr><td>upCurveOffset</td>
<td>1.0</td>
<td>Offset value for the up curve generation</td></tr>
<tr><td>reverseCorners</td>
<td>False</td>
<td>In case you build this module and the zip controls aren't matching their corner (possibly due to a wrong order of vertex selection), set this attribute to True, which should correct the mismatch</td></tr>
<tr><td>reverseRightBindCurves</td>
<td>False</td>
<td>In some symmetry cases, the right side curves are reversed. You will know if that is the case when rotating the upper or lower main eyelid controls, which will result in a reversed bahviour. If that is the case, check this attribute on.</td></tr>
<tr><td>aroundCenter</td>
<td>True</td>
<td>Around center will normalize the result vectors around a given center matrix (module root in this case). This will provide a better range of motion, tranlating the joints around a sphere (assumed from the center matrix). Place your roog guide at the center of the eye (for example) for this to behave as expected</td></tr>
<tr><td>curveResolution</td>
<td>24</td>
<td>Resample curve amount</td></tr>
<tr><td>midCurveMode</td>
<td>1</td>
<td>Mid curve generation mode</td></tr>
<tr><td>midCurveResolution</td>
<td>5</td>
<td>Mid curve generation sampling amount</td></tr>
<tr><td>blinkHeight</td>
<td>0.5</td>
<td>Default value for the Blink height. This dictates the height of the Mid-Meet point between the upper and lower sections</td></tr>
<tr><td>postSymmetryJntStruct</td>
<td>True</td>
<td>Comment wasn't inserted</td></tr>
</table></font>
###EyelidsControls
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>raiseRange</td>
<td>0.5</td>
<td>This value dictates the upper and lower controls opposite direction movement range.</td></tr>
<tr><td>uiCtrlsScale</td>
<td>0.15</td>
<td>Scale multiplier for the remote control style controls for upper and lower lids</td></tr>
<tr><td>uiCtrlsPositionOffset</td>
<td>0.5</td>
<td>Offset value (Pointing away from the root guide) to offset the remote control style controls</td></tr>
<tr><td>doZipControls</td>
<td>True</td>
<td>Create the Zip controls feature</td></tr>
</table></font>
###TweakCcontrols
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>doTweakControls</td>
<td>True</td>
<td>Build the tweak controls feature for this module</td></tr>
<tr><td>numTweakControlsPerSection</td>
<td>3</td>
<td>The amount of tweak controls per section (lower and upper)</td></tr>
<tr><td>cornersControlShape</td>
<td>diamond</td>
<td>Tweak corners controls shape</td></tr>
<tr><td>tweakersControlShape</td>
<td>lightSphere</td>
<td>Tweak controls shape</td></tr>
<tr><td>tweakCurvesInterpolation</td>
<td>1</td>
<td>Tweak controls interpolation type</td></tr>
<tr><td>flipRightX</td>
<td>False</td>
<td>Comment wasn't inserted</td></tr>
<tr><td>flipRightY</td>
<td>False</td>
<td>Comment wasn't inserted</td></tr>
<tr><td>flipRightZ</td>
<td>False</td>
<td>Comment wasn't inserted</td></tr>
</table></font>
###FollowRotation
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>doFollowRotation</td>
<td>False</td>
<td>This feture is mainly used for eye configurations. Follow rotation will create a new layer of orientation control, allowing the animator th choose the amount follow desired based on the given eye module input. This is commonly known as Fleshy-Eye</td></tr>
<tr><td>jntToFollow</td>
<td></td>
<td>The joint orientation to follow</td></tr>
<tr><td>horizontalFollow</td>
<td>0.05</td>
<td>Horizontal follow default value</td></tr>
<tr><td>verticalFollow</td>
<td>0.1</td>
<td>Vertical follow default value</td></tr>
</table></font>
###UpperAttachmentCrv
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>doUpperAttachment</td>
<td>False</td>
<td>This feature is mainly used to create another layer of controls for eyelashes. Since eyelashes should always follow the eyelids outline shape, common tendency is to simply skin them to the eyelid joints. Although in some cases, eyelashes control is required or desired. This feature will create a slave curve based controls layer that will allow for eyelash control, on top of the master eyelid solve that drives the main animation</td></tr>
<tr><td>upperJntCount</td>
<td>2</td>
<td>The amount of upper-attachment joints to create</td></tr>
</table></font>
###LowerAttachmentCrv
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>doLowerAttachment</td>
<td>False</td>
<td>This feature is mainly used to create another layer of controls for eyelashes. Since eyelashes should always follow the eyelids outline shape, common tendency is to simply skin them to the eyelid joints. Although in some cases, eyelashes control is required or desired. This feature will create a slave curve based controls layer that will allow for eyelash control, on top of the master eyelid solve that drives the main animation</td></tr>
<tr><td>lowerJntCount</td>
<td>2</td>
<td>The amount of lower-attachment joints to create</td></tr>
</table></font>
