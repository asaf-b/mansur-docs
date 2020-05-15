#Maya-Plugins
<body>
##mnsAnnotate
<hr width = 100%>
<font color = #5f5f5f size = 3pt><b>Inputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>attributes</td><td>attrs</td><td>multi</td><td>Input attributes array to display, unlimited amount. Each attribute component will be displayed as a single line.</td></tr>
<tr><td>fontSize</td><td>fontSize</td><td>float</td><td>Display Font Size.</td></tr>
<tr><td>fontColor</td><td>fontColor</td><td>float[3]</td><td>Display Font Color, RGB (0 to 1).</td></tr>
<tr><td>fontTransparency</td><td>fontTransparency</td><td>float</td><td>Font transperancy. 1 = Fully opaque, 0 = Fully tansparennt.</td></tr>
<tr><td>precision</td><td>precision</td><td>int</td><td>Numberic attribute display precision- value represents the amount of integers right to the decimal point.</td></tr>
<tr><td>lineSpacing</td><td>lineSpacing</td><td>float</td><td>Line spacing between attributes line.</td></tr>
<tr><td>drawFlat</td><td>drawFlat</td><td>int</td><td>Draw in 2D mode, regardless of the matrix position. The position is dictated by positionX and positionY attributes, relative to the viewports screen space resolution.</td></tr>
<tr><td>positionX</td><td>positionX</td><td>double</td><td>Display top-left corener X position, if drawFlat attribute is True.</td></tr>
<tr><td>positionY</td><td>positionY</td><td>double</td><td>Display top-left corener y position, if drawFlat attribute is True.</td></tr>
<tr><td>nameOnlyMode</td><td>nameOnlyMode</td><td>int</td><td>MObject	mnsAnnotate::aNameMode</td></tr>
</table></font>
<body>
##mnsBuildTransformsCurve
<hr width = 100%>
<font color = #5f5f5f size = 3pt><b>Inputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>buildMode</td><td>buildMode</td><td>enum</td><td>Build mode- EPs, CVs, Hermite, TangentedCVs, bezier.</td></tr>
<tr><td>transforms</td><td>transforms</td><td>compound</td><td>Transforms array to build the curve from.</td></tr>
<tr><td>matrix</td><td>matrix</td><td>matrix</td><td>Input matrix transform, child of transforms.</td></tr>
<tr><td>degree</td><td>degree</td><td>int</td><td>Output curve degree, 1-5.</td></tr>
<tr><td>offsetX</td><td>offsetX</td><td>float</td><td>Output offset curve X parameter.</td></tr>
<tr><td>offsetY</td><td>offsetY</td><td>float</td><td>Output offset curve Y parameter.</td></tr>
<tr><td>offsetZ</td><td>offsetZ</td><td>float</td><td>Output offset curve Z parameter.</td></tr>
<tr><td>tangentDirection</td><td>tangentDirection</td><td>enum</td><td>If build mode is on Hermite, this paremeter dictates the tangent direction.</td></tr>
<tr><td>reverse</td><td>reverse</td><td>int</td><td>Reverse output curve and offset curve.</td></tr>
<tr><td>HermiteSteps</td><td>HermiteSteps</td><td>int</td><td>Hermite mode steps amount.</td></tr>
<tr><td>tangentLength</td><td>tangentLength</td><td>float</td><td>Control tangent length (if present)</td></tr>
<tr><td>OffsetType</td><td>OffsetType</td><td>enum</td><td>Offset build type - world or local.</td></tr>
<tr><td>buildOffsetCurve</td><td>buildOffsetCurve</td><td>int</td><td>Initiate offset curve build.</td></tr>
</table></font>
<font color = #5f5f5f size = 3pt><b>Outputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>outCurve</td><td>outCurve</td><td>kNurbsCurve</td><td>Result curve shape.</td></tr>
<tr><td>outOffsetCurve</td><td>outOffsetCurve</td><td>nurbsCurve</td><td>Result offset curve shape.</td></tr>
<tr><td>length</td><td>length</td><td>double</td><td>Result curve length.</td></tr>
<tr><td>offsetLength</td><td>offsetLength</td><td>double</td><td>Result offset curve length.</td></tr>
</table></font>
<body>
##mnsCameraGateRatio
<hr width = 100%>
<font color = #5f5f5f size = 3pt><b>Inputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>cameraIn</td><td>cameraIn</td><td>message</td><td>Affected camera node.</td></tr>
<tr><td>gateWidth</td><td>gateWidth</td><td>float</td><td>Cemera gate width.</td></tr>
<tr><td>gateHeight</td><td>gateHeight</td><td>float</td><td>Cemera gate height.</td></tr>
</table></font>
<body>
##mnsCompressionTensionBlend
<hr width = 100%>
<font color = #5f5f5f size = 3pt><b>Inputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>baseMesh</td><td>baseMesh</td><td>mesh</td><td>Static base mesh input.</td></tr>
<tr><td>tensionTarget</td><td>tensionTarget</td><td>mesh</td><td>Tension blend target.</td></tr>
<tr><td>compressionTarget</td><td>compressionTarget</td><td>mesh</td><td>Compression blend target.</td></tr>
<tr><td>liveMode</td><td>liveMode</td><td>bool</td><td>Live mode. Re-calculate edge lengthes on evaluation.</td></tr>
<tr><td>displayMode</td><td>displayMode</td><td>enum</td><td>Map display mode- None, compressionTension, compression, tension.</td></tr>
<tr><td>compressionMultiplier</td><td>compressionMultiplier</td><td>float</td><td>Global compression multiplier.</td></tr>
<tr><td>tensionMultiplier</td><td>tensionMultiplier</td><td>float</td><td>Global tension multiplier.</td></tr>
</table></font>
<body>
##mnsCurveVariable
<hr width = 100%>
<font color = #5f5f5f size = 3pt><b>Inputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>curve</td><td>crv</td><td>nurbsCurve</td><td>Input curve.</td></tr>
<tr><td>upCurve</td><td>upCrv</td><td>nurbsCurve</td><td>Input offset curve.</td></tr>
<tr><td>inTransform</td><td>inTransform</td><td>compound</td><td>Input variable control values array.</td></tr>
<tr><td>uPosition</td><td>uPos</td><td>float</td><td>Input U position. Child of inTransform.</td></tr>
<tr><td>strength</td><td>strength</td><td>float</td><td>Input strength. Child of inTransform.</td></tr>
<tr><td>aimTranslate</td><td>aimT</td><td>float</td><td>Input aim translation. Child of inTransform.</td></tr>
<tr><td>upTranslate</td><td>upT</td><td>float</td><td>Input up translation. Child of inTransform.</td></tr>
<tr><td>terTranslate</td><td>terT</td><td>float</td><td>Input tertiary translation. Child of inTransform.</td></tr>
<tr><td>falloff</td><td>falloff</td><td>float</td><td>Input falloff value. Child of inTransform.</td></tr>
<tr><td>aimRotation</td><td>aimRot</td><td>angle</td><td>Input aim-rotation value. Child of inTransform.</td></tr>
<tr><td>upRotation</td><td>upRot</td><td>angle</td><td>Input up-rotation value. Child of inTransform.</td></tr>
<tr><td>tertiaryRotation</td><td>terRot</td><td>angle</td><td>Input tertiary-rotation value. Child of inTransform.</td></tr>
<tr><td>localMatrix</td><td>localMatrix</td><td>angle</td><td>Input local transformation matrix. Child of inTransform.</td></tr>
<tr><td>upMode</td><td>upMode</td><td>enum</td><td>Up mode- normal, curve, worldX, worldY, worldZ.</td></tr>
<tr><td>substeps</td><td>substeps</td><td>int</td><td>Resample substeps value.</td></tr>
<tr><td>translateMode</td><td>tMode</td><td>enum</td><td>Control translation mode- IK, FK.</td></tr>
<tr><td>degree</td><td>degree</td><td>int</td><td>Result curves degree.</td></tr>
<tr><td>buildMode</td><td>buildMode</td><td>enum</td><td>Result curve build mode- EPs, CVs.</td></tr>
<tr><td>rotateOrder</td><td>ro</td><td>enum</td><td>Calculation rotation-order.</td></tr>
<tr><td>aimAxis</td><td>aimAxis</td><td>enum</td><td>Aim axis choice.</td></tr>
<tr><td>upAxis</td><td>upAxis</td><td>enum</td><td>Up axis choice.</td></tr>
<tr><td>offsetType</td><td>offsetType</td><td>enum</td><td>Offset curve adjustment mode- local, world.</td></tr>
<tr><td>offsetX</td><td>offsetX</td><td>float</td><td>Offset curve adjustment offset X parameter.</td></tr>
<tr><td>offsetY</td><td>offsetY</td><td>float</td><td>Offset curve adjustment offset Y parameter.</td></tr>
<tr><td>offsetZ</td><td>offsetZ</td><td>float</td><td>Offset curve adjustment offset Z parameter.</td></tr>
<tr><td>uScale</td><td>uScale</td><td>float</td><td>Global U-Scale adjusment. Addative to array indevidual u inputs.</td></tr>
<tr><td>uOffset</td><td>uOffset</td><td>float</td><td>Global U-Offfset adjusment. Addative to array indevidual u inputs.</td></tr>
<tr><td>startAmp</td><td>startAmp</td><td>float</td><td>Sine start amplitude value.</td></tr>
<tr><td>endAmp</td><td>endAmp</td><td>float</td><td>Sine end amplitude value.</td></tr>
<tr><td>amplitudeAim</td><td>amplitudeAim</td><td>float</td><td>Sine calculation X direction amplitude value.</td></tr>
<tr><td>amplitudeUp</td><td>amplitudeUp</td><td>float</td><td>Sine calculation Y direction amplitude value.</td></tr>
<tr><td>amplitudeTertiary</td><td>amplitudeTertiary</td><td>float</td><td>Sine calculation Z direction amplitude value.</td></tr>
<tr><td>frequencyAim</td><td>frequencyAim</td><td>float</td><td>Sine calculation X direction frequency value.</td></tr>
<tr><td>frequencyUp</td><td>frequencyUp</td><td>float</td><td>Sine calculation Y direction frequency value.</td></tr>
<tr><td>frequencyTertiary</td><td>frequencyTertiary</td><td>float</td><td>Sine calculation Z direction frequency value.</td></tr>
<tr><td>phaseAim</td><td>phaseAim</td><td>float</td><td>Sine calculation X direction phase value.</td></tr>
<tr><td>phaseUp</td><td>phaseUp</td><td>float</td><td>Sine calculation Y direction phase value</td></tr>
<tr><td>phaseTertiary</td><td>phaseTertiary</td><td>float</td><td>Sine calculation Z direction phase value</td></tr>
<tr><td>frequency</td><td>frequency</td><td>float</td><td>Sine calculation global addative frequency value.</td></tr>
<tr><td>phase</td><td>phase</td><td>float</td><td>Sine calculation global addative phase value.</td></tr>
<tr><td>startPos</td><td>startPos</td><td>float</td><td>Sine start position value.</td></tr>
<tr><td>outCtrlsUpMode</td><td>outCtrlsUpMode</td><td>enum</td><td>Out position transforms up type - normal, curve, worldX, worldY, worldZ.</td></tr>
</table></font>
<font color = #5f5f5f size = 3pt><b>Outputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>outCurve</td><td>outCurve</td><td>nurbsCurve</td><td>Output curve shape.</td></tr>
<tr><td>outOffsetCurve</td><td>outOffsetCurve</td><td>nurbsCurve</td><td>Output offset curve shape.</td></tr>
<tr><td>outTransform</td><td>outTransform</td><td>compound</td><td>Output control offset position and rotation array.</td></tr>
<tr><td>translate</td><td>t</td><td>float[3]</td><td>Output control offset position, child of outTransform.</td></tr>
<tr><td>rotate</td><td>r</td><td>angle[3]</td><td>Output control offset rotation, child of outTransform.</td></tr>
<tr><td>rotateX</td><td>rotX</td><td>angle</td><td>Output control offset rotation, X component, child of rotate.</td></tr>
<tr><td>rotateY</td><td>rotY</td><td>angle</td><td>Output control offset rotation, Y component, child of rotate.</td></tr>
<tr><td>rotateZ</td><td>rotZ</td><td>angle</td><td>Output control offset rotation, Z component, child of rotate.</td></tr>
</table></font>
<body>
##mnsCurveZip
<hr width = 100%>
<font color = #5f5f5f size = 3pt><b>Inputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>bindCurveA</td><td>bindCurveA</td><td>nurbsCurve</td><td>Input curve A base-curve shape.</td></tr>
<tr><td>tweakCurveA</td><td>tweakCurveA</td><td>nurbsCurve</td><td>Input curve A curve shape.</td></tr>
<tr><td>bindCurveB</td><td>bindCurveB</td><td>nurbsCurve</td><td>Input curve B base-curve shape.</td></tr>
<tr><td>tweakCurveB</td><td>tweakCurveB</td><td>nurbsCurve</td><td>Input curve B curve shape.</td></tr>
<tr><td>tweakCurveABase</td><td>tweakCurveABase</td><td>nurbsCurve</td><td>Input curve A tweak base-curve shape.</td></tr>
<tr><td>tweakCurveBBase</td><td>tweakCurveBBase</td><td>nurbsCurve</td><td>Input curve B tweak base-curve shape.</td></tr>
<tr><td>midCurve</td><td>midCrv</td><td>nurbsCurve</td><td>Input target mid curve.</td></tr>
<tr><td>centerMatrix</td><td>centerMatrix</td><td>matrix</td><td>Input center transformation matrix.</td></tr>
<tr><td>midPointMatrix</td><td>midPointMatrix</td><td>matrix</td><td>Input mid point traget matrix.</td></tr>
<tr><td>sampleMode</td><td>m</td><td>enum</td><td>Curve sample mode- parametric, uniform.</td></tr>
<tr><td>matchInputCurve</td><td>matchInputCurve</td><td>enum</td><td>Result curve matched parameters to- none, curveA, curveB.</td></tr>
<tr><td>substeps</td><td>substeps</td><td>int</td><td>Result curve resampling sub-step value.</td></tr>
<tr><td>degree</td><td>degree</td><td>int</td><td>Result curve degree value.</td></tr>
<tr><td>buildMode</td><td>buildMode</td><td>enum</td><td>Curve build mode- EPs, CVs.</td></tr>
<tr><td>midGenerateFrom</td><td>midGenerateFrom</td><td>enum</td><td>Generate automatic mid curve from- bindBases, tweakCurves, input.</td></tr>
<tr><td>midBias</td><td>midBias</td><td>float</td><td>Generated curve bias.</td></tr>
<tr><td>aroundCenter</td><td>aroundCenter</td><td>bool</td><td>Calculate results considering the input center matrix.</td></tr>
<tr><td>conformToMeetPoint</td><td>conformToMeetPoint</td><td>bool</td><td>Conform the selected curve result to meet the oter curve based on set parameters.</td></tr>
<tr><td>curveToConform</td><td>curveToConform</td><td>enum</td><td>Which curve to conform - curveA, curveB.</td></tr>
<tr><td>conformDistancethreshold</td><td>conformDistancethreshold</td><td>enum</td><td>Which curve to conform - curveA, curveB.</td></tr>
<tr><td>AToMid</td><td>AToMid</td><td>float</td><td>Blend curve A to mid-curve.</td></tr>
<tr><td>BToMid</td><td>BToMid</td><td>float</td><td>Blend curve B to mid-curve.</td></tr>
<tr><td>AToB</td><td>AToB</td><td>float</td><td>Blend curve A to curve B.</td></tr>
<tr><td>BToA</td><td>BToA</td><td>float</td><td>Blend curve B to curve A.</td></tr>
<tr><td>allToMidPoint</td><td>allToMidPoint</td><td>float</td><td>Blend both curves to mid-curve.</td></tr>
<tr><td>pushOut</td><td>pushOut</td><td>float</td><td>Curves push-out added value.</td></tr>
<tr><td>zipStart</td><td>zipStart</td><td>float</td><td>Zip start value.</td></tr>
<tr><td>zipStartFalloff</td><td>zipStartFalloff</td><td>float</td><td>Zip start falloff value.</td></tr>
<tr><td>zipEnd</td><td>zipEnd</td><td>float</td><td>Zip end value.</td></tr>
<tr><td>zipEndFalloff</td><td>zipEndFalloff</td><td>float</td><td>Zip end falloff value.</td></tr>
<tr><td>glue</td><td>glue</td><td>bool</td><td>Do glue.</td></tr>
<tr><td>glueTherhold</td><td>glueTherhold</td><td>float</td><td>Glue threshold value.</td></tr>
<tr><td>offsetBase</td><td>offsetBase</td><td>enum</td><td>Offset curve build mode. centerMatrix, worldX, worldY, worldZ.</td></tr>
<tr><td>offset</td><td>offset</td><td>float</td><td>Offset curve build parameter.</td></tr>
<tr><td>globalMultiplier</td><td>globalMultiplier</td><td>float</td><td>Global value multiplier.</td></tr>
</table></font>
<font color = #5f5f5f size = 3pt><b>Outputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>outCurveA</td><td>outCurveA</td><td>nurbsCurve</td><td>Result curve A shape.</td></tr>
<tr><td>outCurveB</td><td>outCurveB</td><td>nurbsCurve</td><td>Result curve B shape.</td></tr>
<tr><td>outCurveAOffset</td><td>outCurveAOffset</td><td>nurbsCurve</td><td>Result curve A offset shape.</td></tr>
<tr><td>outCurveBOffset</td><td>outCurveBOffset</td><td>nurbsCurve</td><td>Result curve B offset shape.</td></tr>
</table></font>
<body>
##mnsIKSolver
<hr width = 100%>
<font color = #5f5f5f size = 3pt><b>Inputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>boneLengthA</td><td>bla</td><td>float</td><td>Base length A.</td></tr>
<tr><td>boneLengthB</td><td>blb</td><td>float</td><td>Base length B.</td></tr>
<tr><td>blend</td><td>blend</td><td>float</td><td>IK-FK blend value.</td></tr>
<tr><td>rootFK</td><td>rootFK</td><td>matrix</td><td>Input FK root matrix.</td></tr>
<tr><td>midFK</td><td>midFK</td><td>matrix</td><td>Input FK mid matrix.</td></tr>
<tr><td>endFK</td><td>endFK</td><td>matrix</td><td>Input FK end matrix.</td></tr>
<tr><td>ikTarget</td><td>ikTarget</td><td>matrix</td><td>Input IK target matrix.</td></tr>
<tr><td>poleVector</td><td>poleVector</td><td>matrix</td><td>Input pole-vector target matrix.</td></tr>
<tr><td>rootWorldMatrix</td><td>rootWorldMatrix</td><td>matrix</td><td>Module root input matrix.</td></tr>
<tr><td>roll</td><td>roll</td><td>float</td><td>IK addative roll value.</td></tr>
<tr><td>slide</td><td>slide</td><td>float</td><td>IK mid slide value.</td></tr>
<tr><td>softness</td><td>softness</td><td>float</td><td>IK softness parameter.</td></tr>
<tr><td>stretchLimit</td><td>stretchLimit</td><td>float</td><td>IK stretch limit value. 1 is no stretch, 2 is double the length.</td></tr>
<tr><td>aimAxis</td><td>aimAxis</td><td>enum</td><td>Aim axis choice.</td></tr>
<tr><td>upAxis</td><td>upAxis</td><td>enum</td><td>Up axis choice.</td></tr>
</table></font>
<font color = #5f5f5f size = 3pt><b>Outputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>rootTranslate</td><td>rootTranslate</td><td>float[3]</td><td>Root out translate output. Child of outRoot.</td></tr>
<tr><td>rootRotateX</td><td>rootRotateX</td><td>float</td><td>Root out translate X output. Child of outRoot.</td></tr>
<tr><td>rootRotateY</td><td>rootRotateY</td><td>float</td><td>Root out translate Y output. Child of outRoot.</td></tr>
<tr><td>rootRotateZ</td><td>rootRotateZ</td><td>float</td><td>Root out translate Z output. Child of outRoot.</td></tr>
<tr><td>rootRotate</td><td>rootRotate</td><td>angle[3]</td><td>Root out rotate output. Child of outRoot.</td></tr>
<tr><td>rootScale</td><td>rootScale</td><td>float[3]</td><td>Root out scale output. Child of outRoot.</td></tr>
<tr><td>outRoot</td><td>outRoot</td><td>compound</td><td>Root output transformation values.</td></tr>
<tr><td>midTranslate</td><td>midTranslate</td><td>float[3]</td><td>Mid out translate output. Child of outMid.</td></tr>
<tr><td>midRotateX</td><td>midRotateX</td><td>float</td><td>Mid out translate X output. Child of outMid.</td></tr>
<tr><td>midRotateY</td><td>midRotateY</td><td>float</td><td>Mid out translate Y output. Child of outMid.</td></tr>
<tr><td>midRotateZ</td><td>midRotateZ</td><td>float</td><td>Mid out translate Z output. Child of outMid.</td></tr>
<tr><td>midRotate</td><td>midRotate</td><td>angle[3]</td><td>Mid out rotate output. Child of outMid.</td></tr>
<tr><td>midScale</td><td>midScale</td><td>float[3]</td><td>Mid out scale output. Child of outMid.</td></tr>
<tr><td>outMid</td><td>outMid</td><td>compound</td><td>Mid output transformation values.</td></tr>
<tr><td>endTranslate</td><td>endTranslate</td><td>float[3]</td><td>End out translate output. Child of outEnd.</td></tr>
<tr><td>endRotateX</td><td>endRotateX</td><td>float</td><td>End out translate X output. Child of outEnd.</td></tr>
<tr><td>endRotateY</td><td>endRotateY</td><td>float</td><td>End out translate Y output. Child of outEnd.</td></tr>
<tr><td>endRotateZ</td><td>endRotateZ</td><td>float</td><td>End out translate Z output. Child of outEnd.</td></tr>
<tr><td>endRotate</td><td>endRotate</td><td>angle[3]</td><td>End out rotate output. Child of outEnd.</td></tr>
<tr><td>endScale</td><td>endScale</td><td>float[3]</td><td>End out scale output. Child of outEnd.</td></tr>
<tr><td>outEnd</td><td>outEnd</td><td>compound</td><td>End output transformation values.</td></tr>
<tr><td>ikVis</td><td>ikVis</td><td>bool</td><td>IK mode visibility.</td></tr>
<tr><td>fkVis</td><td>fkVis</td><td>bool</td><td>FK mode visibility.</td></tr>
</table></font>
<body>
##mnsMatrixConstraint
<hr width = 100%>
<body>
##mnsMeshRivets
<hr width = 100%>
<body>
##mnsMeshSeparate
<hr width = 100%>
<body>
##mnsNodeRelationship
<hr width = 100%>
<body>
##mnsPointsOnCurve
<hr width = 100%>
<body>
##mnsResampleCurve
<hr width = 100%>
<body>
##mnsSphereVectorPush
<hr width = 100%>
<body>
##mnsSpringCurve
<hr width = 100%>
<body>
##mnsThreePointArc
<hr width = 100%>
