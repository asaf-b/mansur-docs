<body>
#FKChain Settings
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
Author: Asaf Ben Zur <br>
</i>
<br>
</font>
<hr width = 100%>
##Attributes
</table></font>
###GlobalSettings
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>doInterpolationJoints</td>
<td>False</td>
<td>Create interpolation joints for this module</td></tr>
<tr><td>interpolationJoints</td>
<td>2</td>
<td>Amount of interpolation joints</td></tr>
<tr><td>isolatePolesRotation</td>
<td>False</td>
<td>If this is set to True, the first and last interpolation joints orientation will be isolated. This is primarily used in combination with the EmbeddedIK feature to achive a stable spine setup</td></tr>
<tr><td>offsetX</td>
<td>20.0</td>
<td>Up curve X value offset for the interpolation joints</td></tr>
<tr><td>offsetZ</td>
<td>0.0</td>
<td>Up curve Z value offset for the interpolation joints</td></tr>
<tr><td>scaleMode</td>
<td>2</td>
<td>Default scale mode. Please refer to the documentation of mnsPointsOnCurve node to learn more about each mode</td></tr>
<tr><td>squashMode</td>
<td>0</td>
<td>Default squash mode. Please refer to the documentation of mnsPointsOnCurve node to learn more about each mode</td></tr>
<tr><td>doIntepJntsSpring</td>
<td>False</td>
<td>If this is set to True, a mnsSpringCurve node will be created on top of the primary curve controling the interpolation joints</td></tr>
</table></font>
###FK
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>FKcontrolShape</td>
<td>circle</td>
<td>FK controls shape</td></tr>
<tr><td>doFKSeconderyIK</td>
<td>False</td>
<td>If this is set to True, another level of IK controls will be created below the FK controls</td></tr>
<tr><td>FKSecondaryIKControlShape</td>
<td>diamond</td>
<td>Secodary IK controls shape</td></tr>
<tr><td>primaryCurveDegree</td>
<td>3</td>
<td>Primary interpolation joints curve generation degree. Please refer to the documentation of mnsBuildTransformsCurve node to learn more about curve generation degree</td></tr>
<tr><td>primaryCurveMode</td>
<td>0</td>
<td>Primary interpolation joints curve sampling mode. Please refer to the documentation of mnsPointsOnCurve node to learn more about curve each mode</td></tr>
<tr><td>primaryInterpolaion</td>
<td>0</td>
<td>Primary interpolation joints curve generation interpolation mode. Please refer to the documentation of mnsBuildTransformsCurve node to learn more about each mode</td></tr>
<tr><td>FKChannelControl</td>
<td>
<font size = 2pt>
<table><tr><td style="padding:6px"></td>
<td style="padding:6px"><b>T</b></td>
<td style="padding:6px"><b>R</b></td>
<td style="padding:6px"><b>S</b></td>
</tr>
<tr><td style="padding:6px"><b>X</b></td>
<td style="padding:6px">v</td>
<td style="padding:6px">v</td>
<td style="padding:6px">v</td>
</tr>
<tr><td style="padding:6px"><b>Y</b></td>
<td style="padding:6px">v</td>
<td style="padding:6px">v</td>
<td style="padding:6px">v</td>
</tr>
<tr><td style="padding:6px"><b>Z</b></td>
<td style="padding:6px">v</td>
<td style="padding:6px">v</td>
<td style="padding:6px">v</td>
</tr>
</table>
</font>
</td>
<td>FK controls channel-box settings</td></tr>
</table></font>
###EmbeddedIK
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>doEmbeddedIK</td>
<td>False</td>
<td>This feature is mainly used to create a spine setup, where another layer of IK control is needed. The result of this feature is three IK controls - Root, Mid and End controls, which will allow IK control over the entire chain</td></tr>
<tr><td>defaultVisibilityMode</td>
<td>1</td>
<td>Default visibility settings. FK and IK main controls can be used in combination, or indevidually- hence a manuall visibility switch</td></tr>
<tr><td>embIKCurveDegree</td>
<td>3</td>
<td>Embedded IK curve degree. Please refer to the documentation of mnsBuildTransformsCurve node to learn more about curve generation degree</td></tr>
<tr><td>doMidTangentCtrls</td>
<td>True</td>
<td>If this is set to True, two extra tangent controls will be build from the IK Mid control</td></tr>
<tr><td>embIKControlShape</td>
<td>flatDiamond</td>
<td>Main shape for the embedded IK controls</td></tr>
<tr><td>embIKChannelControl</td>
<td>
<font size = 2pt>
<table><tr><td style="padding:6px"></td>
<td style="padding:6px"><b>T</b></td>
<td style="padding:6px"><b>R</b></td>
<td style="padding:6px"><b>S</b></td>
</tr>
<tr><td style="padding:6px"><b>X</b></td>
<td style="padding:6px">v</td>
<td style="padding:6px">v</td>
<td style="padding:6px">v</td>
</tr>
<tr><td style="padding:6px"><b>Y</b></td>
<td style="padding:6px">v</td>
<td style="padding:6px">v</td>
<td style="padding:6px">v</td>
</tr>
<tr><td style="padding:6px"><b>Z</b></td>
<td style="padding:6px">v</td>
<td style="padding:6px">v</td>
<td style="padding:6px">v</td>
</tr>
</table>
</font>
</td>
<td>Embedded IK controls channel-box settings</td></tr>
</table></font>
###IK_Secondaries
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>doSecondaryIKCtrls</td>
<td>False</td>
<td>This feature will create a secondary IK controls layer below the primary FK chain controls</td></tr>
<tr><td>numIKControls</td>
<td>2</td>
<td>Amount of secondary layer controls</td></tr>
<tr><td>isolateSecPolesRotation</td>
<td>False</td>
<td>If this is set to True, the first and last controls orientation will be isolated. T</td></tr>
<tr><td>IKControlShape</td>
<td>dial</td>
<td>Secondary IK layer control shape</td></tr>
<tr><td>secondaryCurveDegree</td>
<td>3</td>
<td>Secondary IK curve generation degree. Please refer to the documentation of mnsBuildTransformsCurve node to learn more about curve generation degree</td></tr>
<tr><td>secondaryCurveMode</td>
<td>0</td>
<td>Secondary IK curve sampling mode. Please refer to the documentation of mnsPointsOnCurve node to learn more about curve each mode</td></tr>
<tr><td>secondaryInterpolaion</td>
<td>0</td>
<td>Secondary IK curve generation interpolation mode. Please refer to the documentation of mnsBuildTransformsCurve node to learn more about each mode</td></tr>
<tr><td>doIKSpring</td>
<td>False</td>
<td>If this is set to True, a mnsSpringCurve node will be created on top of the secondary curve</td></tr>
<tr><td>IKChannelControl</td>
<td>
<font size = 2pt>
<table><tr><td style="padding:6px"></td>
<td style="padding:6px"><b>T</b></td>
<td style="padding:6px"><b>R</b></td>
<td style="padding:6px"><b>S</b></td>
</tr>
<tr><td style="padding:6px"><b>X</b></td>
<td style="padding:6px">v</td>
<td style="padding:6px">v</td>
<td style="padding:6px">v</td>
</tr>
<tr><td style="padding:6px"><b>Y</b></td>
<td style="padding:6px">v</td>
<td style="padding:6px">v</td>
<td style="padding:6px">v</td>
</tr>
<tr><td style="padding:6px"><b>Z</b></td>
<td style="padding:6px">v</td>
<td style="padding:6px">v</td>
<td style="padding:6px">v</td>
</tr>
</table>
</font>
</td>
<td>Secondary IK controls channel-box settings</td></tr>
</table></font>
###VariableFK
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>doVariableFK</td>
<td>False</td>
<td>This will create a veriable FK setup on this chain</td></tr>
<tr><td>numVarFKControls</td>
<td>2</td>
<td>Number of variable FK controls</td></tr>
<tr><td>varFKControlShape</td>
<td>pinchedCircle</td>
<td>Variable FK control shape</td></tr>
<tr><td>varFKDegree</td>
<td>3</td>
<td>Variable FK curve degree. Please refer to the documentation of mnsBuildTransformsCurve node to learn more about curve generation degree</td></tr>
<tr><td>defaultFalloff</td>
<td>0.5</td>
<td>Default falloff value for the variable FK controls</td></tr>
<tr><td>varFKSubsteps</td>
<td>20</td>
<td>The variable FK setup is able to re-sample the curve to any amount of control points to refine the fidelity of the setup. This is the default sampling value</td></tr>
<tr><td>doVarFKSpring</td>
<td>False</td>
<td>If this is set to True, a mnsSpringCurve node will be created on top of the variable FK controls</td></tr>
<tr><td>varFKChannelControl</td>
<td>
<font size = 2pt>
<table><tr><td style="padding:6px"></td>
<td style="padding:6px"><b>T</b></td>
<td style="padding:6px"><b>R</b></td>
<td style="padding:6px"><b>S</b></td>
</tr>
<tr><td style="padding:6px"><b>X</b></td>
<td style="padding:6px">v</td>
<td style="padding:6px">v</td>
<td style="padding:6px"></td>
</tr>
<tr><td style="padding:6px"><b>Y</b></td>
<td style="padding:6px">v</td>
<td style="padding:6px">v</td>
<td style="padding:6px"></td>
</tr>
<tr><td style="padding:6px"><b>Z</b></td>
<td style="padding:6px">v</td>
<td style="padding:6px">v</td>
<td style="padding:6px"></td>
</tr>
</table>
</font>
</td>
<td>Variable FK controls channel-box settings</td></tr>
</table></font>
###Tweakers
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>doTweakControls</td>
<td>False</td>
<td>This feature is a global extra layer to tweak the final result cuvre samples rotation and scale.</td></tr>
<tr><td>numTweakers</td>
<td>2</td>
<td>Number of tweak controls to create</td></tr>
<tr><td>tweakControlShape</td>
<td>dialSquare</td>
<td>Tweak controls shape</td></tr>
<tr><td>tweakersChannelControl</td>
<td>
<font size = 2pt>
<table><tr><td style="padding:6px"></td>
<td style="padding:6px"><b>T</b></td>
<td style="padding:6px"><b>R</b></td>
<td style="padding:6px"><b>S</b></td>
</tr>
<tr><td style="padding:6px"><b>X</b></td>
<td style="padding:6px"></td>
<td style="padding:6px">v</td>
<td style="padding:6px">v</td>
</tr>
<tr><td style="padding:6px"><b>Y</b></td>
<td style="padding:6px"></td>
<td style="padding:6px">v</td>
<td style="padding:6px">v</td>
</tr>
<tr><td style="padding:6px"><b>Z</b></td>
<td style="padding:6px"></td>
<td style="padding:6px">v</td>
<td style="padding:6px">v</td>
</tr>
</table>
</font>
</td>
<td>Tweak controls channel-box settings</td></tr>
</table></font>
