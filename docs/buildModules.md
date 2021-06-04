<body>
#buildModules
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur === <br>
This is the core BLOCK Build-Modules class library. <br>
This package contains the three main classes for BLOCK: <br>
- MnsBuildModuleBtn <br>
- MnsRig <br>
- MnsBuildModule <br>
 <br>
Most core function are defined within the classes, although any external functionality is maintained in 'blockUtility' py module. <br>
The objective of these classes are mainly effeciant data gathering, constructing and deconstructing modules within a rig group. <br>
 <br>
</font>
</i>
<hr width = 100%>
##Classes
<hr width = 100%>
<h5 id = "MnsBuildModule TARGET"></h5>
###MnsBuildModule [Class]
<font color = #5f5f5f size = 3pt>
<i>
This class is the data store class for any mns 'build-module'. <br>
This class contains the actual creation and deletion of the module, guides and controls. <br>
This class will be initialized through the MnsRig class, althogh process functions regarding the modules are store in this class only. <br>
This class is purely procedular, and so it should remain. <br>
As the main goal of the rig is maintaining dynamic abilities, and easy creation of modules, <br>
this class should remain completely independent of any specific build module. <br>
Guides creation is partlly procedural, as any "main-guides" creation is fully automatic,  <br>
although custom-guides creation isn't- as it is module specific, hence it is store within the buildModule directory. <br>
Interp Joint Structure creation is procedural, although its essence is also defined within each build-module directory, althogh it is not mandatory. <br>
As the build modules are very specific and have to be created manually, guide creation is kept independent. <br>
This for easily creating modules, not needing to worrie about the handeling of guides, consruction and deconstruction. <br>
The actual flow of the build is independent of the modules setup internals. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>MnsBuildModule(<b>MnsBuildModuleButton</b>,<b>**kwargs</b>)</td></tr>
<tr><td><b><font color = #4caf50>Inherits from:  </font></b></td><td>MnsRig</td></tr>
<tr><td><b><font color = #4caf50>Class Members:  </font></b></td>
<td><ul>
<ul>
<li>MnsBuildModuleButton</li>
<li>sidePlaceHolder</li>
<li>builtGuides</li>
<li>rigTop</li>
<li>rootGuide</li>
<li>isFacial</li>
<li>rootCtrl</li>
<li>guideControls</li>
<li>cGuideControls</li>
<li>pureParent</li>
<li>attrHostCtrl</li>
<li>extraChannelsHost</li>
<li>moduleTop</li>
<li>animGrp</li>
<li>animStaticGrp</li>
<li>rigComponentsGrp</li>
<li>moduleSpaceAttrHost</li>
<li>extraSpaces</li>
<li>defaultSpace</li>
<li>pureTops</li>
<li>spaceSwitchCtrls</li>
<li>internalSpaces</li>
<li>controls</li>
<li>allControls</li>
<li>puppetTopCtrl</li>
</ul>
</td></tr>
<tr><td><b><font color = #4caf50>Methods:  </font></b></td><td><ul>
<li><b><a href="#constructAttrHostCtrlTARGET">constructAttrHostCtrl </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#createAttrHostCustomGuideTARGET">createAttrHostCustomGuide </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#createExtraChannelsTARGET">createExtraChannels </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#splitControlsBasedOnTypeTARGET">splitControlsBasedOnType </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#collecteModuleSettingsTARGET">collecteModuleSettings </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#buildGuideObjectsTARGET">buildGuideObjects </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#gatherAllDependeciesTARGET">gatherAllDependecies </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#reCollectControlsFromLocalsTARGET">reCollectControlsFromLocals </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#constructTARGET">construct </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#createGuidesTARGET">createGuides </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#deconstructTARGET">deconstruct </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#buildGuidesTARGET">buildGuides </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#constructSpacesTARGET">constructSpaces </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#createModuleTopNodeTARGET">createModuleTopNode </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#storeCustomDefaultsTARGET">storeCustomDefaults </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#updateCreationArgsToSymmetryModeTARGET">updateCreationArgsToSymmetryMode </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#restoreCustomDefaultsTARGET">restoreCustomDefaults </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#gatherRelatedCtrlsTARGET">gatherRelatedCtrls </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#connectVisChannelsTARGET">connectVisChannels </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#gatherRelatedGuidesTARGET">gatherRelatedGuides </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getRigTopTARGET">getRigTop </b></a> <font size = 2pt><i>[method]</i></font></li>
</ul>
</td>
</tr>
</table></font>
####MnsBuildModule  methods
<hr width = 50%>
<h5 id = "constructAttrHostCtrlTARGET"></h5><font color = 464646 size = 3><b>constructAttrHostCtrl <font size = 2pt> [<a href="#MnsBuildModule TARGET">MnsBuildModule </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>constructAttrHostCtrl(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "createAttrHostCustomGuideTARGET"></h5><font color = 464646 size = 3><b>createAttrHostCustomGuide <font size = 2pt> [<a href="#MnsBuildModule TARGET">MnsBuildModule </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createAttrHostCustomGuide(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "createExtraChannelsTARGET"></h5><font color = 464646 size = 3><b>createExtraChannels <font size = 2pt> [<a href="#MnsBuildModule TARGET">MnsBuildModule </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createExtraChannels(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "splitControlsBasedOnTypeTARGET"></h5><font color = 464646 size = 3><b>splitControlsBasedOnType <font size = 2pt> [<a href="#MnsBuildModule TARGET">MnsBuildModule </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>splitControlsBasedOnType(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "collecteModuleSettingsTARGET"></h5><font color = 464646 size = 3><b>collecteModuleSettings <font size = 2pt> [<a href="#MnsBuildModule TARGET">MnsBuildModule </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>collecteModuleSettings(self, rootGuide = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>rootGuide</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "buildGuideObjectsTARGET"></h5><font color = 464646 size = 3><b>buildGuideObjects <font size = 2pt> [<a href="#MnsBuildModule TARGET">MnsBuildModule </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>A simple method to gather the amount of needed guides to create, and calling the creation accordingly.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>buildGuideObjects(self, **kwargs)</td></tr>
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
<h5 id = "gatherAllDependeciesTARGET"></h5><font color = 464646 size = 3><b>gatherAllDependecies <font size = 2pt> [<a href="#MnsBuildModule TARGET">MnsBuildModule </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Gather all scene object dependecies for the buildModule.</i><br>
<i>A simple wrapper containing 'gatherRelatedGuides' method & gatherRelatedCtrls method.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>gatherAllDependecies(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "reCollectControlsFromLocalsTARGET"></h5><font color = 464646 size = 3><b>reCollectControlsFromLocals <font size = 2pt> [<a href="#MnsBuildModule TARGET">MnsBuildModule </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Re-initialize the 'allControls' attribute of this class, based on the current rig state.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>reCollectControlsFromLocals(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "constructTARGET"></h5><font color = 464646 size = 3><b>construct <font size = 2pt> [<a href="#MnsBuildModule TARGET">MnsBuildModule </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>The main construct method.</i><br>
<i>The actual 'Construct' method within the build module directory is being called here.</i><br>
<i>Flow:</i><br>
<i>- make sure the module isn't built</i><br>
<i>- get the puppet root</i><br>
<i>- try and find the related 'construct' method within the build module directory (or package).</i><br>
<i>- construct the module, feeding the construct method with all of the requested module settings.</i><br>
<i>  this will transfer the related joints to their new ctrl authority.</i><br>
<i>- connect a vis channel to the new module group created.</i><br>
<i>- re-collect relations for the module (post build).</i><br>
<i>- Set colors for all built controls.</i><br>
<i>- parent the new bm top group in the puppet group.</i><br>
<i>- try restore defaults if there are any.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>construct(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsBuildModule (self, this buildModule class)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "createGuidesTARGET"></h5><font color = 464646 size = 3><b>createGuides <font size = 2pt> [<a href="#MnsBuildModule TARGET">MnsBuildModule </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>This is the main guide creation method.</i><br>
<i>This method contains all the steps needed to gather a module data, and create the guides for it.</i><br>
<i>This method will return the built guides, as well as store it in this class 'builtGuides' attribute.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createGuides(self, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>list (bbuiltGuides)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
<td><ul>
<li><b>blkSide</b>(<i>str</i>) ; [default: center]</li>
<li><b>body</b>(<i>str</i>) ; [default: guideCtrl]</li>
<li><b>alpha</b>(<i>str</i>) ; [default: A]</li>
<li><b>alongAxis</b>(<i>int</i>) ; [default: 1]</li>
<li><b>moduleScale</b>(<i>int</i>) ; [default: 1]</li>
<li><b>isFacial</b>(<i>bool</i>)</li>
</ul></td>
</tr>
</table></font>
<h5 id = "deconstructTARGET"></h5><font color = 464646 size = 3><b>deconstruct <font size = 2pt> [<a href="#MnsBuildModule TARGET">MnsBuildModule </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>This is the main module deconstruction method.</i><br>
<i>Flow:</i><br>
<i>- Make sure the module is constructed</i><br>
<i>- In case a deconstruvt method (non mandatory method) is found within the build-module's directory, run it.</i><br>
<i>- Transfer all joint authoities back to the guides.</i><br>
<i>- Remove the related vis channel from puppet root (Needed in case a partial deconstruction was called).</i><br>
<i>- Delete the build module.</i><br>
<i>- Set the construction state for the build module.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>deconstruct(self, mnsRig)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsBuildModule (self, this buildModule class)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>mnsRig</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "buildGuidesTARGET"></h5><font color = 464646 size = 3><b>buildGuides <font size = 2pt> [<a href="#MnsBuildModule TARGET">MnsBuildModule </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>This method is the initialize method for new guides creation.</i><br>
<i>This method will be called first (before 'createGuides') and will also load the modules creation settings window if neccessary.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>buildGuides(self, MnsBuildModuleButton, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>MnsBuildModuleButton</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
<td><ul>
<li><b>skipUI</b>(<i>bool</i>)</li>
<li><b>skipGuidesCreation</b>(<i>bool</i>)</li>
<li><b>settingsHolder</b>(<i>str</i>) ; [default: None]</li>
<li><b>symmetrize</b>(<i>bool</i>)</li>
</ul></td>
</tr>
</table></font>
<h5 id = "constructSpacesTARGET"></h5><font color = 464646 size = 3><b>constructSpaces <font size = 2pt> [<a href="#MnsBuildModule TARGET">MnsBuildModule </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>This method is the spaces construction processing.</i><br>
<i>This method is seperated from the main construct method in order to run it after an entire construction.</i><br>
<i>Because the spaces within the module are dependent of other modules, a first loop is run to construct the modules,</i><br>
<i>after, another loop is running through the built modules, calling this method, trying to construct all of it's spaces.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>constructSpaces(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "createModuleTopNodeTARGET"></h5><font color = 464646 size = 3><b>createModuleTopNode <font size = 2pt> [<a href="#MnsBuildModule TARGET">MnsBuildModule </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>This method is used to create the genric 'module top group' on module construction.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createModuleTopNode(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "storeCustomDefaultsTARGET"></h5><font color = 464646 size = 3><b>storeCustomDefaults <font size = 2pt> [<a href="#MnsBuildModule TARGET">MnsBuildModule </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>This method stores any custom 'defaults' set for the entire module.</i><br>
<i>The collection is stored within the rootGuide node.</i><br>
<i>This is important beacuse when the module is deconstructed, the ctrls containing the 'defaults' attribute are eventually deleted.</i><br>
<i>So, in order to keep the information on deletion, this method runs thorugh the modules controls, </i><br>
<i>and storing the set 'defaults' attribute within the rootGuide, in order to restore them when a reconstruction is called.</i><br>
<i>related method: restoreCustomDefaults</i><br>
<i> </i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>storeCustomDefaults(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "updateCreationArgsToSymmetryModeTARGET"></h5><font color = 464646 size = 3><b>updateCreationArgsToSymmetryMode <font size = 2pt> [<a href="#MnsBuildModule TARGET">MnsBuildModule </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>This method will alter the current setting to their symmetry mode,</i><br>
<i>In case the 'symmetrize' flag was passed into the buildGuides method.</i><br>
<i>Altered attributes:</i><br>
<i>- side (or blkSide)</i><br>
<i>- spaces- if a side related space was found, symmetrize the space as well.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>updateCreationArgsToSymmetryMode(self, optArgs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>dict (optionalArguments)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>optArgs</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "restoreCustomDefaultsTARGET"></h5><font color = 464646 size = 3><b>restoreCustomDefaults <font size = 2pt> [<a href="#MnsBuildModule TARGET">MnsBuildModule </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>This method will attempt to restore any pre-stored 'defaults' set a newly created control.</i><br>
<i>related method: storeCustomDefaults.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>restoreCustomDefaults(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "gatherRelatedCtrlsTARGET"></h5><font color = 464646 size = 3><b>gatherRelatedCtrls <font size = 2pt> [<a href="#MnsBuildModule TARGET">MnsBuildModule </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>This method will collect and store the build-module related control objects from the rig.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>gatherRelatedCtrls(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "connectVisChannelsTARGET"></h5><font color = 464646 size = 3><b>connectVisChannels <font size = 2pt> [<a href="#MnsBuildModule TARGET">MnsBuildModule </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>This method will connect this module into it's related vis channel in the puppet root control.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>connectVisChannels(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "gatherRelatedGuidesTARGET"></h5><font color = 464646 size = 3><b>gatherRelatedGuides <font size = 2pt> [<a href="#MnsBuildModule TARGET">MnsBuildModule </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>This method will gather the buildModules related guides from the rig.</i><br>
<i>collected objects:</i><br>
<i>- rootGuide</i><br>
<i>- guides</i><br>
<i>- customGuides</i><br>
<i>The data collected is stored in their related class attributes:</i><br>
<i>- rootGuide - 'rootGuide'</i><br>
<i>- guides - 'guideControls'</i><br>
<i>- custom guides - 'cGuideControls'</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>gatherRelatedGuides(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getRigTopTARGET"></h5><font color = 464646 size = 3><b>getRigTop <font size = 2pt> [<a href="#MnsBuildModule TARGET">MnsBuildModule </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>get the rigTop nameStd from current selection. </i><br>
<i>If it doesn't exist, initiate a new rig top creation.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getRigTop(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsNameStd (rigTop)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
<h5 id = "MnsBuildModuleBtn TARGET"></h5>
###MnsBuildModuleBtn [Class]
<font color = #5f5f5f size = 3pt>
<i>
The procedural 'module' button class. <br>
This class is being called and constructed procedurally from the file system based on folder contents. <br>
The class itself isn't inhereting from QPushButton, as it only exists to contain build location information. <br>
The class contains a constuctor only, which initializes the following information: <br>
- The full-path to the buildModule  <br>
- The layout Parent of the button <br>
- The group of the button, based on the folder structure of which the bm is located in. <br>
- The 'settings' file-path. <br>
- Short-Name <br>
- The obselete - 'isMayaNative' attribute. <br>
This information will be accessed once the related QPushButton will be triggered. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>MnsBuildModuleBtn(<b>path</b>,<b>**kwargs</b>)</td></tr>
<tr><td><b><font color = #4caf50>Inherits from:  </font></b></td><td>object</td></tr>
<tr><td><b><font color = #4caf50>Class Members:  </font></b></td>
<td><ul>
<ul>
<li>path</li>
<li>moduleName</li>
<li>groupType</li>
</ul>
</td></tr>
</tr>
</table></font>
<hr width = 100%>
<h5 id = "MnsRig TARGET"></h5>
###MnsRig [Class]
<font color = #5f5f5f size = 3pt>
<i>
This is the main 'RIG' data class. <br>
This class's constructor will initialize and build all relevant information regarding the 'rig' top top group. <br>
As The rig topGrp has pre-defined structure, and many dependencies, all basic information will be checked every time this class is constructed. <br>
The essence of this class is first of all to build the predefined rigGroup, <br>
then, to store and parse all relevant data from the scene, as well as validating it and rebuilding any sub-components if necessary. <br>
The procedural settings UI build will be initiated if a rig top wasn't found in the current scene selection (or if there is no selection). <br>
In case a rigTop already exists, it will first be validated, then it's setting will be read and parsed, initiating the the same UI draw, in "edit" mode. <br>
  <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>MnsRig(<b>callerSubClass</b>(<i>str</i>) ; [default: None],<b>**kwargs</b>)</td></tr>
<tr><td><b><font color = #4caf50>Inherits from:  </font></b></td><td>object</td></tr>
<tr><td><b><font color = #4caf50>Class Members:  </font></b></td>
<td><ul>
<ul>
<li>rigTop</li>
<li>rootGuide</li>
<li>callerSubClass</li>
<li>modules</li>
<li>buildModulesBtns</li>
<li>puppetBase</li>
<li>baseGuide</li>
<li>rootJnt</li>
<li>iconsDir</li>
<li>loadSettingsWindow</li>
</ul>
</td></tr>
<tr><td><b><font color = #4caf50>Methods:  </font></b></td><td><ul>
<li><b><a href="#failedConstructionCommandTARGET">failedConstructionCommand </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setVisChannelsBasedOnCunstructModeTARGET">setVisChannelsBasedOnCunstructMode </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#cunstructRigSpacesTARGET">cunstructRigSpaces </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#collectBuildModulesTARGET">collectBuildModules </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#createPickerLayoutBaseTARGET">createPickerLayoutBase </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#createRootGuideTARGET">createRootGuide </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#createPickerTitleGrpTARGET">createPickerTitleGrp </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#createPickerGuideGrpTARGET">createPickerGuideGrp </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#createNewRigTopTARGET">createNewRigTop </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#createPickerProjectionCamTARGET">createPickerProjectionCam </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#createSubGroupForRigTopTARGET">createSubGroupForRigTop </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#createPickerCamTARGET">createPickerCam </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#createPuppetRootCtrlTARGET">createPuppetRootCtrl </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#createVisEnumAndConnectTARGET">createVisEnumAndConnect </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getGlobalConstructionStateTARGET">getGlobalConstructionState </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadSettingsWindowTARGET">loadSettingsWindow </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#restorePuppetBaseDefaultsTARGET">restorePuppetBaseDefaults </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setConstructionModeTARGET">setConstructionMode </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#deconstructRigTARGET">deconstructRig </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#constructRigTARGET">constructRig </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#storePuppetBaseDefaultsTARGET">storePuppetBaseDefaults </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#destroyPuppetRootCtrlTARGET">destroyPuppetRootCtrl </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#createSubGrpsForRigTopTARGET">createSubGrpsForRigTop </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#executeCustomScriptsTARGET">executeCustomScripts </b></a> <font size = 2pt><i>[method]</i></font></li>
</ul>
</td>
</tr>
</table></font>
####MnsRig  methods
<hr width = 50%>
<h5 id = "failedConstructionCommandTARGET"></h5><font color = 464646 size = 3><b>failedConstructionCommand <font size = 2pt> [<a href="#MnsRig TARGET">MnsRig </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>A global method to display and return a message dialog whenever a build fails.</i><br>
<i>This method displays 3 options and returns a paraller state:</i><br>
<i>- 0: 'Continue'</i><br>
<i>- 1: 'Abort'</i><br>
<i>- 2: 'Revert-Construction'</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>failedConstructionCommand(self, fileName = "")</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>int (state/button clicked)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>fileName</b>(<i>str</i>) ; [default: ""]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setVisChannelsBasedOnCunstructModeTARGET"></h5><font color = 464646 size = 3><b>setVisChannelsBasedOnCunstructMode <font size = 2pt> [<a href="#MnsRig TARGET">MnsRig </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>A simple method to set the vis mode of the current rig based on it's construction state.</i><br>
<i>The construction mode is read from the rigTop attribues.</i><br>
<i>Construction modes:</i><br>
<i>0: Guides - guideGrpVis = True, puppetGrpVis = False</i><br>
<i>1: Intermediate (Partially built rig) - guideGrpVis = True, puppetGrpVis = True</i><br>
<i>2: Puppet - guideGrpVis = False, puppetGrpVis = True</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setVisChannelsBasedOnCunstructMode(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "cunstructRigSpacesTARGET"></h5><font color = 464646 size = 3><b>cunstructRigSpaces <font size = 2pt> [<a href="#MnsRig TARGET">MnsRig </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Attempt to construct spaces for all 'modules' within the rig.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>cunstructRigSpaces(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "collectBuildModulesTARGET"></h5><font color = 464646 size = 3><b>collectBuildModules <font size = 2pt> [<a href="#MnsRig TARGET">MnsRig </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Collect all build modules guide hierarchy into the 'modules' attribure of this class.</i><br>
<i>This method will run through the rig, and attempt to collect it's guide heirarchy, validating the modules while collecting.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>collectBuildModules(self, **kwargs)</td></tr>
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
<h5 id = "createPickerLayoutBaseTARGET"></h5><font color = 464646 size = 3><b>createPickerLayoutBase <font size = 2pt> [<a href="#MnsRig TARGET">MnsRig </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Create Picker Layout Base control, and construct all of it's predefined attributes.</i><br>
<i>The predefined attributes for the PLG base is the following:</i><br>
<i>- width - Will define the width of the rig's picker window</i><br>
<i>- height- Will define the height of the rig's picker window</i><br>
<i>- titleVis - vis attr for the title-group</i><br>
<i>- titleSize - a global scalar for all mnsAnnotate PLG titles.</i><br>
<i>This group also contains a few vis control channels to allow easier edit for the PLGs:</i><br>
<i>- bodyPrimaries</i><br>
<i>- bodySecondaries</i><br>
<i>- bodyTertiaries</i><br>
<i>- facialPrimaries</i><br>
<i>- facialSecondaries</i><br>
<i>- facialTertiaries</i><br>
<i>These sub-vis channels will be controled by a global toggle attribute:</i><br>
<i>- pickerMode</i><br>
<i>This will dictate the picker's scene vis mode, the toggle is between 'body' and 'facial' modes.</i><br>
<i>As the picker inhabits to tabs - body and facial, these attributes will allow better manipulation of PLG, grouping them according to the actual picker window tab grouping.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createPickerLayoutBase(self, rigTop, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsNameStd (baseLayoutGuide)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>rigTop</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "createRootGuideTARGET"></h5><font color = 464646 size = 3><b>createRootGuide <font size = 2pt> [<a href="#MnsRig TARGET">MnsRig </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Create the "world control guide", or "rigRootGuide".</i><br>
<i>This rootGuide will be locked completely and will define the predefined "world" control for the puppet.</i><br>
<i>This entity is mandatory.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createRootGuide(self, rigTopNameStd, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsNameStd (Root Guide)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>rigTopNameStd</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "createPickerTitleGrpTARGET"></h5><font color = 464646 size = 3><b>createPickerTitleGrp <font size = 2pt> [<a href="#MnsRig TARGET">MnsRig </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Create the Picker Layout 'titles' sub-component.</i><br>
<i>This group contains the mnsAnnotate locators to toggle PLG view between it's shape and it's title.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createPickerTitleGrp(self, rigTop, pickerLayoutBase,**kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsNameStd (titleGrp)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>rigTop</b></li>
<li><b>pickerLayoutBase</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "createPickerGuideGrpTARGET"></h5><font color = 464646 size = 3><b>createPickerGuideGrp <font size = 2pt> [<a href="#MnsRig TARGET">MnsRig </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Create the main Picker-Layout-Guides sub-component.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createPickerGuideGrp(self, rigTop, pickerLayoutBase, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsNameStd (guidesGrp)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>rigTop</b></li>
<li><b>pickerLayoutBase</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "createNewRigTopTARGET"></h5><font color = 464646 size = 3><b>createNewRigTop <font size = 2pt> [<a href="#MnsRig TARGET">MnsRig </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Create the main rig group, with all of its sub-Components within.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createNewRigTop(self, **kwargs)</td></tr>
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
<h5 id = "createPickerProjectionCamTARGET"></h5><font color = 464646 size = 3><b>createPickerProjectionCam <font size = 2pt> [<a href="#MnsRig TARGET">MnsRig </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Create the predefined "PLG Projection" camera within the rig.</i><br>
<i>A dedicated mns node is used here - 'mnsCamreGateRatio':</i><br>
<i>This dedicated node was written in order to control the camera shape 'gateRatio' attribute.</i><br>
<i>Because this attribute isn't connectable (internal callback within the camera shape), </i><br>
<i>mnsCameraGateRatio inserts a custom maya-callback into itself, in-order to refresh the camera-gate in a "live" fashion,</i><br>
<i>This will allow the user to edit the width and height of the projection camera, seeing a live feed of it's gate in the view.</i><br>
<i>As the projection is based on the camera gate, it is very important for the user to see the actual gate used, while projecting PLG's.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createPickerProjectionCam(self, rigTop, pickerLayoutBase)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsNameStd (Picker Projection Camera)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>rigTop</b></li>
<li><b>pickerLayoutBase</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "createSubGroupForRigTopTARGET"></h5><font color = 464646 size = 3><b>createSubGroupForRigTop <font size = 2pt> [<a href="#MnsRig TARGET">MnsRig </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Create the predefined "guideGrp" or "freeJointsGrp" within the rig.</i><br>
<i>Guides Group - Contains the module main guides.</i><br>
<i>Free Joints Group - Contains the interpLocs intermediate matricies for the interJnts in the main jointStructure</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createSubGroupForRigTop(self, rigTopNameStd, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsNameStd (guideGrp/freeJointsGrp)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>rigTopNameStd</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
<td><ul>
<li><b>subGrpType</b>(<i>str</i>)</li>
<li><b>default</b>(<i>int</i>) ; [default: 1]</li>
</ul></td>
</tr>
</table></font>
<h5 id = "createPickerCamTARGET"></h5><font color = 464646 size = 3><b>createPickerCam <font size = 2pt> [<a href="#MnsRig TARGET">MnsRig </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Create the predefined "picker Layout View" camera within the rig.</i><br>
<i>This camera will be used as the view camera when an "edit picker layout" trigger was initiated from BlockUI.</i><br>
<i>The camera is orthographic, and will be used in a seperate display (Maya-Panel).</i><br>
<i>This to allow easy view of the picker layout, and easy manipulation of PLG shapes and controls.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createPickerCam(self, rigTop, pickerLayoutBase, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsNameStd (Picker Layout Camera)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>rigTop</b></li>
<li><b>pickerLayoutBase</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "createPuppetRootCtrlTARGET"></h5><font color = 464646 size = 3><b>createPuppetRootCtrl <font size = 2pt> [<a href="#MnsRig TARGET">MnsRig </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Create the rig's predefined "puppetRoot" or "worldControl".</i><br>
<i>This depends on the rootGuide of course, and transfer the rigs "Root-Joint" Authority from the rootGuide, to the new puppetRoot control.</i><br>
<i>This method will return the new control, as well as store it in the 'puppetTopCtrl' attribute of this class.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createPuppetRootCtrl(self, rigTop, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsNameStd (Root Guide)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>rigTop</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "createVisEnumAndConnectTARGET"></h5><font color = 464646 size = 3><b>createVisEnumAndConnect <font size = 2pt> [<a href="#MnsRig TARGET">MnsRig </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>For any given slave MnsNameStd group passed in, create a generic vis channel and connect it.</i><br>
<i>The Enums of the generic vis channels are the following:</i><br>
<i>- hidden</i><br>
<i>- normal</i><br>
<i>- template</i><br>
<i>- reference</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createVisEnumAndConnect(self, masterStd, slaveStd, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>PyAttribute (created attribute)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>masterStd</b></li>
<li><b>slaveStd</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
<td><ul>
<li><b>default</b>(<i>int</i>) ; [default: 1]</li>
</ul></td>
</tr>
</table></font>
<h5 id = "getGlobalConstructionStateTARGET"></h5><font color = 464646 size = 3><b>getGlobalConstructionState <font size = 2pt> [<a href="#MnsRig TARGET">MnsRig </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Gey the current rig construction state from rigTop attributes.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getGlobalConstructionState(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>int (mode)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "loadSettingsWindowTARGET"></h5><font color = 464646 size = 3><b>loadSettingsWindow <font size = 2pt> [<a href="#MnsRig TARGET">MnsRig </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Load the dynamic "setting window" for the current rig.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadSettingsWindow(self, **kwargs)</td></tr>
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
<h5 id = "restorePuppetBaseDefaultsTARGET"></h5><font color = 464646 size = 3><b>restorePuppetBaseDefaults <font size = 2pt> [<a href="#MnsRig TARGET">MnsRig </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>On reconstruction, attempt to restore the 'defaults' attribute for the puppet root, if there are any.</i><br>
<i>related method: storePuppetBaseDefaults</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>restorePuppetBaseDefaults(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setConstructionModeTARGET"></h5><font color = 464646 size = 3><b>setConstructionMode <font size = 2pt> [<a href="#MnsRig TARGET">MnsRig </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Set the construction state attribute of the current rig.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setConstructionMode(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "deconstructRigTARGET"></h5><font color = 464646 size = 3><b>deconstructRig <font size = 2pt> [<a href="#MnsRig TARGET">MnsRig </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>This is the main deconstruction method for the rig.</i><br>
<i>Flow:</i><br>
<i>- Log, and set Timer</i><br>
<i>- Collect all relevant data from the rig</i><br>
<i>- Collect modules to build</i><br>
<i>- Loop through the 'modules' dict attribute of this class:</i><br>
<i>- Initiate the 'Deconstruct' method for every buildModule class within the collection.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>deconstructRig(self, **kwargs)</td></tr>
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
<h5 id = "constructRigTARGET"></h5><font color = 464646 size = 3><b>constructRig <font size = 2pt> [<a href="#MnsRig TARGET">MnsRig </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>This method is the main 'Construction' call for a mnsRig.</i><br>
<i>Flow:</i><br>
<i>- Log, and set Timer</i><br>
<i>- Collect all relevant data from the rig</i><br>
<i>- Collect modules to build</i><br>
<i>- Loop through the 'modules' dict attribute of this class:</i><br>
<i>- Initiate the 'Construct' method for every buildModule class within the collection.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>constructRig(self, **kwargs)</td></tr>
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
<h5 id = "storePuppetBaseDefaultsTARGET"></h5><font color = 464646 size = 3><b>storePuppetBaseDefaults <font size = 2pt> [<a href="#MnsRig TARGET">MnsRig </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>This method is used to store the current 'Defaults' set for the puppet-root control on deconstruction.</i><br>
<i>As deconstruction deletes all the controls, including the puppet-root, if any custom-defaults were set,</i><br>
<i>its essential to store them, in order to re-create them on re-construction.</i><br>
<i>This is a specific case for the root-control, as it isn't a 'build-module' hence, the generic defaults store for the build modules doesn't apply.</i><br>
<i>related method: restorePuppetBaseDefaults</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>storePuppetBaseDefaults(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "destroyPuppetRootCtrlTARGET"></h5><font color = 464646 size = 3><b>destroyPuppetRootCtrl <font size = 2pt> [<a href="#MnsRig TARGET">MnsRig </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>This method will destroy the rig's puppetRoot control, and transfer the rig's root-joint authority back to it's rootGuide.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>destroyPuppetRootCtrl(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "createSubGrpsForRigTopTARGET"></h5><font color = 464646 size = 3><b>createSubGrpsForRigTop <font size = 2pt> [<a href="#MnsRig TARGET">MnsRig </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>This wrapper creates all the sub-group components for a given main rigTop group.</i><br>
<i>The sub-groups defenition is the following:</i><br>
<i>- guideGrp - Guides group component</i><br>
<i>- puppetGrp - The Puppet group.</i><br>
<i>- jointStructGrp - Joint Structure group</i><br>
<i>- pickerLayoutGrp - Picker Layout guiides group.</i><br>
<i>- controlShapesGrp - Stored custom shapes group.</i><br>
<i>- freeJointsGrp - "Free joints" group, containing interLocs as intermediate objects to the interJoints in the main joint structure.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createSubGrpsForRigTop(self, rigTop = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>rigTop</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "executeCustomScriptsTARGET"></h5><font color = 464646 size = 3><b>executeCustomScripts <font size = 2pt> [<a href="#MnsRig TARGET">MnsRig </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>for the given 'customScripts' attribute: compile the run files, and execute (if set).</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>executeCustomScripts(self, attrName = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td> bool (Execution success)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>attrName</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
