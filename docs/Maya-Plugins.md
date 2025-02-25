#Maya-Plugins
<body>
##mnsAnnotate
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur ===
<br>
This node is a utility node used to present value annotations in maya's viewport easily.
<br>
When needing to present any keyframed values in a playblast within maya, there isn't any maya native node to allow values display within the VP.
<br>
This node was created for this need.
<br>
All connected attributes will be displayed as a new line presenting attributes and their current values, updating in real time.
<br>
The display settings are controled within this node, where the position of the display is controlled via the custom locator created with it.
<br>
The amount of attribute display is unlimited, and multiple unlimited instances of this node can be created freely.
<br>
This is mainly used to display technicall setups.
<br>
</i></font>
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
##mnsAutoWheelDrive
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur ===
<br>
</i></font>
<hr width = 100%>
<font color = #5f5f5f size = 3pt><b>Inputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>startFrame</td><td>startFrame</td><td>int</td><td>Evaluation start frame.</td></tr>
<tr><td>startFrameFromRange</td><td>startFrameFromRange</td><td>bool</td><td>If true, take the start frame from current maya range instead of the input value given.</td></tr>
<tr><td>time</td><td>time</td><td>time</td><td>Time input.</td></tr>
</table></font>
<body>
##mnsBuildTransformsCurve
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur ===
<br>
This node builds a nurbsCurve shape, based on input transforms array.
<br>
The curve parameters are dictated by this node's attributes, and can be dynamiclly changed and even keyframed if needed.
<br>
This node also creates and offset curve shape result, to be used later as an Up-Vector for every single arbitrary point along the result main curve.
<br>
</i></font>
<hr width = 100%>
<font color = #5f5f5f size = 3pt><b>Inputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>globalScale</td><td>globalScale</td><td>float</td><td>Global scale multiplier.</td></tr>
<tr><td>tweakCurve</td><td>tweakCurve</td><td>nurbsCurve</td><td>Input tweak curve shape.</td></tr>
<tr><td>tweakCurveBase</td><td>tweakCurveBase</td><td>nurbsCurve</td><td>Input tweak curve base shape.</td></tr>
<tr><td>buildMode</td><td>buildMode</td><td>enum</td><td>Build mode- EPs, CVs, Hermite, TangentedCVs, bezier.</td></tr>
<tr><td>transforms</td><td>transforms</td><td>compound</td><td>Transforms array to build the curve from.</td></tr>
<tr><td>matrix</td><td>matrix</td><td>matrix</td><td>Input matrix transform, child of transforms. If this plug is connected, offsetX value will be taken as an the offset amount.</td></tr>
<tr><td>offsetBaseMatrix</td><td>offsetBaseMatrix</td><td>matrix</td><td>Matrix to build offset vectors from</td></tr>
<tr><td>degree</td><td>degree</td><td>int</td><td>Output curve degree, 1-5.</td></tr>
<tr><td>offsetX</td><td>offsetX</td><td>float</td><td>Output offset curve X parameter.</td></tr>
<tr><td>offsetY</td><td>offsetY</td><td>float</td><td>Output offset curve Y parameter.</td></tr>
<tr><td>offsetZ</td><td>offsetZ</td><td>float</td><td>Output offset curve Z parameter.</td></tr>
<tr><td>tangentDirection</td><td>tangentDirection</td><td>enum</td><td>If build mode is on Hermite, this paremeter dictates the tangent direction.</td></tr>
<tr><td>reverse</td><td>reverse</td><td>int</td><td>Reverse output curve and offset curve.</td></tr>
<tr><td>form</td><td>form</td><td>enum</td><td>Result curve form- open or closed</td></tr>
<tr><td>HermiteSteps</td><td>HermiteSteps</td><td>int</td><td>Hermite mode steps amount.</td></tr>
<tr><td>tangentLength</td><td>tangentLength</td><td>float</td><td>Control tangent length (if present)</td></tr>
<tr><td>OffsetType</td><td>OffsetType</td><td>enum</td><td>Offset build type - world or local.</td></tr>
<tr><td>buildOffsetCurve</td><td>buildOffsetCurve</td><td>int</td><td>Initiate offset curve build.</td></tr>
<tr><td>resample</td><td>resample</td><td>bool</td><td>Resample curve before output, based on substeps paremeter.</td></tr>
<tr><td>substeps</td><td>substeps</td><td>int</td><td>resample substeps.</td></tr>
<tr><td>localize</td><td>localize</td><td>bool</td><td> In case this attribute is on, the result will be localized based on the input worldToLocal matrix.</td></tr>
<tr><td>worldToLocalMatrix</td><td>worldToLocalMatrix</td><td>matrix</td><td> In case localize attribute is on, the result will be localized based on this matrix.</td></tr>
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
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur ===
<br>
A simple utility callback node to dynamiclly control and update the input camer'as display "Camera-Gate" parameters.
<br>
</i></font>
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
##mnsClosestPointsOnMesh
<hr width = 100%>
<font color = #5f5f5f size = 3pt><b>Inputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>inMesh</td><td>inMesh</td><td>mesh</td><td>Input mesh to find closest point to.</td></tr>
<tr><td>inPosition</td><td>inPosition</td><td>compound(Array)</td><td>Input position to calculate a result for. Array Attr.</td></tr>
<tr><td>matrix</td><td>matrix</td><td>matrix</td><td>Input matrix to calculate a result for. Array Attr.</td></tr>
<tr><td>targetParentMatrix</td><td>targetParentMatrix</td><td>matrix</td><td>Target parent matrix to multiply by before setting the result.</td></tr>
</table></font>
<font color = #5f5f5f size = 3pt><b>Outputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>outPosition</td><td>op</td><td>vector</td><td>Output position result.</td></tr>
</table></font>
<body>
##mnsCompressionTensionBlend
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur ===
<br>
Deformer.
<br>
A simple compression and tension based deformer.
<br>
This deformer will detect, display and deform a mesh
<br>
based on the difference between the current
<br>
deformed state and an input base-state (base-mesh).
<br>

<br>
The deformer contains 3 display modes:
<br>
- Compression & Tension (50% gray as base-state)
<br>
- Compression Only (black as base-state)
<br>
- Tension (black as base-state)
<br>

