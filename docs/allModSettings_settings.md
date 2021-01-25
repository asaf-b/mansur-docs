<body>
#allModSettings Settings
<hr width = 100%>
##Attributes
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr>
<td>body</td>
<td></td>
<td>Main module name</td>
</tr></td>
<tr>
<td>blkSide</td>
<td>center</td>
<td>Module side</td>
</tr></td>
<tr>
<td>alpha</td>
<td>A</td>
<td>Module's Alpha id</td>
</tr></td>
<tr>
<td>isFacial</td>
<td>False</td>
<td>Choose whether this module is marked as a facial module. This attribute is going to be used by the Picker and ModuleVisUI tools to seperate controls/modules in a Body group and a Facial group.</td>
</tr></td>
<tr>
<td>symmetryType</td>
<td>3</td>
<td>Choose the mirror type for right side controls</td>
</tr></td>
<tr>
<td>controlsMultiplier</td>
<td>2.0</td>
<td>Scale multiplier for this module's controls</td>
</tr></td>
<tr>
<td>alongSurface</td>
<td></td>
<td>Input surface to attach all joints within this module to the selected surface when constructing the rig. NurbsSurface is recommended</td>
</tr></td>
<tr>
<td>doGimbleCtrls</td>
<td>False</td>
<td>Not implemented currently</td>
</tr></td>
<tr>
<td>doPivotCtrls</td>
<td>False</td>
<td>Not implemented currently</td>
</tr></td>
<tr>
<td>postSymmetryJntStruct</td>
<td>False</td>
<td>If this attribute is set to true, a joint structure re-build will be initiated after this module is symmetrized</td>
</tr></td>
<tr>
<td>doAttributeHostCtrl</td>
<td>False</td>
<td>If this is set to True, a new attribute host control will be created along with this module in the position set by it's guide. Depending on the module, all relevant custom channel box attributes/contrls will be created on it for the sake of order and coherence controling the module</td>
</tr></td>
<tr>
<td>attributeHostControlShape</td>
<td>plus</td>
<td>The shape created for the attribute host control</td>
</tr></td>
<tr>
<td>spaces</td>
<td>[' ']</td>
<td>Depending on the module, all relevant space-switch controls will contain these spaces. Valid object types are Guides, Joints, and iterpJoints</td>
</tr></td>
<tr>
<td>splitOrientSpace</td>
<td>False</td>
<td>If this is set to True, all space switch attributes for this module will split into two spaces- Translate and Orient, for the animator to be able to set different space for tranlation and orientation.</td>
</tr></td>
<tr>
<td>colOverride</td>
<td>False</td>
<td>Override the main rig's color scheme for this module only</td>
</tr></td>
<tr>
<td>schemeOverride</td>
<td>[(0.0, 1.0, 0.0), (0.15, 1.0, 0.15), (0.3, 1.0, 0.3), (0.45, 1.0, 0.45), (0.6, 1.0, 0.6)]</td>
<td>Override with these colors</td>
</tr></td>
</table></font>
