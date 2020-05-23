<body>
#blockBuildUI
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur === <br>
MANSUR - BLOCK <br>
Main BLOCK UI. <br>
 <br>
This is the main UI for rig building (BLOCK). This is the essence of the entire library. <br>
This tool gathers all user actions, and defines triggers for edditing rigs. <br>
The main goal of this UI is to collect the available build-modules and draw creation buttons for them. <br>
The core module library is defined as the block library, but additionals paths can be inserted into the collect loop. <br>
 <br>
Many UI triggers are available in this UI, but many are kept external to the UI class, to keep things as clean and independent as possible. <br>
Most core functionalitites belong to the rig classes in 'buildModules'. <br>
 <br>
</font>
</i>
<hr width = 100%>
##Classes
<hr width = 100%>
<h5 id = "MnsBlockBuildUI TARGET"></h5>
###MnsBlockBuildUI [Class]
<font color = #5f5f5f size = 3pt>
<i>
BLOCK UI Class. <br>
</i>
<br>
</font>
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
<li>bmLib</li>
</ul>
</td></tr>
<tr><td><b><font color = #4caf50>Methods:  </font></b></td><td><ul>
<li><b><a href="#bmCategoryChangedTriggerTARGET">bmCategoryChangedTrigger </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#initializePrefDirsTARGET">initializePrefDirs </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#applyModulePathsChangeTARGET">applyModulePathsChange </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#moduleBuildGuideTARGET">moduleBuildGuide </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#addModulePathTARGET">addModulePath </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#connectSignalsTARGET">connectSignals </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#constructRigInitTARGET">constructRigInit </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#deconstructRigInitTARGET">deconstructRigInit </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#buildModulesDefineTARGET">buildModulesDefine </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#defineBuildParentModulesTARGET">defineBuildParentModules </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#extractControlShapesTARGET">extractControlShapes </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getCorrespondingModuleButtonForModuleTARGET">getCorrespondingModuleButtonForModule </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#gatherAdditionalModulePathsTARGET">gatherAdditionalModulePaths </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getConstructModeTARGET">getConstructMode </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getModuleSettingsTARGET">getModuleSettings </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#initializeAdditionalModulePathsTARGET">initializeAdditionalModulePaths </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#initViewTARGET">initView </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadModuleSettingsTARGET">loadModuleSettings </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadRigSettingsTARGET">loadRigSettings </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#duplicateModuleTARGET">duplicateModule </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#pureDuplicateTARGET">pureDuplicate </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#removeModelPathTARGET">removeModelPath </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#removeAllCustomShapesTARGET">removeAllCustomShapes </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#updateRigStructureTARGET">updateRigStructure </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#poseSaveLoadTriggerTARGET">poseSaveLoadTrigger </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadWindowTARGET">loadWindow </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getDefaultsModeTARGET">getDefaultsMode </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#symmetrizeModuleTARGET">symmetrizeModule </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#collectPartialModulesRootsTARGET">collectPartialModulesRoots </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#newRigTopTrigTARGET">newRigTopTrig </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#fixModulePathForRigTopTARGET">fixModulePathForRigTop </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#updateSettingsTARGET">updateSettings </b></a> <font size = 2pt><i>[method]</i></font></li>
</ul>
</td>
</tr>
</table></font>
####MnsBlockBuildUI  methods
<hr width = 50%>
<h5 id = "bmCategoryChangedTriggerTARGET"></h5><font color = 464646 size = 3><b>bmCategoryChangedTrigger <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>bmCategoryChangedTrigger(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "initializePrefDirsTARGET"></h5><font color = 464646 size = 3><b>initializePrefDirs <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>initializePrefDirs(self)</td></tr>
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
<font size = 2pt color= 595959><br>
<i>'Apply' (in build tab, module paths) trigger.</i><br>
<i>Write the additional paths entered within the UI in the stor json.</i><br>
</font>
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
<h5 id = "moduleBuildGuideTARGET"></h5><font color = 464646 size = 3><b>moduleBuildGuide <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Action trigger for any build-module button.</i><br>
<i>This trigger action will be connected procedurally within the 'drawModuleButton' method in blockUtility.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>moduleBuildGuide(self, listWidgetItemName)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>listWidgetItemName</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "addModulePathTARGET"></h5><font color = 464646 size = 3><b>addModulePath <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Add a module path line to the 'module paths' tree trigger.</i><br>
</font>
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
<h5 id = "connectSignalsTARGET"></h5><font color = 464646 size = 3><b>connectSignals <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Connect all UI signals.</i><br>
</font>
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
<h5 id = "constructRigInitTARGET"></h5><font color = 464646 size = 3><b>constructRigInit <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Construct trigger.</i><br>
</font>
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
<font size = 2pt color= 595959><br>
<i>Deconstruct trigger.</i><br>
</font>
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
<h5 id = "buildModulesDefineTARGET"></h5><font color = 464646 size = 3><b>buildModulesDefine <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Define all existing build-modules within a built tab's directory.</i><br>
<i>This mehthod will run for every valid build-module's directory folder, essentially building the actual build-module button in the UI.</i><br>
<i>These will all be stored in the 'buildModulesBtns' attribute of this class.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>buildModulesDefine(self, modParentPath, listWidget)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>modParentPath</b></li>
<li><b>listWidget</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "defineBuildParentModulesTARGET"></h5><font color = 464646 size = 3><b>defineBuildParentModules <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Define build module tabs, based on the collected valid build-modules directories.</i><br>
<i>If the directory in question is a valid directory for build modules:</i><br>
<i>for every folder containing modules within it, a new tab will be inserted and named based on it.</i><br>
</font>
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
<h5 id = "extractControlShapesTARGET"></h5><font color = 464646 size = 3><b>extractControlShapes <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Extract all control shapes from the current constructed rig, and store them for future re-construction.</i><br>
</font>
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
<h5 id = "getCorrespondingModuleButtonForModuleTARGET"></h5><font color = 464646 size = 3><b>getCorrespondingModuleButtonForModule <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>For the given rootGuide object, try to locate its corresponding UI button.</i><br>
<i>Look within this class's 'buildModulesBtns' attribute.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getCorrespondingModuleButtonForModule(self, rootGuide)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsBuildModuleBtn</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>rootGuide</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "gatherAdditionalModulePathsTARGET"></h5><font color = 464646 size = 3><b>gatherAdditionalModulePaths <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Gather all existing additional custom patns from the UI.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>gatherAdditionalModulePaths(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>list (Paths)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getConstructModeTARGET"></h5><font color = 464646 size = 3><b>getConstructMode <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Get current UI radio-buttons construction state (All/Branch/Module).</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getConstructMode(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>int (construction mode)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getModuleSettingsTARGET"></h5><font color = 464646 size = 3><b>getModuleSettings <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Get passed in module settings.</i><br>
<i>First get the default settings and values from the build-module directory,</i><br>
<i>then compare against the rootGuide attributes, and return the filtered and altered settings.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getModuleSettings(self, rootGuide, firstAttempt = True)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td> dict,int (optionalArguments, spilt index - for dynUI)</td></tr>
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
<h5 id = "initializeAdditionalModulePathsTARGET"></h5><font color = 464646 size = 3><b>initializeAdditionalModulePaths <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Initialize any custom build-modules paths that already exist within the data collect json.</i><br>
<i>(Read any paths that were added before, on UI draw).</i><br>
<i>query flag will return the paths only without drawing the items into the UI.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>initializeAdditionalModulePaths(self, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>list (Existing Paths)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "initViewTARGET"></h5><font color = 464646 size = 3><b>initView <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Initialize view:</i><br>
<i>- Set icons</i><br>
<i>- Set logger view</i><br>
<i>- Set tab index to 1</i><br>
<i>- Set-Up CollapsibleWidget view</i><br>
</font>
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
<h5 id = "loadModuleSettingsTARGET"></h5><font color = 464646 size = 3><b>loadModuleSettings <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Load selected module setting trigger.</i><br>
</font>
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
<h5 id = "loadRigSettingsTARGET"></h5><font color = 464646 size = 3><b>loadRigSettings <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Load selected rig settings trigger.</i><br>
</font>
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
<h5 id = "duplicateModuleTARGET"></h5><font color = 464646 size = 3><b>duplicateModule <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Module duplicate.</i><br>
<i>Gather all of the requested module's settings, as well as compare against the module's default settings.</i><br>
<i>Build a new module (same module) using the gathered data, then match all guide positions for the new module guide.</i><br>
</font>
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
<h5 id = "pureDuplicateTARGET"></h5><font color = 464646 size = 3><b>pureDuplicate <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Module duplicate.</i><br>
<i>Gather all of the requested module's settings, as well as compare against the module's default settings.</i><br>
<i>Build a new module (same module) using the gathered data.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>pureDuplicate(self, modRoot, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsBuildModule (New Module)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>modRoot</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "removeModelPathTARGET"></h5><font color = 464646 size = 3><b>removeModelPath <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Remove a module path line from the 'module paths' tree trigger.</i><br>
</font>
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
<h5 id = "removeAllCustomShapesTARGET"></h5><font color = 464646 size = 3><b>removeAllCustomShapes <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Remove all custom control shapes from the current rig.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>removeAllCustomShapes(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "updateRigStructureTARGET"></h5><font color = 464646 size = 3><b>updateRigStructure <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Rig structure update required trigger.</i><br>
<i>This method will be called in case any 'jntStructMember' attribute was altered, which means the internal joint structure of the module needs to be rebuilt.</i><br>
<i>This method will locate and filter the existing module related joint structure, destroy it, and re-build it using the updated settings. </i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>updateRigStructure(self, softMod = False, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>softMod</b>(<i>bool</i>) ; [default: False]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "poseSaveLoadTriggerTARGET"></h5><font color = 464646 size = 3><b>poseSaveLoadTrigger <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Save/Load pose trigger.</i><br>
<i>Simple method to gather pose data and store it, or apply it.</i><br>
</font>
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
<h5 id = "loadWindowTARGET"></h5><font color = 464646 size = 3><b>loadWindow <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Show window method.</i><br>
</font>
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
<h5 id = "getDefaultsModeTARGET"></h5><font color = 464646 size = 3><b>getDefaultsMode <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Simple method to get the current UI 'defaults' mode.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getDefaultsMode(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>int (defaults mode)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "symmetrizeModuleTARGET"></h5><font color = 464646 size = 3><b>symmetrizeModule <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Symmetrize module trigger.</i><br>
<i>Exclusive class member process.</i><br>
<i>This method will attempt to symmetrize the requested module guides.</i><br>
</font>
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
<h5 id = "collectPartialModulesRootsTARGET"></h5><font color = 464646 size = 3><b>collectPartialModulesRoots <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>This method will be called in case a partial build was requested.</i><br>
<i>Using methods within 'blockUtility', this method will collect the requested modules to build based on the UI state.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>collectPartialModulesRoots(self, mode)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td> list (root guides (modules) to build)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>mode</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "newRigTopTrigTARGET"></h5><font color = 464646 size = 3><b>newRigTopTrig <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Utils->'New RigTop' trigger.</i><br>
<i>deselect, then initialize a MnsRig class.</i><br>
</font>
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
<h5 id = "fixModulePathForRigTopTARGET"></h5><font color = 464646 size = 3><b>fixModulePathForRigTop <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Wrapper for 'attemptModulePathFixFroRigTop' in blockUtility.</i><br>
<i>Loop through all existing modules within the rig, and try and locate their module directory.</i><br>
<i>In case a directory wan't found for a build module, attempt to locate it's absolute dirctory by its name in the knowen paths.</i><br>
</font>
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
<h5 id = "updateSettingsTARGET"></h5><font color = 464646 size = 3><b>updateSettings <font size = 2pt> [<a href="#MnsBlockBuildUI TARGET">MnsBlockBuildUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>update setting trigger. This method will apply when a user altered any data within a setting window and chose to apply the changes.</i><br>
<i>The current settings will be validated against the default settings, and in case any data changed,</i><br>
<i>all neccessary actions will be called to apply and store the changes.</i><br>
</font>
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