<br>
The deformer also conatins separate multipliers for both tension and compression.
<br>
This deformer can be used to drive corrective shapes, wrinkles, volume gain/loss and much more.
<br>
</i></font>
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
##mnsCurveTweak
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur ===
<br>
This node was created in order to achive curve modifications/tweaks, without changing its form, not it's shape at bind position.
<br>
The input and output curves will match while the base curve and tweak curve match in shape.
<br>
Once any difference between the base shape and tweak shape was detected, the difference between these curves will be projected onto the input curve.
<br>
The objective of this node is to maintain all curve attributes/data (nSpans, nCvs, form, degree) unchanged while still having the ability to tweak the curve with different parameters.
<br>
</i></font>
<hr width = 100%>
<font color = #5f5f5f size = 3pt><b>Inputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>inputCurve</td><td>inputCurve</td><td>kNurbsCurve</td><td> Input curve to tweak. Output curve will be the same as this curve while the tweak curve matches the base curve.</td></tr>
<tr><td>inputBaseCurve</td><td>inputBaseCurve</td><td>kNurbsCurve</td><td>Input base curve. This curve will be used to calculate the delta for the tweak.</td></tr>
<tr><td>inputTweakCurve</td><td>inputTweakCurve</td><td>kNurbsCurve</td><td>Input twek curve. This curve is intended to match the base curve as bind. This curve should be modified - after the curve is modified, the delta difference between it and the base curve will be projected on the input curve.</td></tr>
<tr><td>buildOffsetCurve</td><td>buildOffsetCurve</td><td>int</td><td>Initiate offset curve build.</td></tr>
<tr><td>tweakOffset</td><td>tweakOffset</td><td>int</td><td>This will determine whether the offset curve created will be tweaked or not.</td></tr>
<tr><td>offsetBaseMatrix</td><td>offsetBaseMatrix</td><td>matrix</td><td>Matrix to build offset vectors from</td></tr>
<tr><td>offset</td><td>offset</td><td>float</td><td>Output offset curve parameter.</td></tr>
</table></font>
<font color = #5f5f5f size = 3pt><b>Outputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>outCurve</td><td>outCurve</td><td>kNurbsCurve</td><td>Result curve shape.</td></tr>
<tr><td>outOffsetCurve</td><td>outOffsetCurve</td><td>kNurbsCurve</td><td>Result offset curve shape.</td></tr>
</table></font>
<body>
##mnsCurveVariable
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur ===
<br>
Curve based solve for a Variable-FK Setup.
<br>
This fast and efficient node allows the user to create a variable FK setup using input curves and local transformations, outputting a solved curve and up-curve- instead of the more common transforms output method.
<br>
The node will accept any amount of input transforms, outputting the complex offset parent solve for each input as well as the solved curves shapes.
<br>
This is to avoid the use of any extra nodes or multiple parent transforms- pinning the controls to the output curve at all times.
<br>
The initial solve, as well as all features are calculated within a single loop.
<br>
As opposed to the common Variable FK setup, the curve based approach eliminates the Rest-Pose constant- making the node's algorithm Rest-Pose dynamic. In fact, it doesn't exist.
<br>
This approach uses only the input array amount constant to calculate a uniform positioning along the output curve- allowing the input curve to be changeable (live / dynamic).
<br>
Notice that the amount of input variable controls is completely independent of the main controls input.
<br>
</i></font>
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
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur ===
<br>
Curve based node.
<br>
This is primarily used for eyelids and lips.
<br>
This fast solution was developed to replace complex and heavy graphs- containing many math nodes, curve deformers and constraints.
<br>
This setup provides a very clean deployment, processing the math algorithm internally.
<br>
Combining this node with mnsBuildTransformsCurve and mnsPointsOnCurve, will result in a very efficient, dynamic and flexible setup.
<br>
All calculations are processed within a single loop.
<br>
All curve operations are aware of one another, and are NOT addative- meaning that all operations are available at any position, and will NOT break one another, nor overlap.
<br>
All attributes are not minimum limited to 0 and can be adjusted to the negative direction- pulling the bind pose against each other instead of towards each other.
<br>
The node contains a centerMatrix input plug, which is a live world position that is used to scale the calculated vectors based on the bind position offset (per curve parameter).
<br>
The problem arising from this method is a mismatch at any meet position between curve A and B due to an offset variation between all points (except for a perfect circle scenario, which is never the case).
<br>
This problem is solved using a conform attribute within which will pull one of the curves (based on user choice) to the other below a selected distance threshold- Resulting in a watertight-seal.
<br>
Using mnsPointsOnCurve to sample the result curves allows for a simple skinCluster to deform the mesh.
<br>
mnsCurveZip will output a pair of offset curves as well as the result curves, calculated by world axis vectors or the centerMatrix as a base, which are used as an Up-Curve input for the mnsPointsOnCurve node to manage rotations correctly as well.
<br>
The node contatins some more important inputs: The tweakCurves inputs.
<br>
Aspiring to an inclusive and comprehensive setup, tweak curves (A, B and Mid) can be plugged in to expose another manual layer of animation using scene controls.
<br>
The input curves are 100% independent of the base curve inputs and DO-NOT need to share topology with each other, nor the source inputs - as they are being re-sampled internally based on the build mode.
<br>
This means that the tweak controls amount is limitless and is NOT a constant, nor predefined.
<br>
</i></font>
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
<tr><td>midCurveBase</td><td>midCrvBase</td><td>nurbsCurve</td><td>Input mid tweak curve base.</td></tr>
<tr><td>midCurveTweak</td><td>midCrvTweak</td><td>nurbsCurve</td><td>Input mid tweak curve.</td></tr>
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
##mnsCurveZipB
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur ===
<br>
Curve based node.
<br>
This is primarily used for eyelids and lips.
<br>
This fast solution was developed to replace complex and heavy graphs- containing many math nodes, curve deformers and constraints.
<br>
This setup provides a very clean deployment, processing the math algorithm internally.
<br>
Combining this node with mnsBuildTransformsCurve and mnsPointsOnCurve, will result in a very efficient, dynamic and flexible setup.
<br>
All calculations are processed within a single loop.
<br>
All curve operations are aware of one another, and are NOT addative- meaning that all operations are available at any position, and will NOT break one another, nor overlap.
<br>
All attributes are not minimum limited to 0 and can be adjusted to the negative direction- pulling the bind pose against each other instead of towards each other.
<br>
The node contains a centerMatrix input plug, which is a live world position that is used to scale the calculated vectors based on the bind position offset (per curve parameter).
<br>
The problem arising from this method is a mismatch at any meet position between curve A and B due to an offset variation between all points (except for a perfect circle scenario, which is never the case).
<br>
This problem is solved using a conform attribute within which will pull one of the curves (based on user choice) to the other below a selected distance threshold- Resulting in a watertight-seal.
<br>
Using mnsPointsOnCurve to sample the result curves allows for a simple skinCluster to deform the mesh.
<br>
mnsCurveZip will output a pair of offset curves as well as the result curves, calculated by world axis vectors or the centerMatrix as a base, which are used as an Up-Curve input for the mnsPointsOnCurve node to manage rotations correctly as well.
<br>
The node contatins some more important inputs: The tweakCurves inputs.
<br>
Aspiring to an inclusive and comprehensive setup, tweak curves (A, B and Mid) can be plugged in to expose another manual layer of animation using scene controls.
<br>
The input curves are 100% independent of the base curve inputs and DO-NOT need to share topology with each other, nor the source inputs - as they are being re-sampled internally based on the build mode.
<br>
This means that the tweak controls amount is limitless and is NOT a constant, nor predefined.
<br>
</i></font>
<hr width = 100%>
<font color = #5f5f5f size = 3pt><b>Inputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>globalScale</td><td>globalScale</td><td>double</td><td>Global scale value.</td></tr>
<tr><td>inTweakAPosition</td><td>inTweakAPosition</td><td>matrix (array)</td><td>Input tweaker local matrix.</td></tr>
<tr><td>inTweakBPosition</td><td>inTweakBPosition</td><td>matrix (array)</td><td>Input tweaker local matrix.</td></tr>
<tr><td>tweakMode</td><td>tweakMode</td><td>enum</td><td>Tweak curve build mode.</td></tr>
<tr><td>tweakMirrorMatrix</td><td>tweakMirrorMatrix</td><td>matrix</td><td>Mirror matrix to add to the local tweaker transfomation build.</td></tr>
<tr><td>bindCurveA</td><td>bindCurveA</td><td>nurbsCurve</td><td>Input curve A base-curve shape.</td></tr>
<tr><td>bindCurveB</td><td>bindCurveB</td><td>nurbsCurve</td><td>Input curve B base-curve shape.</td></tr>
<tr><td>centerMatrix</td><td>centerMatrix</td><td>matrix</td><td>Input center transformation matrix.</td></tr>
<tr><td>sampleMode</td><td>m</td><td>enum</td><td>Curve sample mode- parametric, uniform.</td></tr>
<tr><td>midCurveMode</td><td>midCurveMode</td><td>enum</td><td>Mid curve generation mode. One To one - calculate mid point for every upper and lower pair. Regenerate- create a new mid curve, resample based on midCurveSubsteps attribute value.</td></tr>
<tr><td>midCurveSubsteps</td><td>midCurveSubsteps</td><td>int</td><td>Mid curve generation sampling amount</td></tr>
<tr><td>matchInputCurve</td><td>matchInputCurve</td><td>enum</td><td>Result curve matched parameters to- none, curveA, curveB.</td></tr>
<tr><td>substeps</td><td>substeps</td><td>int</td><td>Result curve resampling sub-step value.</td></tr>
<tr><td>degree</td><td>degree</td><td>int</td><td>Result curve degree value.</td></tr>
<tr><td>buildMode</td><td>buildMode</td><td>enum</td><td>Curve build mode- EPs, CVs.</td></tr>
<tr><td>midBias</td><td>midBias</td><td>float</td><td>Generated curve bias.</td></tr>
<tr><td>aroundCenter</td><td>aroundCenter</td><td>bool</td><td>Calculate results considering the input center matrix.</td></tr>
<tr><td>conformToMeetPoint</td><td>conformToMeetPoint</td><td>bool</td><td>Conform the selected curve result to meet the oter curve based on set parameters.</td></tr>
<tr><td>curveToConform</td><td>curveToConform</td><td>enum</td><td>Which curve to conform - curveA, curveB.</td></tr>
<tr><td>conformDistancethreshold</td><td>conformDistancethreshold</td><td>enum</td><td>Which curve to conform - curveA, curveB.</td></tr>
<tr><td>AToMid</td><td>AToMid</td><td>float</td><td>Blend curve A to mid-curve.</td></tr>
<tr><td>BToMid</td><td>BToMid</td><td>float</td><td>Blend curve B to mid-curve.</td></tr>
<tr><td>AToBindB</td><td>AToBindB</td><td>float</td><td>Blend curve A to curve B.</td></tr>
<tr><td>BToBindA</td><td>BToBindA</td><td>float</td><td>Blend curve B to curve A.</td></tr>
<tr><td>AToB</td><td>AToB</td><td>float</td><td>Blend curve A to curve B.</td></tr>
<tr><td>BToA</td><td>BToA</td><td>float</td><td>Blend curve B to curve A.</td></tr>
<tr><td>sCurveA</td><td>sCurveA</td><td>float</td><td>Blend curve A into a procedural S shape.</td></tr>
<tr><td>sCurveB</td><td>sCurveB</td><td>float</td><td>Blend curve B into a procedural S shape.</td></tr>
<tr><td>allToMidPoint</td><td>allToMidPoint</td><td>float</td><td>Blend both curves to mid-curve.</td></tr>
<tr><td>pushOut</td><td>pushOut</td><td>float</td><td>Curves push-out added value.</td></tr>
<tr><td>zipStart</td><td>zipStart</td><td>float</td><td>Zip start value.</td></tr>
<tr><td>zipStartFalloff</td><td>zipStartFalloff</td><td>float</td><td>Zip start falloff value.</td></tr>
<tr><td>zipEnd</td><td>zipEnd</td><td>float</td><td>Zip end value.</td></tr>
<tr><td>zipEndFalloff</td><td>zipEndFalloff</td><td>float</td><td>Zip end falloff value.</td></tr>
<tr><td>offsetBase</td><td>offsetBase</td><td>enum</td><td>Offset curve build mode. centerMatrix, worldX, worldY, worldZ.</td></tr>
<tr><td>offset</td><td>offset</td><td>float</td><td>Offset curve build parameter.</td></tr>
</table></font>
<font color = #5f5f5f size = 3pt><b>Outputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>outCurveA</td><td>outCurveA</td><td>nurbsCurve</td><td>Result curve A shape.</td></tr>
<tr><td>outCurveB</td><td>outCurveB</td><td>nurbsCurve</td><td>Result curve B shape.</td></tr>
<tr><td>outCurveAOffset</td><td>outCurveAOffset</td><td>nurbsCurve</td><td>Result curve A offset shape.</td></tr>
<tr><td>outCurveBOffset</td><td>outCurveBOffset</td><td>nurbsCurve</td><td>Result curve B offset shape.</td></tr>
<tr><td>outTweakA</td><td>outTweakA</td><td>compound (array)</td><td>Parent attribute that holds output values for tweaker offset position.</td></tr>
<tr><td>outTweakATranslate</td><td>outTweakATranslate</td><td>vector</td><td>Output offset position for a given tweaker.</td></tr>
<tr><td>outTweakARotate</td><td>outTweakARotate</td><td>vector</td><td>Output offset rotation for a given tweaker.</td></tr>
<tr><td>outTweakB</td><td>outTweakB</td><td>compound (array)</td><td>Parent attribute that holds output values for tweaker offset position.</td></tr>
<tr><td>outTweakBTranslate</td><td>outTweakBTranslate</td><td>vector</td><td>Output offset position for a given tweaker.</td></tr>
<tr><td>outTweakBRotate</td><td>outTweakBRotate</td><td>vector</td><td>Output offset rotation for a given tweaker.</td></tr>
</table></font>
<body>
##mnsDynamicPivot
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur ===
<br>
This is a simple node to calculate a foot's dynamic pivot internally, acoiding the use of many transforms and node connections.
<br>
Given an input curve, world origin position (as matrix) and mapping info, this node will map the input rotation values into a new custom point adding the rotation into the translation.
<br>
This essentailly will push the new point rapidly away from it's origin into the mapping direction.
<br>
Now using the given input curve, the closest point on curve from the new point will be calcultaed and outputted into the rotatePivot plug.
<br>
This output plug can then be plugged into a custom pivot attribute of any transform- creating a dynamiclly calculated pivot along the given curve.
<br>
</i></font>
<hr width = 100%>
<font color = #5f5f5f size = 3pt><b>Inputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>inputCurve</td><td>inputCurve</td><td>nurbsCurve</td><td>Input curve.</td></tr>
<tr><td>rotateX</td><td>rx</td><td>angle</td><td>Input local X rotation.</td></tr>
<tr><td>rotateY</td><td>ry</td><td>angle</td><td>Input local Y rotation.</td></tr>
<tr><td>rotateZ</td><td>rz</td><td>angle</td><td>Input local Z rotation.</td></tr>
<tr><td>rotate</td><td>r</td><td>angle[3]</td><td>Input rotations.</td></tr>
<tr><td>originWorldMatrix</td><td>owm</td><td>matrix</td><td>Input origin position to strat the calculation from.</td></tr>
<tr><td>targetParentInverseMatrix</td><td>tpim</td><td>matrix</td><td> Target transform parent inverse matrix to localize the rotate pivot position result.</td></tr>
<tr><td>mapRotXTo</td><td>mapRotXTo</td><td>enum</td><td>Mapping info from input X rotation.</td></tr>
<tr><td>mapRotYTo</td><td>mapRotYTo</td><td>enum</td><td>Mapping info from input Y rotation.</td></tr>
<tr><td>mapRotZTo</td><td>mapRotZTo</td><td>enum</td><td>Mapping info from input Z rotation.</td></tr>
<tr><td>distRateMultiplier</td><td>distRateMultiplier</td><td>double</td><td>The rotation rate of addition in the translation values.</td></tr>
<tr><td>inputMultipliers</td><td>inputMultipliers</td><td>bool</td><td>Pre-calc input multipliers.</td></tr>
</table></font>
<font color = #5f5f5f size = 3pt><b>Outputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>rotatePivot</td><td>rotatePivot</td><td>float[3]</td><td>Result rotate pivot position.</td></tr>
</table></font>
<body>
##mnsExponential
<hr width = 100%>
<body>
##mnsIKSolver
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur ===
<br>
This IK-Solver node provides an alternative, faster and more reliable solution for a 2-joint IK set-up.
<br>
This enhanced IK-solution offers a much cleaner approach as well, computing the blend internally- making any basic IK-FK set-up efficient, stable, fast and clean.
<br>
To add on the internal FK-IK switch, this node contains a few more features that are already an industry
<br>
standard:
<br>
Softness - prevents a pop on ik limit approach.
<br>
Slide - Knee position sliding (for character animation).
<br>
Stretch - Providing a limb-stretch when the ik-solve is beyond its limit.
<br>
Axis Switching - Offering an easy switch to any joint orientation.
<br>
</i></font>
<hr width = 100%>
<font color = #5f5f5f size = 3pt><b>Inputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>boneLengthA</td><td>bla</td><td>float</td><td>Base length A.</td></tr>
<tr><td>boneLengthB</td><td>blb</td><td>float</td><td>Base length B.</td></tr>
<tr><td>restHandleLength</td><td>restHandleLength</td><td>float</td><td>Base length between the root position and the handle.</td></tr>
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
<tr><td>segmentScaleCompensate</td><td>segmentScaleCompensate</td><td>bool</td><td>calculate with segment scale compensate on or off.</td></tr>
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
##mnsLipZip
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur ===
<br>
Curve based node.
<br>
</i></font>
<hr width = 100%>
<font color = #5f5f5f size = 3pt><b>Inputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>globalScale</td><td>globalScale</td><td>double</td><td>Global scale value.</td></tr>
<tr><td>inTweakAPosition</td><td>inTweakAPosition</td><td>matrix (array)</td><td>Input tweaker local matrix.</td></tr>
<tr><td>inTweakBPosition</td><td>inTweakBPosition</td><td>matrix (array)</td><td>Input tweaker local matrix.</td></tr>
<tr><td>tweakMode</td><td>tweakMode</td><td>enum</td><td>Tweak curve build mode.</td></tr>
<tr><td>tweakMirrorMatrix</td><td>tweakMirrorMatrix</td><td>matrix</td><td>Mirror matrix to add to the local tweaker transfomation build.</td></tr>
<tr><td>centerMatrix</td><td>centerMatrix</td><td>matrix</td><td>Input center transformation matrix.</td></tr>
<tr><td>sampleMode</td><td>m</td><td>enum</td><td>Curve sample mode- parametric, uniform.</td></tr>
<tr><td>substeps</td><td>substeps</td><td>int</td><td>Result curve resampling sub-step value.</td></tr>
<tr><td>degree</td><td>degree</td><td>int</td><td>Result curve degree value.</td></tr>
<tr><td>buildMode</td><td>buildMode</td><td>enum</td><td>Curve build mode- EPs, CVs.</td></tr>
<tr><td>midBias</td><td>midBias</td><td>float</td><td>Generated curve bias.</td></tr>
<tr><td>aroundCenter</td><td>aroundCenter</td><td>bool</td><td>Calculate results considering the input center matrix.</td></tr>
<tr><td>alongSurface</td><td>alongSurface</td><td>bool</td><td>Calculate results considering the input surface.</td></tr>
<tr><td>conformToMeetPoint</td><td>conformToMeetPoint</td><td>bool</td><td>Conform the selected curve result to meet the oter curve based on set parameters.</td></tr>
<tr><td>curveToConform</td><td>curveToConform</td><td>enum</td><td>Which curve to conform - curveA, curveB.</td></tr>
<tr><td>conformDistancethreshold</td><td>conformDistancethreshold</td><td>enum</td><td>Which curve to conform - curveA, curveB.</td></tr>
<tr><td>AToMid</td><td>AToMid</td><td>float</td><td>Blend curve A to mid-curve.</td></tr>
<tr><td>BToMid</td><td>BToMid</td><td>float</td><td>Blend curve B to mid-curve.</td></tr>
<tr><td>AToB</td><td>AToB</td><td>float</td><td>Blend curve A to curve B.</td></tr>
<tr><td>BToA</td><td>BToA</td><td>float</td><td>Blend curve B to curve A.</td></tr>
<tr><td>sCurveA</td><td>sCurveA</td><td>float</td><td>Blend curve A into a procedural S shape.</td></tr>
<tr><td>sCurveB</td><td>sCurveB</td><td>float</td><td>Blend curve B into a procedural S shape.</td></tr>
<tr><td>allToMidPoint</td><td>allToMidPoint</td><td>float</td><td>Blend both curves to mid-curve.</td></tr>
<tr><td>upperCurlBaseMatrix</td><td>upperCurlBaseMatrix</td><td>matrix</td><td>Base upper matrix to calculate offsets before calculating the curl.</td></tr>
<tr><td>upperCurlMatrix</td><td>upperCurlMatrix</td><td>matrix</td><td> Upper matrix for calculating the curl.</td></tr>
<tr><td>upperCurlFalloff</td><td>upperCurlFalloff</td><td>float</td><td> Upper curl falloff</td></tr>
<tr><td>lowerCurlBaseMatrix</td><td>lowerCurlBaseMatrix</td><td>matrix</td><td>Base lower matrix to calculate offsets before calculating the curl.</td></tr>
<tr><td>lowerCurlMatrix</td><td>lowerCurlMatrix</td><td>matrix</td><td> Lower matrix for calculating the curl.</td></tr>
<tr><td>lowerCurlFalloff</td><td>lowerCurlFalloff</td><td>float</td><td> Lower curl falloff</td></tr>
<tr><td>pushOutA</td><td>pushOutA</td><td>float</td><td>Curves push-out added value.</td></tr>
<tr><td>pushOutB</td><td>pushOutB</td><td>float</td><td>Curves push-out added value.</td></tr>
<tr><td>zipStart</td><td>zipStart</td><td>float</td><td>Zip start value.</td></tr>
<tr><td>zipStartFalloff</td><td>zipStartFalloff</td><td>float</td><td>Zip start falloff value.</td></tr>
<tr><td>zipEnd</td><td>zipEnd</td><td>float</td><td>Zip end value.</td></tr>
<tr><td>zipEndFalloff</td><td>zipEndFalloff</td><td>float</td><td>Zip end falloff value.</td></tr>
<tr><td>offsetBase</td><td>offsetBase</td><td>enum</td><td>Offset curve build mode. centerMatrix, worldX, worldY, worldZ.</td></tr>
<tr><td>offset</td><td>offset</td><td>float</td><td>Offset curve build parameter.</td></tr>
</table></font>
<font color = #5f5f5f size = 3pt><b>Outputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>outCurveA</td><td>outCurveA</td><td>nurbsCurve</td><td>Result curve A shape.</td></tr>
<tr><td>outCurveB</td><td>outCurveB</td><td>nurbsCurve</td><td>Result curve B shape.</td></tr>
<tr><td>outCurveAOffset</td><td>outCurveAOffset</td><td>nurbsCurve</td><td>Result curve A offset shape.</td></tr>
<tr><td>outCurveBOffset</td><td>outCurveBOffset</td><td>nurbsCurve</td><td>Result curve B offset shape.</td></tr>
<tr><td>outTweakA</td><td>outTweakA</td><td>compound (array)</td><td>Parent attribute that holds output values for tweaker offset position.</td></tr>
<tr><td>outTweakATranslate</td><td>outTweakATranslate</td><td>vector</td><td>Output offset position for a given tweaker.</td></tr>
<tr><td>outTweakARotate</td><td>outTweakARotate</td><td>vector</td><td>Output offset rotation for a given tweaker.</td></tr>
<tr><td>outTweakB</td><td>outTweakB</td><td>compound (array)</td><td>Parent attribute that holds output values for tweaker offset position.</td></tr>
<tr><td>outTweakBTranslate</td><td>outTweakBTranslate</td><td>vector</td><td>Output offset position for a given tweaker.</td></tr>
<tr><td>outTweakBRotate</td><td>outTweakBRotate</td><td>vector</td><td>Output offset rotation for a given tweaker.</td></tr>
</table></font>
<body>
##mnsMatrixConstraint
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur ===
<br>
Light weight alternative to Maya's native constraints - All within one node.
<br>
Live switchable/keyable maintainOffset channel.
<br>
Easily add spaces/masters to existing constraint using recalcOffset channel.
<br>
</i></font>
<hr width = 100%>
<font color = #5f5f5f size = 3pt><b>Inputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>sourceWorldMatrix</td><td>sourceWorldMatrix</td><td>matrix</td><td>Source world matrix.</td></tr>
<tr><td>spaceSet</td><td>spaceSet</td><td>int</td><td>Constraint Space index.</td></tr>
<tr><td>maintainOffset</td><td>maintainOffset</td><td>bool</td><td>Maintain offset attribute.</td></tr>
<tr><td>recalcOffsets</td><td>recalcOffsets</td><td>int</td><td>Recalculate offset in current state.</td></tr>
<tr><td>targetParentInverseMatrix</td><td>targetParentInverseMatrix</td><td>matrix</td><td>Traget inverse matrix.</td></tr>
<tr><td>targetRotateOrder</td><td>targetRotateOrder</td><td>enum</td><td>Calculation rotate-order.</td></tr>
<tr><td>targetWorldMatrix</td><td>targetWorldMatrix</td><td>matrix</td><td>Traget world matrix.</td></tr>
</table></font>
<font color = #5f5f5f size = 3pt><b>Outputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>matrix</td><td>m</td><td>matrix</td><td>Result as matrix form.</td></tr>
<tr><td>translate</td><td>t</td><td>float[3]</td><td>Translation values result.</td></tr>
<tr><td>rotate</td><td>r</td><td>angle[3]</td><td>Rotation values result.</td></tr>
<tr><td>scale</td><td>s</td><td>float[3]</td><td>Scale values result.</td></tr>
<tr><td>shear</td><td>shear</td><td>float[3]</td><td>Shear values result.</td></tr>
</table></font>
<body>
##mnsMeshRivets
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur ===
<br>
A multi "Point-On-Poly" constraint style compute node.
<br>
The node will accept any amount of input positions, as well as an input base-mesh and a target mesh.
<br>
The base mesh is used to calculate the source position and offset, the target mesh is used to calculate the result position based on the selected attributes within the node:
<br>
- Calculation Method: Closest UV, Vertex, Face
<br>
- Do Rotation: On, Off
<br>
- Do Scale: On, Off
<br>
- Rotation: Aim-Axis and up Axis choice (All 6)
<br>
- Up-Mode: World (X,Y,Z), Closest Tangent, Closest Binormal
<br>
The node will accept any amount on input tweaker matrices that can be used to adjust the riveted transforms globally and easily.
<br>
The tweakers adjustments are calculated in world spcae and the algorithm is fully independent, additive, and keyable.
<br>
The proximity calculation is matrix based to achieve non-spherical tweaks.
<br>
As tweaking the position of the rivets is not sensible as the transforms' position is based on the target mesh, the proximity tweakers are used to adjust rotation and scale only.
<br>
The node contains two adjustemt spaces:
<br>
- World- Will transform the outputs in world space, providing a more intuative behaviour, although less practical.
<br>
- Object - Will transform the outputs in their relative local spaces (preferable), which will provide a less intuative behaviour (dependent of the tweaker and output orientation), although very practical.
<br>
A falloff attribute is also implemented to allow control over the decay within the "collision" zone.
<br>
</i></font>
<hr width = 100%>
<font color = #5f5f5f size = 3pt><b>Inputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>mesh</td><td>mesh</td><td>mesh</td><td>Input mesh to rivet to.</td></tr>
<tr><td>targetWorldMatrix</td><td>targetWorldMatrix</td><td>matrix</td><td>Input mesh world matrix.</td></tr>
<tr><td>rivet</td><td>rivet</td><td>compound</td><td>Input rivet transforms array.</td></tr>
<tr><td>worldMatrix</td><td>worldMatrix</td><td>matrix</td><td>Input rivet transforms matrix. Child of rivet.</td></tr>
<tr><td>parentInverseMatrix</td><td>parentInverseMatrix</td><td>matrix</td><td>Input rivet transforms inverse parent matrix. Child of rivet.</td></tr>
<tr><td>liveMode</td><td>liveMode</td><td>bool</td><td>Live mode. Calculate everything in every evaluation.</td></tr>
<tr><td>calculationMethod</td><td>calculationMethod</td><td>enum</td><td>Calculation basis- UV, closestVertex, closestFace.</td></tr>
<tr><td>uvTolerance</td><td>uvTolerance</td><td>float</td><td>UV search tolerance threshold value.</td></tr>
<tr><td>doRotation</td><td>doRotation</td><td>bool</td><td>Calculate rotations.</td></tr>
<tr><td>doRivetRotation</td><td>doRivetRotation</td><td>bool</td><td>Calculate rivet local rotations.</td></tr>
<tr><td>rotateOrder</td><td>ro</td><td>enum</td><td>Calculation rotate-order.</td></tr>
<tr><td>upMode</td><td>upMode</td><td>enum</td><td>Rotation calculation up mode- worldX, worldY, worldZ, closestVertexBinormal, closestVertexTangent.</td></tr>
<tr><td>aimAxis</td><td>aimAxis</td><td>enum</td><td>Aim Axis choice.</td></tr>
<tr><td>upAxis</td><td>upAxis</td><td>enum</td><td>Up Axis choice.</td></tr>
<tr><td>doRivetScale</td><td>doRivetScale</td><td>bool</td><td>Calculate scale.</td></tr>
<tr><td>doScale</td><td>doScale</td><td>bool</td><td>Scale the rivets with the target mesh scale. When off the mesh's scale doesn't affect the rivets.</td></tr>
<tr><td>maintainOffset</td><td>maintainOffset</td><td>bool</td><td>Maintain offset between rivet position and target mesh.</td></tr>
<tr><td>proximityRotationSpace</td><td>proximityRotationSpace</td><td>enum</td><td>Proximity tweak rotation space- object, world.</td></tr>
<tr><td>proximityTweaker</td><td>proximityTweaker</td><td>compound</td><td>Proximity tweakers input array.</td></tr>
<tr><td>proximityWorldMatrix</td><td>proximityWorldMatrix</td><td>matrix</td><td>Proximity tweaker matrix. Child of proximityTweaker.</td></tr>
<tr><td>proximityLocalMatrix</td><td>proximityLocalMatrix</td><td>matrix</td><td>Proximity tweaker local matrix. Child of proximityTweaker.</td></tr>
<tr><td>rivetScale</td><td>rivetScale</td><td>float[3]</td><td>Scale tweak input.</td></tr>
<tr><td>falloff</td><td>falloff</td><td>float</td><td>Proximity tweak falloff. Child of proximityTweaker.</td></tr>
<tr><td>texture</td><td>texture</td><td>color</td><td>Input color map adjustment.</td></tr>
<tr><td>rotationTextureAmplitude</td><td>rotationTextureAmplitude</td><td>float</td><td>Color map adjustment amplitude.</td></tr>
<tr><td>textureBothDirections</td><td>textureBothDirections</td><td>bool</td><td>Avarage color map adjustment to both direction. -0.5 0.5 instead of 0 to 1.</td></tr>
<tr><td>scaleTextureAmplitude</td><td>scaleTextureAmplitude</td><td>float</td><td>Color map scale affect amplitude.</td></tr>
</table></font>
<font color = #5f5f5f size = 3pt><b>Outputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>translate</td><td>t</td><td>float[3]</td><td>Translation output. Child of transform.</td></tr>
<tr><td>rotate</td><td>r</td><td>angle[3]</td><td>Rotation output. Child of transform.</td></tr>
<tr><td>transform</td><td>transform</td><td>compound</td><td>Output transforms array.</td></tr>
<tr><td>scale</td><td>s</td><td>angle[3]</td><td>Scale output. Child of transform.</td></tr>
<tr><td>baseMesh</td><td>baseMesh</td><td>mesh</td><td>Input base-mesh.</td></tr>
</table></font>
<body>
##mnsMeshSeparate
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur ===
<br>
A simple node to drive seprated shell objects using one combined mesh.
<br>
</i></font>
<hr width = 100%>
<font color = #5f5f5f size = 3pt><b>Inputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>mesh</td><td>mesh</td><td>mesh</td><td>Input mesh to separate.</td></tr>
<tr><td>inShell</td><td>inShell</td><td>mesh</td><td>Input shell object array.</td></tr>
</table></font>
<font color = #5f5f5f size = 3pt><b>Outputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>outMesh</td><td>outMesh</td><td>mesh</td><td>Result shell meshes array.</td></tr>
</table></font>
<body>
##mnsModuleVis
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur ===
<br>
A Simple dedicated node to control module visibility.
<br>
Previously was done using 3 animCurvesUU nodes, this is designed to replace them.
<br>
This node takes an input enum attribute, which was 8 states:
<br>
1. None
<br>
2. Primaries
<br>
3. Secondaries
<br>
4. Tertiaries
<br>
5. Secondaries Only
<br>
6. Tertiaries Only
<br>
7. No Primaries
<br>
8. No Secondaries
<br>

