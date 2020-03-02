<body>
#blockBuildUI
<hr width = 100%>
##Classes
<hr width = 100%>
<h5 id = "MnsBlockBuildUI TARGET"></h5>
###MnsBlockBuildUI [Class]
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>MnsBlockBuildUI(<b>parent</b>(<i>str</i>) ; [default: mnsUIUtils.get_maya_window()])</td></tr>
<tr><td><b><font color = #4caf50>Inherits from:  </font></b></td><td>form_class, base_class</td></tr>
<tr><td><b><font color = #4caf50>Class Members:  </font></b></td>
<td><ul>
<ul>
<li>iconsDir</li>
<li>tabIndex</li>
<li>buildModulesBtns</li>
<li>sidePlaceHolder</li>
</ul>
</td></tr>
<tr><td><b><font color = #4caf50>Methods:  </font></b></td><td><ul>
<li><b><a href="#addModulePathTARGET">addModulePath </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#applyModulePathsChangeTARGET">applyModulePathsChange </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#connectSignalsTARGET">connectSignals </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#defineBuildParentModulesTARGET">defineBuildParentModules </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#duplicateModuleTARGET">duplicateModule </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#fixModulePathForRigTopTARGET">fixModulePathForRigTop </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#gatherAdditionalModulePathsTARGET">gatherAdditionalModulePaths </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getConstructModeTARGET">getConstructMode </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#initViewTARGET">initView </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadRigSettingsTARGET">loadRigSettings </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadWindowTARGET">loadWindow </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#newRigTopTrigTARGET">newRigTopTrig </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#removeModelPathTARGET">removeModelPath </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#symmetrizeModuleTARGET">symmetrizeModule </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#constructRigInitTARGET">constructRigInit </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#deconstructRigInitTARGET">deconstructRigInit </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#extractControlShapesTARGET">extractControlShapes </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#initializeAdditionalModulePathsTARGET">initializeAdditionalModulePaths </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#poseSaveLoadTriggerTARGET">poseSaveLoadTrigger </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#updateRigStructureTARGET">updateRigStructure </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#updateSettingsTARGET">updateSettings </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#moduleBuildGuideTARGET">moduleBuildGuide </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadModuleSettingsTARGET">loadModuleSettings </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#buildModulesDefineTARGET">buildModulesDefine </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#pureDuplicateTARGET">pureDuplicate </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#collectPartialModulesRootsTARGET">collectPartialModulesRoots </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getCorrespondingModuleButtonForModuleTARGET">getCorrespondingModuleButtonForModule </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getModuleSettingsTARGET">getModuleSettings </b></a> <font size = 2pt><i>[method]</i></font></li>
</ul>
</td>
</tr>
</table></font>
####MnsBlockBuildUI  methods
<hr width = 50%>
<h5 id = "addModulePathTARGET"></h5><font color = 464646 size = 3><b>addModulePath <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>addModulePath(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "applyModulePathsChangeTARGET"></h5><font color = 464646 size = 3><b>applyModulePathsChange <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>applyModulePathsChange(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "connectSignalsTARGET"></h5><font color = 464646 size = 3><b>connectSignals <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>connectSignals(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "defineBuildParentModulesTARGET"></h5><font color = 464646 size = 3><b>defineBuildParentModules <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>defineBuildParentModules(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "duplicateModuleTARGET"></h5><font color = 464646 size = 3><b>duplicateModule <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>duplicateModule(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "fixModulePathForRigTopTARGET"></h5><font color = 464646 size = 3><b>fixModulePathForRigTop <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>fixModulePathForRigTop(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "gatherAdditionalModulePathsTARGET"></h5><font color = 464646 size = 3><b>gatherAdditionalModulePaths <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>gatherAdditionalModulePaths(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getConstructModeTARGET"></h5><font color = 464646 size = 3><b>getConstructMode <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getConstructMode(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "initViewTARGET"></h5><font color = 464646 size = 3><b>initView <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>initView(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "loadRigSettingsTARGET"></h5><font color = 464646 size = 3><b>loadRigSettings <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadRigSettings(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "loadWindowTARGET"></h5><font color = 464646 size = 3><b>loadWindow <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadWindow(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "newRigTopTrigTARGET"></h5><font color = 464646 size = 3><b>newRigTopTrig <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>newRigTopTrig(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "removeModelPathTARGET"></h5><font color = 464646 size = 3><b>removeModelPath <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>removeModelPath(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "symmetrizeModuleTARGET"></h5><font color = 464646 size = 3><b>symmetrizeModule <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>symmetrizeModule(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "constructRigInitTARGET"></h5><font color = 464646 size = 3><b>constructRigInit <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>constructRigInit(self, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "deconstructRigInitTARGET"></h5><font color = 464646 size = 3><b>deconstructRigInit <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>deconstructRigInit(self, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "extractControlShapesTARGET"></h5><font color = 464646 size = 3><b>extractControlShapes <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>extractControlShapes(self, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "initializeAdditionalModulePathsTARGET"></h5><font color = 464646 size = 3><b>initializeAdditionalModulePaths <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>initializeAdditionalModulePaths(self, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "poseSaveLoadTriggerTARGET"></h5><font color = 464646 size = 3><b>poseSaveLoadTrigger <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>poseSaveLoadTrigger(self, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "updateRigStructureTARGET"></h5><font color = 464646 size = 3><b>updateRigStructure <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>updateRigStructure(self, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "updateSettingsTARGET"></h5><font color = 464646 size = 3><b>updateSettings <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>updateSettings(self, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "moduleBuildGuideTARGET"></h5><font color = 464646 size = 3><b>moduleBuildGuide <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>moduleBuildGuide(self, MnsBuildModuleButton)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>MnsBuildModuleButton</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "loadModuleSettingsTARGET"></h5><font color = 464646 size = 3><b>loadModuleSettings <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadModuleSettings(self, firstAttempt = True)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>firstAttempt</b>(<i>bool</i>) ; [default: True]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "buildModulesDefineTARGET"></h5><font color = 464646 size = 3><b>buildModulesDefine <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>buildModulesDefine(self, modParentPath, dirLayout)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>modParentPath</b></li>
<li><b>dirLayout</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "pureDuplicateTARGET"></h5><font color = 464646 size = 3><b>pureDuplicate <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>pureDuplicate(self, modRoot)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>modRoot</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "collectPartialModulesRootsTARGET"></h5><font color = 464646 size = 3><b>collectPartialModulesRoots <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>collectPartialModulesRoots(self, mode)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>mode</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getCorrespondingModuleButtonForModuleTARGET"></h5><font color = 464646 size = 3><b>getCorrespondingModuleButtonForModule <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getCorrespondingModuleButtonForModule(self, rootGuide)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>rootGuide</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getModuleSettingsTARGET"></h5><font color = 464646 size = 3><b>getModuleSettings <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getModuleSettings(self, rootGuide, firstAttempt = True)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>rootGuide</b></li>
<li><b>firstAttempt</b>(<i>bool</i>) ; [default: True]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
