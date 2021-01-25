<body>
#FKChain Settings
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
test header is this just a text <br>
another line here <br>
</i>
<br>
</font>
<hr width = 100%>
##Attributes
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr>
<td>doInterpolationJoints</td>
<td>False</td>
<td>Create interpolation joints for this module</td>
</tr></td>
<tr>
<td>interpolationJoints</td>
<td>2</td>
<td>Amount of interpolation joints</td>
</tr></td>
<tr>
<td>isolatePolesRotation</td>
<td>False</td>
<td>If this is set to True, the first and last interpolation joints orientation will be isolated. This is primarily used in combination with the EmbeddedIK feature to achive a stable spine setup</td>
</tr></td>
<tr>
<td>offsetX</td>
<td>20.0</td>
<td>Up curve X value offset for the interpolation joints</td>
</tr></td>
<tr>
<td>offsetZ</td>
<td>0.0</td>
<td>Up curve Z value offset for the interpolation joints</td>
</tr></td>
<tr>
<td>scaleMode</td>
<td>2</td>
<td>Default scale mode. Please refer to the documentation of mnsPointsOnCurve node to learn more about each mode</td>
</tr></td>
<tr>
<td>squashMode</td>
<td>0</td>
<td>Default squash mode. Please refer to the documentation of mnsPointsOnCurve node to learn more about each mode</td>
</tr></td>
<tr>
<td>doIntepJntsSpring</td>
<td>False</td>
<td>If this is set to True, a mnsSpringCurve node will be created on top of the primary curve controling the interpolation joints</td>
</tr></td>
<tr>
<td>FKcontrolShape</td>
<td>circle</td>
<td>FK controls shape</td>
</tr></td>
<tr>
<td>doFKSeconderyIK</td>
<td>False</td>
<td>If this is set to True, another level of IK controls will be created below the FK controls</td>
</tr></td>
<tr>
<td>FKSecondaryIKControlShape</td>
<td>diamond</td>
<td>Secodary IK controls shape</td>
</tr></td>
<tr>
<td>primaryCurveDegree</td>
<td>3</td>
<td>Primary interpolation joints curve generation degree. Please refer to the documentation of mnsBuildTransformsCurve node to learn more about curve generation degree</td>
</tr></td>
<tr>
<td>primaryCurveMode</td>
<td>0</td>
<td>Primary interpolation joints curve sampling mode. Please refer to the documentation of mnsPointsOnCurve node to learn more about curve each mode</td>
</tr></td>
<tr>
<td>primaryInterpolaion</td>
<td>0</td>
<td>Primary interpolation joints curve generation interpolation mode. Please refer to the documentation of mnsBuildTransformsCurve node to learn more about each mode</td>
</tr></td>
<tr>
<td>FKChannelControl</td>
<td>{'s': (True, True, True), 'r': (True, True, True), 't': (True, True, True)}</td>
<td>FK controls channel-box settings</td>
</tr></td>
<tr>
<td>doEmbeddedIK</td>
<td>False</td>
<td>This feature is mainly used to create a spine setup, where another layer of IK control is needed. The result of this feature is three IK controls - Root, Mid and End controls, which will allow IK control over the entire chain</td>
</tr></td>
<tr>
<td>defaultVisibilityMode</td>
<td>1</td>
<td>Default visibility settings. FK and IK main controls can be used in combination, or indevidually- hence a manuall visibility switch</td>
</tr></td>
<tr>
<td>embIKCurveDegree</td>
<td>3</td>
<td>Embedded IK curve degree. Please refer to the documentation of mnsBuildTransformsCurve node to learn more about curve generation degree</td>
</tr></td>
<tr>
<td>doMidTangentCtrls</td>
<td>True</td>
<td>If this is set to True, two extra tangent controls will be build from the IK Mid control</td>
</tr></td>
<tr>
<td>embIKControlShape</td>
<td>flatDiamond</td>
<td>Main shape for the embedded IK controls</td>
</tr></td>
<tr>
<td>embIKChannelControl</td>
<td>{'s': (True, True, True), 'r': (True, True, True), 't': (True, True, True)}</td>
<td>Embedded IK controls channel-box settings</td>
</tr></td>
<tr>
<td>doSecondaryIKCtrls</td>
<td>False</td>
<td>This feature will create a secondary IK controls layer below the primary FK chain controls</td>
</tr></td>
<tr>
<td>numIKControls</td>
<td>2</td>
<td>Amount of secondary layer controls</td>
</tr></td>
<tr>
<td>isolateSecPolesRotation</td>
<td>False</td>
<td>If this is set to True, the first and last controls orientation will be isolated. T</td>
</tr></td>
<tr>
<td>IKControlShape</td>
<td>dial</td>
<td>Secondary IK layer control shape</td>
</tr></td>
<tr>
<td>secondaryCurveDegree</td>
<td>3</td>
<td>Secondary IK curve generation degree. Please refer to the documentation of mnsBuildTransformsCurve node to learn more about curve generation degree</td>
</tr></td>
<tr>
<td>secondaryCurveMode</td>
<td>0</td>
<td>Secondary IK curve sampling mode. Please refer to the documentation of mnsPointsOnCurve node to learn more about curve each mode</td>
</tr></td>
<tr>
<td>secondaryInterpolaion</td>
<td>0</td>
<td>Secondary IK curve generation interpolation mode. Please refer to the documentation of mnsBuildTransformsCurve node to learn more about each mode</td>
</tr></td>
<tr>
<td>doIKSpring</td>
<td>False</td>
<td>If this is set to True, a mnsSpringCurve node will be created on top of the secondary curve</td>
</tr></td>
<tr>
<td>IKChannelControl</td>
<td>{'s': (True, True, True), 'r': (True, True, True), 't': (True, True, True)}</td>
<td>Secondary IK controls channel-box settings</td>
</tr></td>
<tr>
<td>doVariableFK</td>
<td>False</td>
<td>This will create a veriable FK setup on this chain</td>
</tr></td>
<tr>
<td>numVarFKControls</td>
<td>2</td>
<td>Number of variable FK controls</td>
</tr></td>
<tr>
<td>varFKControlShape</td>
<td>pinchedCircle</td>
<td>Variable FK control shape</td>
</tr></td>
<tr>
<td>varFKDegree</td>
<td>3</td>
<td>Variable FK curve degree. Please refer to the documentation of mnsBuildTransformsCurve node to learn more about curve generation degree</td>
</tr></td>
<tr>
<td>defaultFalloff</td>
<td>0.5</td>
<td>Default falloff value for the variable FK controls</td>
</tr></td>
<tr>
<td>varFKSubsteps</td>
<td>20</td>
<td>The variable FK setup is able to re-sample the curve to any amount of control points to refine the fidelity of the setup. This is the default sampling value</td>
</tr></td>
<tr>
<td>doVarFKSpring</td>
<td>False</td>
<td>If this is set to True, a mnsSpringCurve node will be created on top of the variable FK controls</td>
</tr></td>
<tr>
<td>varFKChannelControl</td>
<td>{'s': (False, False, False), 'r': (True, True, True), 't': (True, True, True)}</td>
<td>Variable FK controls channel-box settings</td>
</tr></td>
<tr>
<td>doTweakControls</td>
<td>False</td>
<td>This feature is a global extra layer to tweak the final result cuvre samples rotation and scale.</td>
</tr></td>
<tr>
<td>numTweakers</td>
<td>2</td>
<td>Number of tweak controls to create</td>
</tr></td>
<tr>
<td>tweakControlShape</td>
<td>dialSquare</td>
<td>Tweak controls shape</td>
</tr></td>
<tr>
<td>tweakersChannelControl</td>
<td>{'s': (True, True, True), 'r': (True, True, True), 't': (False, False, False)}</td>
<td>Tweak controls channel-box settings</td>
</tr></td>
</table></font>