<br>
Based on the selected input state, the node will output 3 channels which will be connected to the modules' root transform.
<br>
1. Primary Vis
<br>
2. Secondary Vis
<br>
3. Tertiary Vis
<br>

<br>
The result graph:
<br>
+ None
<br>
	- Primary Vis - OFF
<br>
	- Secondary Vis - OFF
<br>
	- Tertiary Vis - OFF
<br>
+ Primaries
<br>
	- Primary Vis - ON
<br>
	- Secondary Vis - OFF
<br>
	- Tertiary Vis - OFF
<br>
+ Secondaries
<br>
	- Primary Vis - ON
<br>
	- Secondary Vis - ON
<br>
	- Tertiary Vis - ON
<br>
+ Tertiaries
<br>
	- Primary Vis - ON
<br>
	- Secondary Vis - ON
<br>
	- Tertiary Vis - OFF
<br>
+ Secondaries Only
<br>
	- Primary Vis - OFF
<br>
	- Secondary Vis - ON
<br>
	- Tertiary Vis - OFF
<br>
+ Tertiaries Only
<br>
	- Primary Vis - OFF
<br>
	- Secondary Vis - OFF
<br>
	- Tertiary Vis - ON
<br>
+ No Primaries
<br>
	- Primary Vis - OFF
<br>
	- Secondary Vis - ON
