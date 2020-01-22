<body>
#blockUtility
<hr width = 100%>
##Defenitions
<hr width = 100%>
###alignPLGuides
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>alignPLGuides(border = "left", mode = 0)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>border</b>(<i>str</i>) ; [default: "left"]</li>
<li><b>mode</b>(<i>int</i>) ; [default: 0]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###attemptModulePathFixFroRigTop
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>attemptModulePathFixFroRigTop(rigTop, existingBtns)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rigTop</b></li>
<li><b>existingBtns</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###autoHierarchyPlgs
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>autoHierarchyPlgs(rigTop, overrideCbx = False, autoH = True)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rigTop</b></li>
<li><b>overrideCbx</b>(<i>bool</i>) ; [default: False]</li>
<li><b>autoH</b>(<i>bool</i>) ; [default: True]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###collectGuides
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>collectGuides(roots = pm.ls(sl = 1), **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>roots</b>(<i>str</i>) ; [default: selection]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
<td><ul>
<li><b>rigTop</b>(<i>str</i>) ; [default: None]</li>
<li><b>includeDecendents</b>(<i>bool</i>)</li>
<li><b>includeDecendentBranch</b>(<i>bool</i>)</li>
<li><b>getGuides</b>(<i>bool</i>) ; [default: True]</li>
<li><b>getCustomGuides</b>(<i>bool</i>) ; [default: True]</li>
<li><b>allAsSparse</b>(<i>bool</i>)</li>
</ul></td>
</tr>
</table></font>
<hr width = 100%>
###collectHierarchy
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>collectHierarchy(sel = [])</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>sel</b>(<i>list</i>) ; [default: []]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###collectPLGuidesToAlign
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>collectPLGuidesToAlign(mode = 0)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>mode</b>(<i>int</i>) ; [default: 0]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###connectSlaveToDeleteMaster
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>connectSlaveToDeleteMaster(slave, master)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>slave</b></li>
<li><b>master</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###createModuleTopNode
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createModuleTopNode(MnsBuildModuleA = None, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>MnsBuildModuleA</b>(<i>str</i>) ; [default: None]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###createOffsetGroup
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createOffsetGroup(transformObject, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>transformObject</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
<td><ul>
<li><b>type</b>(<i>str</i>) ; [default: offsetGrp]</li>
</ul></td>
</tr>
</table></font>
<hr width = 100%>
###createPickerLayoutGuide
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createPickerLayoutGuide(guide, override, rigTop, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>guide</b></li>
<li><b>override</b></li>
<li><b>rigTop</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###createPickerLayoutGuides
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createPickerLayoutGuides(guidesToProject, rigTop, msgPrompt = True, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>guidesToProject</b></li>
<li><b>rigTop</b></li>
<li><b>msgPrompt</b>(<i>bool</i>) ; [default: True]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###deletePoseForGuides
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>deletePoseForGuides(guides = [], poseSet = "T")</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>guides</b>(<i>list</i>) ; [default: []]</li>
<li><b>poseSet</b>(<i>str</i>) ; [default: "T"]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###deletePuppetName
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>deletePuppetName(rigTop, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rigTop</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###filterCreationOnlyFromArgs
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>filterCreationOnlyFromArgs(argsList)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>argsList</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###filterSettings
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>filterSettings(fileSettings, node)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>fileSettings</b></li>
<li><b>node</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getAllGuideRootsForRigTop
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getAllGuideRootsForRigTop(rigTop)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rigTop</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getAllPlgsForRigTop
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getAllPlgsForRigTop(rigTop)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rigTop</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getAllcolCtrlforRigTop
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getAllcolCtrlforRigTop(rigTop)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rigTop</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getChildModules
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getChildModules(rootGuide)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rootGuide</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getCtrlCol
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getCtrlCol(ctrl, rigTop)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>ctrl</b></li>
<li><b>rigTop</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getDeleteMasterFromSlave
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getDeleteMasterFromSlave(slave)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>slave</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getGuideParent
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getGuideParent(objectSel = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>objectSel</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getModuleDecendentsWildcard
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getModuleDecendentsWildcard(guideRoot, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>guideRoot</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getModuleFromGuide
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getModuleFromGuide(guideRoot, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>guideRoot</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
<td><ul>
<li><b>fileType</b>(<i>str</i>) ; [default: jntStruct]</li>
<li><b>modPath</b>(<i>str</i>) ; [default: None]</li>
<li><b>modName</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
</table></font>
<hr width = 100%>
###getModuleGuideDecendents
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getModuleGuideDecendents(guideRoot)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>guideRoot</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getModuleInterpJoints
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getModuleInterpJoints(guideRoot)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>guideRoot</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getModuleRoot
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getModuleRoot(objectA)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>objectA</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getModuleRootForSel
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getModuleRootForSel()</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getNodeRelationshipNodeFromObject
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getNodeRelationshipNodeFromObject(node)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>node</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getOffsetGrpForCtrl
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getOffsetGrpForCtrl(ctrl, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>ctrl</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
<td><ul>
<li><b>type</b>(<i>str</i>) ; [default: offsetGrp]</li>
</ul></td>
</tr>
</table></font>
<hr width = 100%>
###getPickerGuidesGrpFromRigTop
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getPickerGuidesGrpFromRigTop(rigTop = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rigTop</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getPickerLayoutBaseFromRigTop
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getPickerLayoutBaseFromRigTop(rigTop = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rigTop</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getPickerLayoutCamFromRigTop
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getPickerLayoutCamFromRigTop(rigTop = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rigTop</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getPickerProjectionCamFromRigTop
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getPickerProjectionCamFromRigTop(rigTop = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rigTop</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getPickerTitleGrpFromRigTop
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getPickerTitleGrpFromRigTop(rigTop = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rigTop</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getPuppetBaseFromRigTop
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getPuppetBaseFromRigTop(rigTop = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rigTop</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getPuppetRootFromRigTop
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getPuppetRootFromRigTop(rigTop = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rigTop</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getRelatedNodeFromObject
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getRelatedNodeFromObject(node)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>node</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getRelatedNodesFromObject
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getRelatedNodesFromObject(node)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>node</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getRelationMasterFromSlave
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getRelationMasterFromSlave(slave)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>slave</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getRigTop
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getRigTop(objectA)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>objectA</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getRigTopForSel
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getRigTopForSel()</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getRootGuideFromRigTop
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getRootGuideFromRigTop(rigTop = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rigTop</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getSettings
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getSettings(settingsPath, node, blkType)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>settingsPath</b></li>
<li><b>node</b></li>
<li><b>blkType</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getTreeFromGuideRoot
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getTreeFromGuideRoot(guideRoot = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>guideRoot</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###guidePickerGuideToggle
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>guidePickerGuideToggle()</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###hierarchyPlgsTrigger
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>hierarchyPlgsTrigger()</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###loadPerspCam
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadPerspCam()</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###loadPickerProjectionCam
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadPickerProjectionCam()</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###loadPoseForGuides
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadPoseForGuides(guides = [], poseSet = "T")</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>guides</b>(<i>list</i>) ; [default: []]</li>
<li><b>poseSet</b>(<i>str</i>) ; [default: "T"]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###missingModuleActionTrigger
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>missingModuleActionTrigger(rigTop, missingModuleName, existingBtns)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rigTop</b></li>
<li><b>missingModuleName</b></li>
<li><b>existingBtns</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###namePuppet
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>namePuppet(rigTop, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rigTop</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###pickerLayoutAdjust
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>pickerLayoutAdjust()</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###pickerTitleToggle
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>pickerTitleToggle()</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###preCheckNameForUI
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>preCheckNameForUI(arguments, suffix)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>arguments</b></li>
<li><b>suffix</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###projectAllPlg
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>projectAllPlg(msgPrompt = True, autoH = True)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>msgPrompt</b>(<i>bool</i>) ; [default: True]</li>
<li><b>autoH</b>(<i>bool</i>) ; [default: True]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###projectPickerLayoutPos
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>projectPickerLayoutPos(guide, cam, layoutBase)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>guide</b></li>
<li><b>cam</b></li>
<li><b>layoutBase</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###projectSelectedModulesPickerLayout
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>projectSelectedModulesPickerLayout(msgPrompt = True, autoH = True)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>msgPrompt</b>(<i>bool</i>) ; [default: True]</li>
<li><b>autoH</b>(<i>bool</i>) ; [default: True]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###projectSelectedPickerLayout
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>projectSelectedPickerLayout(msgPrompt = True, autoH = True)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>msgPrompt</b>(<i>bool</i>) ; [default: True]</li>
<li><b>autoH</b>(<i>bool</i>) ; [default: True]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###projectSelectedTreesPickerLayout
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>projectSelectedTreesPickerLayout(msgPrompt = True, autoH = True)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>msgPrompt</b>(<i>bool</i>) ; [default: True]</li>
<li><b>autoH</b>(<i>bool</i>) ; [default: True]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###removeAllAuthority
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>removeAllAuthority(slave = None, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>slave</b>(<i>str</i>) ; [default: None]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###saveLoadPose
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>saveLoadPose(guides = [], **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>guides</b>(<i>list</i>) ; [default: []]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
<td><ul>
<li><b>rigTop</b>(<i>str</i>) ; [default: None]</li>
<li><b>mode</b>(<i>int</i>) ; [default: 1]</li>
<li><b>saveLoad</b>(<i>int</i>)</li>
<li><b>msgPrompt</b>(<i>bool</i>)</li>
<li><b>pose</b>(<i>str</i>) ; [default: T]</li>
<li><b>delete</b>(<i>bool</i>)</li>
</ul></td>
</tr>
</table></font>
<hr width = 100%>
###savePoseForGuides
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>savePoseForGuides(guides = [], poseSet = "T", msgPrompt = False)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>guides</b>(<i>list</i>) ; [default: []]</li>
<li><b>poseSet</b>(<i>str</i>) ; [default: "T"]</li>
<li><b>msgPrompt</b>(<i>bool</i>) ; [default: False]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###setCtrlCol
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setCtrlCol(ctrl, rigTop, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>ctrl</b></li>
<li><b>rigTop</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###setgCtrlColorForModule
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setgCtrlColorForModule(rigTop, moduleRoot)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rigTop</b></li>
<li><b>moduleRoot</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###setgCtrlColorForRigTop
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setgCtrlColorForRigTop(rigTop)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rigTop</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###transferAuthorityToCtrl
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>transferAuthorityToCtrl(slave = None, ctrlMaster = None, **kwargs)	</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>slave</b>(<i>str</i>) ; [default: None]</li>
<li><b>ctrlMaster</b>(<i>str</i>) ; [default: None]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###upParentAllPlgTrigger
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>upParentAllPlgTrigger()</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