<br>
	- Tertiary Vis - ON
<br>
+ No Secondaries
<br>
	- Primary Vis - ON
<br>
	- Secondary Vis - OFF
<br>
	- Tertiary Vis - ON
<br>

<br>
This node will be used by block to cleanup the input graph for the visibility control.
<br>
</i></font>
<hr width = 100%>
<font color = #5f5f5f size = 3pt><b>Inputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>inputVisibility</td><td>inputVisibility</td><td>enum</td><td>Input visibility enum.</td></tr>
</table></font>
<font color = #5f5f5f size = 3pt><b>Outputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>primaryVis</td><td>primaryVis</td><td>double</td><td>Output visibility for primaries</td></tr>
<tr><td>secondaryVis</td><td>secondaryVis</td><td>double</td><td>Output visibility for secondaries</td></tr>
<tr><td>tertiaryVis</td><td>reinitialize</td><td>double</td><td>Output visibility for tertiaries</td></tr>
</table></font>
<body>
##mnsModulo
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur ===
<br>
A simple math node missing from Maya's native library.
<br>
Given a value and a devisor, the node will compute modulo based operations:
<br>
- modulos - the remainder or signed remainder of a division, after one number is divided by another- double.
<br>
- modulosInt - the remainder or signed remainder of a division, after one number is divided by another- int.
<br>
- Cycles - Number of repetitions - double.
<br>
- CyclesInt - Number of repetitions - int.
<br>
- Alternate - Alternating between 0 and the devisor.
<br>
- Alternate - Alternating between 0 and 1, based on the devisor.
<br>
</i></font>
<hr width = 100%>
<font color = #5f5f5f size = 3pt><b>Inputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>value</td><td>value</td><td>double</td><td>Value to compute.</td></tr>
<tr><td>devisor</td><td>devisor</td><td>double</td><td>Devisor to compute.</td></tr>
</table></font>
<font color = #5f5f5f size = 3pt><b>Outputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>modulus</td><td>modulus</td><td>double</td><td>The remainder or signed remainder of a division, after value is divided by the devisor.</td></tr>
<tr><td>modulusInt</td><td>modulusInt</td><td>int</td><td>The remainder or signed remainder of a division, after value is divided by the devisor.</td></tr>
<tr><td>cycles</td><td>cycles</td><td>double</td><td>Number of repetitions-Double.</td></tr>
<tr><td>cyclesInt</td><td>cyclesInt</td><td>double</td><td>Number of repetitions-Int.</td></tr>
<tr><td>alternate</td><td>alternate</td><td>double</td><td>Alternating value between 0 and the devisor.</td></tr>
<tr><td>alternateNormalized</td><td>alternateNormalized</td><td>double</td><td>Alternating between 0 and 1, based on the devisor.</td></tr>
</table></font>
<body>
##mnsNodeRelationship
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur ===
<br>
BLOCK main relationship node.
<br>
</i></font>
<hr width = 100%>
<font color = #5f5f5f size = 3pt><b>Inputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>messageIn</td><td>messageIn</td><td>message</td><td>Input master node.</td></tr>
<tr><td>messageOut</td><td>messageOut</td><td>message</td><td>Input slaves nodes array.</td></tr>
<tr><td>deleteSlaves</td><td>deleteSlaves</td><td>message</td><td>Input delete only slaves nodes array.</td></tr>
</table></font>
<body>
##mnsPointsOnCurve
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur ===
<br>
A fast and efficient parameter based compute node to sample and control points along a given curve.
<br>
In combination with mnsBuildTransformsCurve will result in a very advanced and robust "spline IK" control.
<br>
- Creation modes
<br>
     + Parametric - curve parameterized position calculation
<br>
	 + Uniform - Addaptive uniform sampling
<br>
	 + Fixed length - Uniform sampling based on an input max length. Initialized to curve length on creation, Keyable.
<br>
- Position control
<br>
- Rotation control
<br>
	 + Aim modes - curveTangent, object
<br>
	 + Up modes - curveNormal, up-curve, worldX, worldY, worldZ, object
<br>
- Scale control
<br>
- Spring ability
<br>
</i></font>
<hr width = 100%>
<font color = #5f5f5f size = 3pt><b>Inputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>curve</td><td>crv</td><td>nurbsCurve</td><td>Input curve to sample.</td></tr>
<tr><td>upCurve</td><td>upCrv</td><td>nurbsCurve</td><td>Input up curve to sample.</td></tr>
<tr><td>bindCurve</td><td>bindCrv</td><td>nurbsCurve</td><td>Input bind curve to sample. Used only in parametrically-uniform build mode.</td></tr>
<tr><td>aimCurve</td><td>aimCurve</td><td>nurbsCurve</td><td>Input aim curve to sample. Used only in curveAim rotation mode.</td></tr>
<tr><td>upObject</td><td>upObj</td><td>matrix</td><td>Input up object matrix to use if requsted.</td></tr>
<tr><td>objectOrientUpAxis</td><td>objectOrientUpAxis</td><td>enum</td><td>In case object orient up mode is selected, which axis to use.</td></tr>
<tr><td>objectOrientAimAxis</td><td>objectOrientAimAxis</td><td>enum</td><td>In case object orient aim mode is selected, which axis to use.</td></tr>
<tr><td>aimObject</td><td>aimObj</td><td>matrix</td><td>Input aim object matrix to use if requsted.</td></tr>
<tr><td>globalScale</td><td>globalScale</td><td>float</td><td>Global scale multiplier.</td></tr>
<tr><td>numOutputs</td><td>numO</td><td>int</td><td>Number of outputs/samples.</td></tr>
<tr><td>mode</td><td>m</td><td>enum direction=i</td><td>Smaple mode- parametric, uniform, uniformFixedLength.</td></tr>
<tr><td>cycle</td><td>cycle</td><td>bool</td><td>Enable cycle mode.</td></tr>
<tr><td>closedShape</td><td>closedShape</td><td>bool</td><td>Enable closed shape mode.</td></tr>
<tr><td>uScale</td><td>uScl</td><td>float</td><td>Global positions U-Scale adjustment.</td></tr>
<tr><td>uScaleInverse</td><td>uSclInv</td><td>float</td><td>Global positions U-Scale-Inverse adjustment.</td></tr>
<tr><td>uScaleMid</td><td>uSclMid</td><td>float</td><td>Global positions U-Scale-mid adjustment.</td></tr>
<tr><td>uScaleMidPos</td><td>uSclMidPos</td><td>float</td><td>U-Scale-mid-position value.</td></tr>
<tr><td>uScaleMidInverse</td><td>uSclMidInv</td><td>float</td><td>Global positions U-Scale-mid-inverse adjustment.</td></tr>
<tr><td>uOffset</td><td>uOffset</td><td>float</td><td>Global positions U-offset adjustment.</td></tr>
<tr><td>inverse</td><td>inv</td><td>bool</td><td>Inverse result order.</td></tr>
<tr><td>fixedLength</td><td>fixedLength</td><td>float</td><td>The maximum fixed length for the result sample if requested.</td></tr>
<tr><td>creationLength</td><td>creationLen</td><td>float</td><td>Value store for the creation curve length.</td></tr>
<tr><td>curveLength</td><td>crvLrn</td><td>float</td><td>Current curve length display.</td></tr>
<tr><td>uTugScale</td><td>uTugScl</td><td>float</td><td>Global positions U-Tug-Scale adjustment.</td></tr>
<tr><td>uTugScaleTension</td><td>uTugSclTension</td><td>float</td><td>Global positions U-Tug-Scale-tension parameter.</td></tr>
<tr><td>uTugOffset</td><td>uTugOffset</td><td>float</td><td>Global positions U-Tug-Offset adjustment.</td></tr>
<tr><td>rotateMode</td><td>rotMode</td><td>enum</td><td>Samples rotation mode- curveTangent, objectAim.</td></tr>
<tr><td>upMode</td><td>upMode</td><td>enum</td><td>Samples rotation up mode- normal, curve, worldX, worldY, worldZ, objectUp.</td></tr>
<tr><td>scaleMode</td><td>sclMode</td><td>enum</td><td>Samples scale mode- absuloteCurveLength, addaptiveCurveLength, segmentLengthDependent.</td></tr>
<tr><td>squashMode</td><td>squashMode</td><td>enum</td><td>Samples squash mode- squashStretch, squash, stretch, uniform, none.</td></tr>
<tr><td>doRotation</td><td>doRot</td><td>bool</td><td>Do samples rotation.</td></tr>
<tr><td>doScale</td><td>doScl</td><td>bool</td><td>Do samples scale.</td></tr>
<tr><td>rotateOrder</td><td>ro</td><td>enum direction=i</td><td>Calculation rotation order.</td></tr>
<tr><td>aimAxis</td><td>aimAxis</td><td>enum</td><td>Aim axis choice.</td></tr>
<tr><td>upAxis</td><td>upAxis</td><td>enum</td><td>Up axis choice.</td></tr>
<tr><td>customPointsUpMode</td><td>cusPointsUpMode</td><td>enum</td><td>Custom tweakers rotation up mode.</td></tr>
<tr><td>enableParamAdjust</td><td>enableParamAdjust</td><td>bool</td><td> Enable Manual parameter adjustments.</td></tr>
<tr><td>paramAdjustment</td><td>paramAdjustment</td><td>double</td><td>Manual parameter adjustments array input. Use this parameter to adjust calculated curve parameters manually. This parameter is addative.</td></tr>
<tr><td>aimParamAdjustment</td><td>aimParamAdjustment</td><td>double</td><td>Manual parameter adjustments array input for the aim curve param. Use this parameter to adjust calculated aim curve parameters manually. This parameter is addative.</td></tr>
<tr><td>excludePolesTranslation</td><td>excludePolesTranslation</td><td>bool</td><td>exclude translation set for base and tip.</td></tr>
<tr><td>excludePolesRotation</td><td>excludePolesRotation</td><td>bool</td><td>exclude rotation set for base and tip.</td></tr>
<tr><td>excludeBaseRotation</td><td>excludeBaseRotation</td><td>bool</td><td>exclude rotation set for base. Only if excludePolesRotation is set to True.</td></tr>
<tr><td>excludeTipRotation</td><td>excludeTipRotation</td><td>bool</td><td>exclude rotation set for tip. Only if excludePolesRotation is set to True.</td></tr>
<tr><td>excludePolesScale</td><td>excludePolesScale</td><td>bool</td><td>exclude scale set for base and tip.</td></tr>
<tr><td>twistAimStart</td><td>twistAimStart</td><td>float</td><td>Self explanatory.</td></tr>
<tr><td>twistAimMid</td><td>twistAimMid</td><td>float</td><td>Self explanatory.</td></tr>
<tr><td>squeezeAim</td><td>squeezeAim</td><td>float</td><td>Self explanatory.</td></tr>
<tr><td>waveAimAngle</td><td>waveAimAng</td><td>float</td><td>Self explanatory.</td></tr>
<tr><td>twistAimWavePhase</td><td>twistAimWavePhase</td><td>float</td><td>Self explanatory.</td></tr>
<tr><td>twistAimMidPos</td><td>twistAimMidPos</td><td>float</td><td>Self explanatory.</td></tr>
<tr><td>twistAimEnd</td><td>twistAimEnd</td><td>float</td><td>Self explanatory.</td></tr>
<tr><td>twistAimAll</td><td>twistAimAll</td><td>float</td><td>Self explanatory.</td></tr>
<tr><td>aimToObj</td><td>aimToObj</td><td>float</td><td>Self explanatory.</td></tr>
<tr><td>upToObj</td><td>upToObj</td><td>float</td><td>Self explanatory.</td></tr>
<tr><td>twistUpStart</td><td>twistUpStart</td><td>float</td><td>Self explanatory.</td></tr>
<tr><td>twistUpMid</td><td>twistUpMid</td><td>float</td><td>Self explanatory.</td></tr>
<tr><td>twistUpSqueeze</td><td>twistUpqueeze</td><td>float</td><td>Self explanatory.</td></tr>
<tr><td>waveUpAngle</td><td>waveUpAng</td><td>float</td><td>Self explanatory.</td></tr>
<tr><td>waveUpPhase</td><td>waveUPPhase</td><td>float</td><td>Self explanatory.</td></tr>
<tr><td>twistUpMidPos</td><td>twistUpMidPos</td><td>float</td><td>Self explanatory.</td></tr>
<tr><td>twistUpEnd</td><td>twistUpEnd</td><td>float</td><td>Self explanatory.</td></tr>
<tr><td>twistUpAll</td><td>twistUpAll</td><td>float</td><td>Self explanatory.</td></tr>
<tr><td>twistTertiaryStart</td><td>twistTerStart</td><td>float</td><td>Self explanatory.</td></tr>
<tr><td>twistTertiaryMid</td><td>twistTerMid</td><td>float</td><td>Self explanatory.</td></tr>
<tr><td>tertiarySqueeze</td><td>terSqueeze</td><td>float</td><td>Self explanatory.</td></tr>
<tr><td>tertiaryWaveAngle</td><td>tertiaryWaveAng</td><td>float</td><td>Self explanatory.</td></tr>
<tr><td>tertiaryWavePhase</td><td>terWavePhase</td><td>float</td><td>Self explanatory.</td></tr>
<tr><td>twistTertiaryMidPos</td><td>twistTerMidPos</td><td>float</td><td>Self explanatory.</td></tr>
<tr><td>tertiaryTwistEnd</td><td>terTwistEnd</td><td>float</td><td>Self explanatory.</td></tr>
<tr><td>tertiaryTwistAll</td><td>terTwistAll</td><td>float</td><td>Self explanatory.</td></tr>
<tr><td>resetScale</td><td>resetScl</td><td>int</td><td>Reset scale values to current state.</td></tr>
<tr><td>scaleMaxAddaptive</td><td>sclMaxAddaptive</td><td>bool</td><td>Adapt max scale to squash/scale relative values.</td></tr>
<tr><td>squashFactor</td><td>squashFactor</td><td>float</td><td>Squash multiplier.</td></tr>
<tr><td>squashPos</td><td>squashPos</td><td>float</td><td>Squash position.</td></tr>
<tr><td>scaleStart</td><td>sclStart</td><td>float</td><td>Self explanatory.</td></tr>
<tr><td>scaleMid</td><td>sclMid</td><td>float</td><td>Self explanatory.</td></tr>
<tr><td>scaleMidPos</td><td>sclMidPos</td><td>float</td><td>Self explanatory.</td></tr>
<tr><td>scaleWaveAmp</td><td>sclWaveAmp</td><td>float</td><td>Self explanatory.</td></tr>
<tr><td>scaleWavePhase</td><td>sclWavePhase</td><td>float</td><td>Self explanatory.</td></tr>
<tr><td>scaleEnd</td><td>sclEnd</td><td>float</td><td>Self explanatory.</td></tr>
<tr><td>scaleAll</td><td>sclAll</td><td>float</td><td>Self explanatory.</td></tr>
<tr><td>scaleAllAim</td><td>scaleAllAim</td><td>float</td><td>Self explanatory.</td></tr>
<tr><td>scaleAllUp</td><td>scaleAllUp</td><td>float</td><td>Self explanatory.</td></tr>
<tr><td>scaleAllTertiary</td><td>scaleAllTertiary</td><td>float</td><td>Self explanatory.</td></tr>
<tr><td>scaleMin</td><td>sclMin</td><td>float</td><td>Self explanatory.</td></tr>
<tr><td>scaleMax</td><td>sclMax</td><td>float</td><td>Self explanatory.</td></tr>
<tr><td>springMode</td><td>sprMode</td><td>enum</td><td>Samples spring mode- UScale, UScaleInverse, UMidScaleInverse, UTugOffset, UTugScale.</td></tr>
<tr><td>springStrength</td><td>sprStrength</td><td>float</td><td>spring strength.</td></tr>
<tr><td>springDamp</td><td>sprDamp</td><td>float</td><td>Spring damping factor.</td></tr>
<tr><td>springStiffness</td><td>sprStiffness</td><td>float</td><td>Spring stiffness factor.</td></tr>
<tr><td>goalMatrix</td><td>goalMatrix</td><td>matrix</td><td>Spring goal matrix.</td></tr>
<tr><td>doSpring</td><td>doSpr</td><td>bool</td><td>Do spring calculation.</td></tr>
<tr><td>time</td><td>time</td><td>time</td><td>Input time value.</td></tr>
<tr><td>customPosition</td><td>customPosition</td><td>compound</td><td>Custom tweakers input transforms array.</td></tr>
<tr><td>uPosition</td><td>uPos</td><td>float</td><td>Custom tweaker U-Position. Child of customPositionOut.</td></tr>
<tr><td>twist</td><td>twist</td><td>float</td><td>Custom tweaker twist value. Child of customPositionOut.</td></tr>
<tr><td>aimRotation</td><td>aimRot</td><td>float</td><td>Custom tweaker aim-rotation value. Child of customPositionOut.</td></tr>
<tr><td>tertiaryRotation</td><td>tertiaryRot</td><td>float</td><td>Custom tweaker tertiary-rotation value. Child of customPositionOut.</td></tr>
<tr><td>scaleAim</td><td>sclAim</td><td>float</td><td>Custom tweaker aim-scale value. Child of customPositionOut.</td></tr>
<tr><td>scaleUp</td><td>sclUp</td><td>float</td><td>Custom tweaker up-scale value. Child of customPositionOut.</td></tr>
<tr><td>tertiaryScale</td><td>terScl</td><td>float</td><td>Custom tweaker tertiary-scale value. Child of customPositionOut.</td></tr>
<tr><td>falloff</td><td>falloff</td><td>float</td><td>Custom tweaker falloff value. Child of customPositionOut.</td></tr>
</table></font>
<font color = #5f5f5f size = 3pt><b>Outputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>transforms</td><td>transforms</td><td>compound</td><td>Result transforms array.</td></tr>
<tr><td>translate</td><td>t</td><td>float[3]</td><td>Result transform translation values. Child of transforms.</td></tr>
<tr><td>rotate</td><td>r</td><td>angle[3]</td><td>Result rotation translation values. Child of transforms.</td></tr>
<tr><td></td><td></td><td>matrix</td><td>Result matrix. Child of transforms.</td></tr>
<tr><td>scale</td><td>s</td><td>float[3]</td><td>Result scale translation values. Child of transforms.</td></tr>
<tr><td>customPositionOut</td><td>cusPosOut</td><td>compound</td><td>Custom tweakers offset transformation values array.</td></tr>
<tr><td>cusTranslate</td><td>cusT</td><td>float[3]</td><td>Custom tweakers offset translation values. Child of customPositionOut.</td></tr>
<tr><td>cusRotate</td><td>cusR</td><td>angle[3]</td><td>Custom tweakers offset rotation values. Child of customPositionOut.</td></tr>
</table></font>
<body>
##mnsPoseBlend
<hr width = 100%>
<body>
##mnsQuaternionBlend
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur ===
<br>
</i></font>
<hr width = 100%>
<font color = #5f5f5f size = 3pt><b>Inputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>inMatrix1</td><td>inMatrix1</td><td>matrix</td><td> Input matrix1. Blend source A.</td></tr>
<tr><td>inMatrix2</td><td>inMatrix2</td><td>matrix</td><td> Input matrix1. Blend source B.</td></tr>
</table></font>
<font color = #5f5f5f size = 3pt><b>Outputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>rotate</td><td>r</td><td>angle[3]</td><td>Rotation output.</td></tr>
</table></font>
<body>
##mnsRemapFloatArray
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur ===
<br>
This simple node will take the input value (as float or angle) and split and remap the values across the requested output count, based on the given values map graph attribute.
<br>
The value can also be re-ranged between two values, using the remapToRnage attributes given.
<br>
The input value plug will accept floats, doubles and angles (genericAttr).
<br>
The output plug will be set according to the input type given.
<br>
</i></font>
<hr width = 100%>
<font color = #5f5f5f size = 3pt><b>Inputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>valuesMap</td><td>valuesMap</td><td>float(array)</td><td>Output values remap graph.</td></tr>
<tr><td>value</td><td>value</td><td>float</td><td>Input value to remap. Can be float, double and angle.</td></tr>
<tr><td>angleOutputAsDegrees</td><td>angleOutputAsDegrees</td><td>bool</td><td>In case the input is set to angle, if this is set to true, the output values will be in degrees instead of the original radians input.</td></tr>
<tr><td>remapToRange</td><td>remapToRange</td><td>bool</td><td>A choice to remap the outputs to a new range, using the relevant attributes.</td></tr>
<tr><td>outputCount</td><td>outputCount</td><td>int</td><td>The amount of outputs to remap the input value to.</td></tr>
<tr><td>min</td><td>min</td><td>float</td><td>RemapToRnage new minimum value.</td></tr>
<tr><td>max</td><td>max</td><td>float</td><td>RemapToRnage new maximum value.</td></tr>
<tr><td>oldMin</td><td>oldMin</td><td>float</td><td>RemapToRnage old minimum value.</td></tr>
<tr><td>oldMax</td><td>oldMax</td><td>float</td><td>RemapToRnage old maximum value.</td></tr>
</table></font>
<font color = #5f5f5f size = 3pt><b>Outputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>outValue</td><td>outValue</td><td>float</td><td>Output values array.</td></tr>
</table></font>
<body>
##mnsResampleCurve
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur ===
<br>
A simple light weight curve re-sampler.
<br>
Primaraly used to embed mnsThreePointArc into an IK setup.
<br>
</i></font>
<hr width = 100%>
<font color = #5f5f5f size = 3pt><b>Inputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>resampleMode</td><td>resampleMode</td><td>enum</td><td>Reample mode- parametric, uniform.</td></tr>
<tr><td>degree</td><td>degree</td><td>int</td><td>Reample degree.</td></tr>
<tr><td>sections</td><td>sections</td><td>int</td><td>Reample amount of sections.</td></tr>
<tr><td>inputCurve</td><td>inputCurve</td><td>nurbsCurve</td><td>Input curve to re-sample.</td></tr>
</table></font>
<font color = #5f5f5f size = 3pt><b>Outputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>outCurve</td><td>outCurve</td><td>nurbsCurve</td><td>Result curve.</td></tr>
</table></font>
<body>
##mnsSimpleRivets
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur ===
<br>
This is a simple mesh rivet node.
<br>
This node will take any amount of input start position as matrix and will compile a transformation matrix for the closest face center position on the given input mesh.
<br>
This node will output the result in world space, unless an inpur targetParentInverseMatrix is plugged into the relevant element.
<br>
The deafult output will be the closest face center transformation matrix unless maintainOffset is set to ON- then the offset will be calculated and stored resulting in the same transformation matrix as the startPosition at bind.
<br>
Live mode should only be used for debugging purposes as this will initiate the nodes initialization process on every evaluation- impacting the nodes performance significantly.
<br>
The initialization process will be performed from from the given input mesh, unless a base mesh is plugged in to baseMesh plug.
<br>
It is recommended to avoid keeping baseMesh and startPosition plugs live.
<br>
</i></font>
<hr width = 100%>
<font color = #5f5f5f size = 3pt><b>Inputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>mesh</td><td>mesh</td><td>mesh</td><td>Input mesh to rivet to.</td></tr>
<tr><td>positionMode</td><td>positionMode</td><td>int</td><td> position mode. 0 is closest face center, 1 is closest vertex</td></tr>
<tr><td>upMode</td><td>upMode</td><td>int</td><td> up mode. 0 is closest vertex, 1 is input up matrix.</td></tr>
<tr><td>upMatrix</td><td>upMatrix</td><td>int</td><td> Up matrix to use in case upMode is set to 1.</td></tr>
<tr><td>targetWorldMatrix</td><td>targetWorldMatrix</td><td>matrix</td><td>Input mesh world matrix.</td></tr>
<tr><td>rivet</td><td>rivet</td><td>compound (Array)</td><td>Input rivets compound array.</td></tr>
<tr><td>rivetStartPosition</td><td>rivetStartPosition</td><td>matrix</td><td>Input start position. Rivet position will be calculated from this origin matrix.</td></tr>
<tr><td>targetParentInverseMatrix</td><td>targetParentInverseMatrix</td><td>matrix</td><td>Target transform parent inverse matrix. Use when output result is needed in local space (connect the target transform parentInverseMatrix plug)</td></tr>
<tr><td>liveMode</td><td>liveMode</td><td>bool</td><td>Live mode. Calculate everything in every evaluation.</td></tr>
<tr><td>maintainOffset</td><td>maintainOffset</td><td>bool</td><td>Maintain offset between rivet position and target mesh.</td></tr>
</table></font>
<font color = #5f5f5f size = 3pt><b>Outputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>translate</td><td>t</td><td>float[3]</td><td>Translation output. Child of transform.</td></tr>
<tr><td>rotate</td><td>r</td><td>angle[3]</td><td>Rotation output. Child of transform.</td></tr>
<tr><td>transform</td><td>transform</td><td>compound</td><td>Output transforms array.</td></tr>
<tr><td>scale</td><td>s</td><td>angle[3]</td><td>Scale output. Child of transform.</td></tr>
<tr><td>baseMesh</td><td>baseMesh</td><td>mesh</td><td>Input base-mesh.</td></tr>
</table></font>
<body>
##mnsSimpleSquash
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur ===
<br>
This simple node is designed to output a scale value to squash and stretch a given single transform value.
<br>
Based on the creation distance between the target and source matricies, the scale values will be calculated using a squash/stretch algorithm using the dynamic distance (or current distance).
<br>
All input values will be taken into account calculating the result.
<br>
The static arc length is the creation length. This value can be set manually if needed, although the node will set this value in it's initialization stage- in case the source and handle matricies where connected.
<br>
This value will be set automatically only once, in case this value needs to be changed it will need to be set manually.
<br>
Aim axis attribute- stretch value will be set to the aim axis selection, squash value will be set to the remaining axes.
<br>
Global scale attribute - this attribute is set to scale the static arc length to avoid unwanted scaling issues when aiming for a uniform scale of the target transform.
<br>
</i></font>
<hr width = 100%>
<font color = #5f5f5f size = 3pt><b>Inputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>handleWorldMatrix</td><td>handleWorldMatrix</td><td>matrix</td><td>Input handle world matrix.</td></tr>
<tr><td>squashRootWorldMatrix</td><td>squashRootWorldMatrix</td><td>matrix</td><td>Input squash root position world matrix.</td></tr>
<tr><td>squashFactor</td><td>squashFactor</td><td>float</td><td>Input squash factor.</td></tr>
<tr><td>stretchFactor</td><td>stretchFactor</td><td>float</td><td>Input stretch factor.</td></tr>
<tr><td>stretchMin</td><td>stretchMin</td><td>float</td><td>Input minimum stretch value.</td></tr>
<tr><td>stretchMax</td><td>stretchMax</td><td>float</td><td>Input maximum stretch value.</td></tr>
<tr><td>squashMin</td><td>squashMin</td><td>float</td><td>Input maximum squash value.</td></tr>
<tr><td>squashMax</td><td>squashMax</td><td>float</td><td>Input minimum squash value.</td></tr>
<tr><td>staticArcLength</td><td>staticArcLength</td><td>float</td><td>Static arc length / creation length value.</td></tr>
<tr><td>aimAxis</td><td>aimAxis</td><td>enum</td><td>Aim axis- stretch value will be set to the aim axis selection, squash value will be set to the remaining axes.</td></tr>
<tr><td>globalScale</td><td>globalScale</td><td>float</td><td>Global scale multiplier value.</td></tr>
</table></font>
<font color = #5f5f5f size = 3pt><b>Outputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>scale</td><td>s</td><td>float[3]</td><td>Output scale result.</td></tr>
<tr><td>arcLength</td><td>arcLength</td><td>float</td><td>Current arc length.</td></tr>
</table></font>
<body>
##mnsSphereRoll
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur ===
<br>
This node was created to deal with a ball/sphere rolling.
<br>
As oposed to common solutions, this node will evaluate the rotation of the target based on it's previous state, resulting in a non-gimble solution.
<br>
This node will solve the rotation for the current time.
<br>
Since ball rolling is a non-deterministic solution, this node will consider the previous state of the target transform to solve for the best posssible rotation given the input values.
<br>
Best used for a simple ball rolling on the ground, or a BB-8 style character, where the charcter's movements are rotation (roll) based.
<br>
</i></font>
<hr width = 100%>
<font color = #5f5f5f size = 3pt><b>Inputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>globalScale</td><td>globalScale</td><td>double</td><td>MObject  MnsSphereRoll::aGlobalScale</td></tr>
<tr><td>speedMultiplier</td><td>speedMultiplier</td><td>double</td><td> a global keyable multiplier to offset the solve. 1 is even, less then 1 will result in a backspin, greater then one will result in a topspin.</td></tr>
<tr><td>sphereRadius</td><td>sphereRadius</td><td>double</td><td> The radius of the traget sphere to rotate.</td></tr>
<tr><td>driverWorldMatrix</td><td>driverWorldMatrix</td><td>matrix</td><td> This matrix will be sampled in order to evaluate the transition to the next calculation. This should be the target transform for the output rotation.</td></tr>
<tr><td>upVectorWorldMatrix</td><td>upVectorWorldMatrix</td><td>matrix</td><td> This up vector direction will be calculated in relation to the input driver world matrix.</td></tr>
<tr><td>startFrame</td><td>startFrame</td><td>int</td><td>Evaluation start frame.</td></tr>
<tr><td>startFrameFromRange</td><td>startFrameFromRange</td><td>bool</td><td>If true, take the start frame from current maya range instead of the input value given.</td></tr>
<tr><td>time</td><td>time</td><td>time</td><td>Time input.</td></tr>
</table></font>
<font color = #5f5f5f size = 3pt><b>Outputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>outRotation</td><td>outRotation</td><td>vector</td><td>MObject  MnsSphereRoll::aOutRotation</td></tr>
</table></font>
<body>
##mnsSphereVectorPush
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur ===
<br>
Presenting mnsSphereVectorPush deformer.
<br>
This deformer was purpose built for the Eye-Meniscus deformation, but can be used for many more applications.
<br>
As opposed to the commonly used "matrixCollision", mnsSphereVectorPush will also collide back faces and push them at a higher radius based on a thickness threshold (keyable).
<br>
The node will accept unlimited collider matrix inputs and will combine the deformations with ease.
<br>
The input radiuses and thicknesses can be varied and keyed to choice.
<br>
Implementing the mnsSphereVectorPush deformer within the eyelid setup will result in a natural looking deformation of the cornea and the eyelids.
<br>
This is the case for a closed eye pose as well- which will naturally suggest the eye aim even when it isn't seen, corresponding to real life behavior.
<br>
The deformer can also be used to represent the eye volume- pushing the eyelid verticies towards the eye surface, for extreme poses of which are not handled correctly by the "aroundCenterMatrix" of mnsCurveZip due to a range which exceeds the normalization.
<br>
</i></font>
<hr width = 100%>
<font color = #5f5f5f size = 3pt><b>Inputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>collideMatrix</td><td>collideMatrix</td><td>matrix</td><td>Input collision matrix.</td></tr>
<tr><td>radius</td><td>radius</td><td>matrix</td><td>Input collision radius.</td></tr>
<tr><td>thicknessCollide</td><td>thicknessCollide</td><td>bool</td><td>If true, collide against back-faces using the input threshold.</td></tr>
<tr><td>thicknessThreshold</td><td>thicknessThreshold</td><td>float</td><td>Backface avarage distance to collide against.</td></tr>
<tr><td>collider</td><td>collider</td><td>compound</td><td>Collision object input array.</td></tr>
<tr><td>collideMethod</td><td>collideMethod</td><td>enum</td><td>Collision method- matrix, position.</td></tr>
</table></font>
<body>
##mnsSpringCurve
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur ===
<br>
This node is used to achive simple secondary motion proceduraly.
<br>
Tihs node will accept an input curve and offset curves to act upon, and using the stiffness and damping graph attributes it will calculate a new curve with secondary motion embedded.
<br>
This is an evaluation node rather then a simulation. Time needs to be connected to the node in order to see it's effect.
<br>
</i></font>
<hr width = 100%>
<font color = #5f5f5f size = 3pt><b>Inputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>inputCurve</td><td>inputCurve</td><td>nurbsCurve</td><td>Input curve.</td></tr>
<tr><td>inputOffsetCurve</td><td>inputOffsetCurve</td><td>nurbsCurve</td><td>Input offset curve.</td></tr>
<tr><td>strength</td><td>strength</td><td>float</td><td>Global strength. 0 is do nothing.</td></tr>
<tr><td>preventStretching</td><td>preventStretching</td><td>bool</td><td>Calculate stretch prevention.</td></tr>
<tr><td>startFrame</td><td>startFrame</td><td>int</td><td>Evaluation start frame.</td></tr>
<tr><td>startFrameFromRange</td><td>startFrameFromRange</td><td>bool</td><td>If true, take the start frame from current maya range instead of the input value given.</td></tr>
<tr><td>time</td><td>time</td><td>time</td><td>Time input.</td></tr>
<tr><td>stiffness</td><td>stiffness</td><td>graph</td><td>Stiffness graph control.</td></tr>
<tr><td>damping</td><td>damping</td><td>graph</td><td>Damping graph control.</td></tr>
</table></font>
<font color = #5f5f5f size = 3pt><b>Outputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>outCurve</td><td>outCurve</td><td>nurbsCurve</td><td>Result curve.</td></tr>
<tr><td>outOffsetCurve</td><td>outOffsetCurve</td><td>nurbsCurve</td><td>Result offset curve.</td></tr>
</table></font>
<body>
##mnsThreePointArc
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur ===
<br>
This node was written to create a perfectly curved limb blend, instead of using common approaches like skinned curves, simulated tangents, scaled points, etc.
<br>
This method provides a very elegant way of enabling curvable limbs to animators, avoiding the use of Maya's 'makeThreePointCircularArc' which doesn't support a case where the 3 input points are collinear, nor any input curve or blending support.
<br>
Another major advantage of this node is the 'conformToMidPoint' attribute-
<br>
This attribute signals the algorithm to take the mid-point into consideration when drawing the edit points of the calculated arc, 'pinning' the elbow/knee in place when blending to the curved shape, even when the ratio between the 2 bones is not even (most cases).
<br>
The blend is triggered once with the attribute set to 'Off' - causing the knee to shift position completely- making it unusable in animation. Then, the blend is triggered when the attribute is 'On' and the knee is pinned in place, while the result curve edit points are being shifted based on the mid-point's position.
<br>
</i></font>
<hr width = 100%>
<font color = #5f5f5f size = 3pt><b>Inputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>point1</td><td>point1</td><td>matrix</td><td>Input position A.</td></tr>
<tr><td>point2</td><td>point2</td><td>matrix</td><td>Input position B.</td></tr>
<tr><td>point3</td><td>point3</td><td>matrix</td><td>Input position C.</td></tr>
<tr><td>blend</td><td>blend</td><td>float</td><td>Blend value.</td></tr>
<tr><td>blendSectionA</td><td>blendSectionA</td><td>float</td><td>Section A only blend value.</td></tr>
<tr><td>blendSectionB</td><td>blendSectionB</td><td>float</td><td>Section B only blend value.</td></tr>
<tr><td>swipeStart</td><td>swipeStart</td><td>float</td><td>Swipe blend from start value.</td></tr>
<tr><td>swipeStartFalloff</td><td>swipeStartFalloff</td><td>float</td><td>Swipe blend from start falloff value.</td></tr>
<tr><td>swipeMidToRoot</td><td>swipeMidToRoot</td><td>float</td><td>Swipe blend from mid to start value.</td></tr>
<tr><td>swipeMidToRootFalloff</td><td>swipeMidToRootFalloff</td><td>float</td><td>Swipe blend from mid to start falloff value.</td></tr>
<tr><td>swipeMidToEnd</td><td>swipeMidToEnd</td><td>float</td><td>Swipe blend from mid to end value.</td></tr>
<tr><td>swipeMidToEndFalloff</td><td>swipeMidToEndFalloff</td><td>float</td><td>Swipe blend from mid to end falloff value.</td></tr>
<tr><td>swipeEnd</td><td>swipeEnd</td><td>float</td><td>Swipe blend from end to start value.</td></tr>
<tr><td>swipeEndFalloff</td><td>swipeEndFalloff</td><td>float</td><td>Swipe blend from end to start falloff value.</td></tr>
<tr><td>collinearAction</td><td>collinearAction</td><td>enum</td><td>Collinear action choice- inputCurve, resample.</td></tr>
<tr><td>resampleMode</td><td>resampleMode</td><td>enum</td><td>If resmapling is chosen, use this mode to resample- parametric, uniform.</td></tr>
<tr><td>degree</td><td>degree</td><td>int</td><td>If resmapling is chosen, use this degree.</td></tr>
<tr><td>sections</td><td>sections</td><td>int</td><td>If resmapling is chosen, use this amount of sections.</td></tr>
<tr><td>conformMidPoint</td><td>conformMidPoint</td><td>bool</td><td>Use the mid point to enhance clending algorithm.</td></tr>
<tr><td>inputCurve</td><td>inputCurve</td><td>nurbsCurve</td><td>Input curve.</td></tr>
<tr><td>inputOffsetCurve</td><td>inputOffsetCurve</td><td>nurbsCurve</td><td>Input offset curve.</td></tr>
</table></font>
<font color = #5f5f5f size = 3pt><b>Outputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>outCurve</td><td>outCurve</td><td>nurbsCurve</td><td>Result Curve.</td></tr>
<tr><td>outOffsetCurve</td><td>outOffsetCurve</td><td>nurbsCurve</td><td>Result offset Curve.</td></tr>
<tr><td>center</td><td>center</td><td>float[3]</td><td>Result circle center point.</td></tr>
<tr><td>radius</td><td>radius</td><td>float</td><td>Result circle radius.</td></tr>
</table></font>
<body>
##mnsTransformSpring
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur ===
<br>
</i></font>
<hr width = 100%>
<font color = #5f5f5f size = 3pt><b>Inputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>inputWorldMatrix</td><td>inputWorldMatrix</td><td>float</td><td>MObject  MnsTransformSpring::aInputWorldMatrix</td></tr>
<tr><td>targetParentInverseMatrix</td><td>targetParentInverseMatrix</td><td>float</td><td>MObject  MnsTransformSpring::aTargetParentInverseMatrix</td></tr>
<tr><td>strength</td><td>strength</td><td>float</td><td>Global strength. 0 is do nothing.</td></tr>
<tr><td>startFrame</td><td>startFrame</td><td>int</td><td>Evaluation start frame.</td></tr>
<tr><td>startFrameFromRange</td><td>startFrameFromRange</td><td>bool</td><td>If true, take the start frame from current maya range instead of the input value given.</td></tr>
<tr><td>time</td><td>time</td><td>time</td><td>Time input.</td></tr>
<tr><td>stiffness</td><td>stiffness</td><td>graph</td><td>Stiffness graph control.</td></tr>
<tr><td>damping</td><td>damping</td><td>graph</td><td>Damping graph control.</td></tr>
</table></font>
<font color = #5f5f5f size = 3pt><b>Outputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>translate</td><td>t</td><td>float</td><td>MObject  MnsTransformSpring::aOutTranslate</td></tr>
</table></font>
<body>
##mnsVolumeJoint
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur ===
<br>
</i></font>
<hr width = 100%>
<font color = #5f5f5f size = 3pt><b>Inputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>globalScale</td><td>globalScale</td><td>double</td><td>Global scale multiplier.</td></tr>
<tr><td>parentJointWorldMatrix</td><td>parentJointWorldMatrix</td><td>matrix</td><td> Input parent joint world Matrix. Angle source-A.</td></tr>
<tr><td>childJointWorldMatrix</td><td>childJointWorldMatrix</td><td>matrix</td><td> Input child joint world Matrix. Angle source-B.</td></tr>
<tr><td>childJointRestWorldMatrix</td><td>childJointRestWorldMatrix</td><td>matrix</td><td> Input child joint rest matrix. This will dictate the zero position for the calculation.</td></tr>
<tr><td>volumeJoint</td><td>volumeJoint</td><td>compound array</td><td> Input array compound for a volume joint calculation. Unlimited.</td></tr>
<tr><td>restTranslate</td><td>restTranslate</td><td>vector[3]</td><td> Rest translation values.</td></tr>
<tr><td>posXTranslate</td><td>posXTranslate</td><td>vector[3]</td><td> Positive X angle translation values.</td></tr>
<tr><td>negXTranslate</td><td>negXTranslate</td><td>vector[3]</td><td> Negative X angle translation values.</td></tr>
<tr><td>posYTranslate</td><td>posYTranslate</td><td>vector[3]</td><td> Positive Y angle translation values.</td></tr>
<tr><td>negYTranslate</td><td>negYTranslate</td><td>vector[3]</td><td> Negative Y angle translation values.</td></tr>
<tr><td>posZTranslate</td><td>posZTranslate</td><td>vector[3]</td><td> Positive Z angle translation values.</td></tr>
<tr><td>negZTranslate</td><td>negZTranslate</td><td>vector[3]</td><td> Negative Z angle translation values.</td></tr>
<tr><td>posXScale</td><td>posXScale</td><td>vector[3]</td><td> Positive X angle scale values.</td></tr>
<tr><td>negXScale</td><td>negXScale</td><td>vector[3]</td><td> Negative X angle scale values.</td></tr>
<tr><td>posYScale</td><td>posYScale</td><td>vector[3]</td><td> Positive Y angle scale values.</td></tr>
<tr><td>negYScale</td><td>negYScale</td><td>vector[3]</td><td> Negative Y angle scale values.</td></tr>
<tr><td>posZScale</td><td>posZScale</td><td>vector[3]</td><td> Positive Z angle scale values.</td></tr>
<tr><td>negZScale</td><td>negZScale</td><td>vector[3]</td><td> Negative Z angle scale values.</td></tr>
<tr><td>rotationBlend</td><td>rotationBlend</td><td>double</td><td> Rotation blend between the 2 sources (parent and child joints) for this volume joint. 0 is parent rotation, 1 is child rotation.</td></tr>
<tr><td>parentInverseMatrix</td><td>parentInverseMatrix</td><td>matrix</td><td> Target joint's parent inverse matrix to be used to localize the output values.</td></tr>
</table></font>
<font color = #5f5f5f size = 3pt><b>Outputs</b></font><p>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Long-Name</font></b></td><td><b><font color = #4caf50>Short-Name</b></td><td><font color = #4caf50><b>Type</b></td><td><font color = #4caf50><b>Description</b></td></tr>
<tr><td>result</td><td>result</td><td>compound</td><td>Output transforms array.</td></tr>
<tr><td>translate</td><td>t</td><td>float[3]</td><td>Translation output. Child of transform.</td></tr>
<tr><td>rotate</td><td>r</td><td>angle[3]</td><td>Rotation output. Child of transform.</td></tr>
<tr><td>scale</td><td>s</td><td>angle[3]</td><td>Scale output. Child of transform.</td></tr>
<tr><td>posXState</td><td>posXState</td><td>double</td><td>Current Positive-X direction state, between 0 and 1.</td></tr>
<tr><td>negXState</td><td>negXState</td><td>double</td><td>Current Negative-X direction state, between 0 and 1.</td></tr>
<tr><td>posYState</td><td>posYState</td><td>double</td><td>Current Positive-Y direction state, between 0 and 1.</td></tr>
<tr><td>negYState</td><td>negYState</td><td>double</td><td>Current Negative-Y direction state, between 0 and 1.</td></tr>
<tr><td>posZState</td><td>posZState</td><td>double</td><td>Current Positive-Z direction state, between 0 and 1.</td></tr>
<tr><td>negZState</td><td>negZState</td><td>double</td><td>Current Negative-Z direction state, between 0 and 1.</td></tr>
</table></font>
