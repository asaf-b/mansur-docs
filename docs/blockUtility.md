<body>
#blockUtility
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur === <br>
BLOCK Core Utility Library. <br>
This library contains all utility methods used primarily by BLOCK. <br>
The objective of this library is mainting most Block-Core abilities external and independent. <br>
 <br>
</font>
</i>
<hr width = 100%>
##Classes
<hr width = 100%>
<h5 id = "MnsRigInfo TARGET"></h5>
###MnsRigInfo [Class]
<font color = #5f5f5f size = 3pt>
<i>
Mansur - About dialog <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>MnsRigInfo(<b>parent</b>(<i>str</i>) ; [default: mnsUIUtils.get_maya_window()],<b>rigInfoData</b>(<i>dict</i>) ; [default: {}])</td></tr>
<tr><td><b><font color = #4caf50>Inherits from:  </font></b></td><td>QtWidgets.QDialog</td></tr>
<tr><td><b><font color = #4caf50>Class Members:  </font></b></td>
<td><ul>
<ul>
<li>iconsDir</li>
<li>close_btn</li>
</ul>
</td></tr>
</tr>
</table></font>
<hr width = 100%>
##Defenitions
<hr width = 100%>
###addDefaultAttrsToPlg
<font color = #5f5f5f size = 3pt>
<i>
For a newly created plg, create all of it's default predefined attributes. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>addDefaultAttrsToPlg(plg, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>plg</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###alignPLGuides
<font color = #5f5f5f size = 3pt>
<i>
This is the main 'align' trigger to all 'align tools' in BLOCK. <br>
   This method will calidate and collect the current scene slection, then align the collected PLG's based on the mode passed in. <br>
</i>
<br>
</font>
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
###attemptModulePathFixForRootGuide
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>attemptModulePathFixForRootGuide(guideRoot, existingBtns)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>guideRoot</b></li>
<li><b>existingBtns</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###attemptModulePathFixFroRigTop
<font color = #5f5f5f size = 3pt>
<i>
Run through all existing rig component (in rigTop) and validate the module directories against all existing module directories. <br>
If a module path was found invalid, attempt to re-find it in the existing modules. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>attemptModulePathFixFroRigTop(rigTop, existingBtns, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rigTop</b></li>
<li><b>existingBtns</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###bakeSlaveControls
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>bakeSlaveControls(rigTop = None)</td></tr>
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
###buildShapes
<font color = #5f5f5f size = 3pt>
<i>
This method will be called from a rig construction. <br>
   This method will look for any contol shapes stored within the given rig (rigTop), and replace the default shapes with any corresponding control shape. <br>
   Shape replacement method will be done according to the 'mode' flag (relative/absulote). <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>buildShapes(ctrls = [], rigTop = None, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>ctrls</b>(<i>list</i>) ; [default: []]</li>
<li><b>rigTop</b>(<i>str</i>) ; [default: None]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
<td><ul>
<li><b>mode</b>(<i>int</i>)</li>
</ul></td>
</tr>
</table></font>
<hr width = 100%>
###characterizeHumanIK
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>characterizeHumanIK(charDefData = {}, mode = 0, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>charDefData</b>(<i>dict</i>) ; [default: {}]</li>
<li><b>mode</b>(<i>int</i>) ; [default: 0]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###collectCtrlRelatives
<font color = #5f5f5f size = 3pt>
<i>
Collect ctrls based on given state: <br>
0: All <br>
1: Modules <br>
2: Selected <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>collectCtrlRelatives(mode = 0, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>list (controls)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>mode</b>(<i>int</i>) ; [default: 0]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###collectCtrls
<font color = #5f5f5f size = 3pt>
<i>
Collect ALL related controls for th given rigTop. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>collectCtrls(rigTop = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>list (controls)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rigTop</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###collectGuides
<font color = #5f5f5f size = 3pt>
<i>
Based on the oprional arguments passed in, collect all matching related guides to the input root list. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>collectGuides(roots = pm.ls(sl = 1), **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>dict (Related guides), list (sparseGuides, guide without any relations)</td></tr>
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
###collectModuleControls
<font color = #5f5f5f size = 3pt>
<i>
Collect all related controls for the given module. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>collectModuleControls(moduleTop, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>list (controls)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>moduleTop</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###collectModuleRootsBasedOnMode
<font color = #5f5f5f size = 3pt>
<i>
0: All <br>
1: Branch <br>
2: Module <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>collectModuleRootsBasedOnMode(mode = 0)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td> list (root guides (modules) to build)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>mode</b>(<i>int</i>) ; [default: 0]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###collectPLGuidesToAlign
<font color = #5f5f5f size = 3pt>
<i>
This is the main collect wrapper for all 'align plg' tools in BLOCK. <br>
   This methods will validate and collect all PLG to align from the current scene selection <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>collectPLGuidesToAlign(mode = 0)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>dict (PLGs to align)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>mode</b>(<i>int</i>) ; [default: 0]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###collectPartialModules
<font color = #5f5f5f size = 3pt>
<i>
This method will collect module root objects based on the input data. <br>
If you need to run MnsRig class internal methods, which can operate on partial modules as well as the entire rig, use this method to collect the partial data to be passed into MnsRig class methods. <br>
In case fromNodes argument is Null, this method will return data based on the current scene selection. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>collectPartialModules(fromNodes = [], mode = 0)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>fromNodes</b>(<i>list</i>) ; [default: []]</li>
<li><b>mode</b>(<i>int</i>) ; [default: 0]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###collectPartialModulesRoots
<font color = #5f5f5f size = 3pt>
<i>
This method will be called in case a partial build was requested. <br>
Using methods within 'blockUtility', this method will collect the requested modules to build based on the UI state. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>collectPartialModulesRoots(mode)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td> list (root guides (modules) to build)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>mode</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###collectPickerDataForRigTop
<font color = #5f5f5f size = 3pt>
<i>
mode 0 = All <br>
mode 1 = Brnach <br>
mode 2 = module <br>
mode 3 = selected <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>collectPickerDataForRigTop(rigTop = None, mode = 0)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td> dict (plgs data)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rigTop</b>(<i>str</i>) ; [default: None]</li>
<li><b>mode</b>(<i>int</i>) ; [default: 0]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###collectPlgsBasedOnMode
<font color = #5f5f5f size = 3pt>
<i>
mode 0 = All <br>
mode 1 = Brnach <br>
mode 2 = module <br>
mode 3 = selected <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>collectPlgsBasedOnMode(rigTop = None, mode = 0, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rigTop</b>(<i>str</i>) ; [default: None]</li>
<li><b>mode</b>(<i>int</i>) ; [default: 0]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###collectSlavesFromNdr
<font color = #5f5f5f size = 3pt>
<i>
Collect all slaves related to the passed in 'mnsNodeRelationship' node. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>collectSlavesFromNdr(ndrNode)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>list (slave nodes)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>ndrNode</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###compileCnsCtrlsAttrString
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>compileCnsCtrlsAttrString(exsitingCnsCtrlsDict = {})</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>exsitingCnsCtrlsDict</b>(<i>dict</i>) ; [default: {}]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###connectIfNotConnected
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>connectIfNotConnected(attrA, attrB)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>attrA</b></li>
<li><b>attrB</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###connectPlgToVisChannel
<font color = #5f5f5f size = 3pt>
<i>
This method handles the vis channel connection of a plg to it's related layoutBase attributes based on it's type. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>connectPlgToVisChannel(plg)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>plg</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###connectSlaveToDeleteMaster
<font color = #5f5f5f size = 3pt>
<i>
Connect the passed in 'slave' node to the passed in 'master' node using 'mnsNodeRelationship'. <br>
This method will be successfull only if the master already has a related 'mnsNodeRelationship' node. <br>
</i>
<br>
</font>
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
###connectTargetSkeleton
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>connectTargetSkeleton(defenitionDict = {}, blockNameSpace = "", targetNameSpace = "")</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>defenitionDict</b>(<i>dict</i>) ; [default: {}]</li>
<li><b>blockNameSpace</b>(<i>str</i>) ; [default: ""]</li>
<li><b>targetNameSpace</b>(<i>str</i>) ; [default: ""]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###constrainObjectsToSurface
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>constrainObjectsToSurface(MnsBuildModule = None, ctrlMasters = [], jointsToAttach = [], surface = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td> list (new ctrls)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>MnsBuildModule</b>(<i>str</i>) ; [default: None]</li>
<li><b>ctrlMasters</b>(<i>list</i>) ; [default: []]</li>
<li><b>jointsToAttach</b>(<i>list</i>) ; [default: []]</li>
<li><b>surface</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###constructRig
<font color = #5f5f5f size = 3pt>
<i>
API style scripted construction method.  <br>
If you wish to construct a rig from an external command instead of Block's UI, use this method. <br>
You can pass in a fromNodes argument to specify the rig you wish to construct. <br>
In case the fromNodes argument isn't valid, the construction will be selection based. <br>
Also, use the mode argument to specify which mode you wish to construct in: <br>
mode 0 = ALL <br>
mode 1 = Branch <br>
mode 2 = Module <br>
fromNodes is a list argument.  <br>
In case any input is passed, this method will attempt to aquire the modules to construct based on the mode selected. <br>
You can pass in any Block-Node names into this method. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>constructRig(fromNodes = [], mode = 0)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>fromNodes</b>(<i>list</i>) ; [default: []]</li>
<li><b>mode</b>(<i>int</i>) ; [default: 0]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###convertInputObjToSpace
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>convertInputObjToSpace(obj = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td> PyNode (Space object if found)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>obj</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###convertModuleAuthorityToSurface
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>convertModuleAuthorityToSurface(MnsBuildModule)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td> list (new ctrls)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>MnsBuildModule</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###copyShape
<font color = #5f5f5f size = 3pt>
<i>
copy shape utility. <br>
This method is operation on selection. <br>
Copy the control shape of the first selected component, to the rest of the selection. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>copyShape(source = None, targets = [], reposition = True, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>source</b>(<i>str</i>) ; [default: None]</li>
<li><b>targets</b>(<i>list</i>) ; [default: []]</li>
<li><b>reposition</b>(<i>bool</i>) ; [default: True]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###createAndConnectModuleVisChannelsToPuppetRootCtrl
<font color = #5f5f5f size = 3pt>
<i>
This method will create and connect the pedefined visibility graph to a given 'Module Top Group'. <br>
The driver attribute will be created within the puppet's 'world control', and the connection graph (using animCurvesUU node) will input into the group's visibility channels. <br>
The channels are split (predefined) as follows: <br>
0. None <br>
1. primaries <br>
2. Secondaries <br>
3. Tertiaries <br>
4. Secondaries Only <br>
5. Tertiaries Only <br>
6. No Primaries <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createAndConnectModuleVisChannelsToPuppetRootCtrl(moduleTopNode = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>moduleTopNode</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###createCnsForCtrls
<font color = #5f5f5f size = 3pt>
<i>
This method is used to create CNS controls/sub-controls for existing puppet controls. <br>
In case you need to add extra offset controls in order to constraint them to other components, you can use this method. <br>
Pass in a list of controls you want to add sub-controls to, and run. <br>
This method is also the one used by the CNS Tool. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createCnsForCtrls(ctrls = [])</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td> bool (success state)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>ctrls</b>(<i>list</i>) ; [default: []]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###createOffsetSkeleton
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createOffsetSkeleton(rigTop = None)</td></tr>
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
###createPickerLayoutGuide
<font color = #5f5f5f size = 3pt>
<i>
The main creation method for PLG creation. <br>
   This method will create a new 'Pikcer Layout Guide' based on the passed in parameters. <br>
   1. get picker layout base. <br>
   2. collect projection position if requested. <br>
   3. create and set all attributes <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createPickerLayoutGuide(ctrl, override, rigTop = None, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsNameStd (plg)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>ctrl</b></li>
<li><b>override</b></li>
<li><b>rigTop</b>(<i>str</i>) ; [default: None]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###createPickerLayoutGuides
<font color = #5f5f5f size = 3pt>
<i>
Warpper method that handles multiple PLGs creation. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createPickerLayoutGuides(ctrlsToProject, rigTop, msgPrompt = True, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>ctrlsToProject</b></li>
<li><b>rigTop</b></li>
<li><b>msgPrompt</b>(<i>bool</i>) ; [default: True]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###createPlgBaseVisChannels
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createPlgBaseVisChannels(baseLayoutGuide = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>baseLayoutGuide</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###createVisibilityBridgeMdl
<font color = #5f5f5f size = 3pt>
<i>
This method will check wether the 'target' has a visibility channel connection. <br>
   In the case the given 'target' has input visibility connection, a 'bridge' multiplyDoubleLinear node will be created. <br>
   The brigde node will accomidate both sources as an input, instead of replacing the original visibility by simple multiplication. <br>
   By creating the 'bridge', both old and new sources will be kept as drivers, setting the visibility to 'False' if ANY of the given sources is 'False'. <br>
   In case there is no connection input to the target's visibility channel, a simple connection will be made using the input source. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createVisibilityBridgeMdl(source = None, target = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>source</b>(<i>str</i>) ; [default: None]</li>
<li><b>target</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###createVolumeJoint
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createVolumeJoint(parentJoint = None, childJoint = None, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td> mnsNameStd (volumeJoint)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>parentJoint</b>(<i>str</i>) ; [default: None]</li>
<li><b>childJoint</b>(<i>str</i>) ; [default: None]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###createVolumeJointForSelection
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createVolumeJointForSelection()</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td> mnsNameStd (volumeJoint)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###ctrlPickerGuideToggle
<font color = #5f5f5f size = 3pt>
<i>
Atempt to toggle between a selection "control" and "PLG" if possible. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>ctrlPickerGuideToggle(**kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###deconstructRig
<font color = #5f5f5f size = 3pt>
<i>
API style scripted deconstruction method.  <br>
If you wish to construct a rig from an external command instead of Bloxk's UI, use this method. <br>
You can pass in a fromNodes argument to specify the rig you wish to construct. <br>
In case the fromNodes argument isn't valid, the deconstruction will be selection based. <br>
Also, use the mode argument to specify which mode you wish to construct in: <br>
mode 0 = ALL <br>
mode 1 = Branch <br>
mode 2 = Module <br>
fromNodes is a list argument.  <br>
In case any input is passed, this method will attempt to aquire the modules to construct based on the mode selected. <br>
You can pass in any Block-Node names into this method. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>deconstructRig(fromNodes = [], mode = 0)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>fromNodes</b>(<i>list</i>) ; [default: []]</li>
<li><b>mode</b>(<i>int</i>) ; [default: 0]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###deleteDefaultsForCtrl
<font color = #5f5f5f size = 3pt>
<i>
Delete all set custom attributes for the given ctrl. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>deleteDefaultsForCtrl(ctrl, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>ctrl</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###deleteFreeJntGrpForModule
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>deleteFreeJntGrpForModule(guideRoot = None, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>guideRoot</b>(<i>str</i>) ; [default: None]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###deleteOffsetSekeleton
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>deleteOffsetSekeleton(rigTop = None)</td></tr>
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
###deletePoseForGuides
<font color = #5f5f5f size = 3pt>
<i>
Block's delete pose wrapper. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>deletePoseForGuides(guides = [], poseSet = "T", **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>guides</b>(<i>list</i>) ; [default: []]</li>
<li><b>poseSet</b>(<i>str</i>) ; [default: "T"]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###deletePuppetName
<font color = #5f5f5f size = 3pt>
<i>
This method will filter and delete the rigTops' puppet curves title. <br>
</i>
<br>
</font>
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
###deleteRigDefaults
<font color = #5f5f5f size = 3pt>
<i>
Load controls predefined and custom defaults: <br>
0: All <br>
1: Modules <br>
2: Selected <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>deleteRigDefaults(mode = 0, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>mode</b>(<i>int</i>) ; [default: 0]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###detrmineSymmetryDelta
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>detrmineSymmetryDelta(sourceA = None, sourceB = None, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>sourceA</b>(<i>str</i>) ; [default: None]</li>
<li><b>sourceB</b>(<i>str</i>) ; [default: None]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###disconnectSlaveFromMaster
<font color = #5f5f5f size = 3pt>
<i>
Disconnect the slave passed in from it's master, if there is one. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>disconnectSlaveFromMaster(slave)</td></tr>
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
###disconnectTargetSkeleton
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>disconnectTargetSkeleton(defenitionDict = {}, blockNameSpace = "", targetNameSpace = "", **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>defenitionDict</b>(<i>dict</i>) ; [default: {}]</li>
<li><b>blockNameSpace</b>(<i>str</i>) ; [default: ""]</li>
<li><b>targetNameSpace</b>(<i>str</i>) ; [default: ""]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###duplicatePlg
<font color = #5f5f5f size = 3pt>
<i>
Block "PLG duplicate" trigger. <br>
   This method will handle PLG validation and duplication. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>duplicatePlg(guide = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>guide</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###duplicatePlgs
<font color = #5f5f5f size = 3pt>
<i>
A simple wrapper mwthod to handle multiple PLG duplication (Based on scene selection). <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>duplicatePlgs()</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###executeActionScript
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>executeActionScript(plgNode)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>plgNode</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###exportCtrlShapes
<font color = #5f5f5f size = 3pt>
<i>
mode = 0 - All <br>
mode = 1 - Branch <br>
mode = 2 - module <br>
Simple export method for control shapes. <br>
The relevant control shapes are collected, duplicated and exported to MA. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>exportCtrlShapes(mode = 0)</td></tr>
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
###exportPickerData
<font color = #5f5f5f size = 3pt>
<i>
mode 0 = All <br>
mode 1 = Brnach <br>
mode 2 = module <br>
mode 3 = selected <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>exportPickerData(rigTop = None, mode = 0)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rigTop</b>(<i>str</i>) ; [default: None]</li>
<li><b>mode</b>(<i>int</i>) ; [default: 0]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###extractControlShapes
<font color = #5f5f5f size = 3pt>
<i>
Trigger method for BLOCK - 'extract control shapes' method. <br>
   This method will extract and store the current state of control shapes within the given rig (rigTop). <br>
   The extracted shapes will be re-constructed once a rig-rebuild is initiated. <br>
   In case of any control shape already exists, it will be replaced by default. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>extractControlShapes(ctrls = [], rigTop = None, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>list (controls)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>ctrls</b>(<i>list</i>) ; [default: []]</li>
<li><b>rigTop</b>(<i>str</i>) ; [default: None]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###extractSkeleton
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>extractSkeleton(rigTop = None, mode = 0, bakeAnim = False, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rigTop</b>(<i>str</i>) ; [default: None]</li>
<li><b>mode</b>(<i>int</i>) ; [default: 0]</li>
<li><b>bakeAnim</b>(<i>bool</i>) ; [default: False]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###extractSkeleton2
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>extractSkeleton2(rigTop = None, mode = 0, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rigTop</b>(<i>str</i>) ; [default: None]</li>
<li><b>mode</b>(<i>int</i>) ; [default: 0]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###filterCreationOnlyFromArgs
<font color = #5f5f5f size = 3pt>
<i>
A simple method to filter out the "creationOnly" flag for an argument. <br>
   This method is called on a dynamicUI creation call if it NOT a "new creation" mode in BLOCK. <br>
   In case any arguments within the list passed in is flagged as "creationOnly", it is removed from the list <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>filterCreationOnlyFromArgs(argsList)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>list (filtered arguments)</td></tr>
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
<font color = #5f5f5f size = 3pt>
<i>
Filter all pre-defined settings to their corresponding gathering methods, and re-collect <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>filterSettings(fileSettings, node)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>list (settings), string (current side place holder)</td></tr>
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
###findNamingIssuesInHierarchy
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>findNamingIssuesInHierarchy()</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###gatherAllControlsCustomDefaults
<font color = #5f5f5f size = 3pt>
<i>
Gather custom defaults for all ctrls within the given rig. <br>
This method is used on rig deconstruction, to store all set default values, in order to restore them on construction. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>gatherAllControlsCustomDefaults(rigTop)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>dict (All rig custom defaults)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rigTop</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###gatherCustomDefaultDictForCtrl
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>gatherCustomDefaultDictForCtrl(ctrl)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>dict (Custom Defaults Dict)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>ctrl</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###gatherMnsRigObject
<font color = #5f5f5f size = 3pt>
<i>
This method will gather an MnsRig class object based on the passed in input, in order to use all of it's methods. <br>
If you need to run any method from MnsRig class, use this method to gather the class object, the run any internal method within. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>gatherMnsRigObject()</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###gatherModuleCustomDefaults
<font color = #5f5f5f size = 3pt>
<i>
Gather custom defaults for all ctrls within the given module. <br>
This method is used on rig deconstruction, to store all set default values, in order to restore them on construction. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>gatherModuleCustomDefaults(moduleTop)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>dict (module custom defaults)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>moduleTop</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getAllCtrlsFromRigTop
<font color = #5f5f5f size = 3pt>
<i>
Get all controls for the given rig top. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getAllCtrlsFromRigTop(rigTop = None)</td></tr>
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
###getAllGuideRootsForRigTop
<font color = #5f5f5f size = 3pt>
<i>
Gather all guide roots for the passed in rigTop node. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getAllGuideRootsForRigTop(rigTop)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>list (rootGuides)</td></tr>
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
<font color = #5f5f5f size = 3pt>
<i>
Collect all 'picker layout guides' from the rig passed in (as rigTop) <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getAllPlgsForRigTop(rigTop)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>list (All PLGs)</td></tr>
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
<font color = #5f5f5f size = 3pt>
<i>
Collect all 'color associated' nodes within the passed in rigTop. <br>
   All returned nodes are considered 'color associated', meaning they are nodes that all of their shapes need to be directly colored. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getAllcolCtrlforRigTop(rigTop)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>list (colorControls)</td></tr>
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
<font color = #5f5f5f size = 3pt>
<i>
Recusrsivly collect all child modules from the given rootGuide's decendents. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getChildModules(rootGuide)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>list (module decendents)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rootGuide</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getCompundChildren
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getCompundChildren(rootGuide = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rootGuide</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getConstructionState
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getConstructionState(rigTop = None)</td></tr>
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
###getCsGrpFromRigTop
<font color = #5f5f5f size = 3pt>
<i>
Attempt to collect the 'Control Shapes Group' from the passed in rigTop. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getCsGrpFromRigTop(rigTop = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsNameStd (ctrlShapes group)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rigTop</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getCtrlAuthFromRootGuide
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getCtrlAuthFromRootGuide(rootGuide = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rootGuide</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getCtrlAuthFromRootGuides
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getCtrlAuthFromRootGuides(rGuides = [])</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rGuides</b>(<i>list</i>) ; [default: []]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getCtrlCol
<font color = #5f5f5f size = 3pt>
<i>
Get the passed in node's color based on it's type, heirarchy and attributes. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getCtrlCol(ctrl, rigTop, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>tuple[3] (color)</td></tr>
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
###getCtrlShapesForModueRoot
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getCtrlShapesForModueRoot(guideRoot)</td></tr>
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
###getCtrlsFromModuleRoot
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getCtrlsFromModuleRoot(guideRoot)</td></tr>
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
###getDeleteMasterFromSlave
<font color = #5f5f5f size = 3pt>
<i>
Collect the delete master from a slave's related 'mnsNodeRelationship' node, if there is one. <br>
   This method will collect the master connected to the 'deleteMaster' attribute of the node. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getDeleteMasterFromSlave(slave)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsNameStd (master)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>slave</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getExisingCnsCtrlsForRigTop
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getExisingCnsCtrlsForRigTop(rigTop)</td></tr>
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
###getExistingCpomNodeFromSurface
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getExistingCpomNodeFromSurface(surface)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>surface</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getExistingSpaceConstraintForControl
<font color = #5f5f5f size = 3pt>
<i>
Collect existing 'spaces' constraints for a passed in (built) control, in order to re-build them in turn, after correct filtering and validation (in case of a partial build for example). <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getExistingSpaceConstraintForControl(ctrl = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>list (mnsMatrixConstraint nodes)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>ctrl</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getExistingSpaceConstraintForControls
<font color = #5f5f5f size = 3pt>
<i>
Wrapper mwthod to collect 'spaces' constraints for multiple controls. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getExistingSpaceConstraintForControls(controls = [])</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>dict (constraintSpaces dictionary)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>controls</b>(<i>list</i>) ; [default: []]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getExistingVolumeJointNodeForJoint
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getExistingVolumeJointNodeForJoint(joint = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>joint</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getExistingVolumeJointNodeForVolumeJoint
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getExistingVolumeJointNodeForVolumeJoint(joint = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>joint</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getGlobalScaleAttrFromTransform
<font color = #5f5f5f size = 3pt>
<i>
This method is used to retreive any output decompose matrix node to be used as global scale input connection. <br>
If this method fails to retreive such attribute, it creates one and returns it. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getGlobalScaleAttrFromTransform(transform = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td> Attribute</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>transform</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getGuideParent
<font color = #5f5f5f size = 3pt>
<i>
Collect a ctrl type object's 'Guide Authority', or related guide object. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getGuideParent(objectSel = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td> PyNode</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>objectSel</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getJointStructGrpFromRigTop
<font color = #5f5f5f size = 3pt>
<i>
Attempt to collect the 'Picker Title Group' from the passed in rigTop. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getJointStructGrpFromRigTop(rigTop = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsNameStd (Offset Skeleton Grp)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rigTop</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getKeyboardModifiersState
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getKeyboardModifiersState()</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getLimbModuleControls
<font color = #5f5f5f size = 3pt>
<i>
mode 0: fk controls and attrHost <br>
mode 1: ik controls and attrHost <br>
mode 2: both and attrHost <br>
mode 3: attrHost only <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getLimbModuleControls(limbCtrl, mode = 2)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>limbCtrl</b></li>
<li><b>mode</b>(<i>int</i>) ; [default: 2]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getModuleAnimGrp
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getModuleAnimGrp(obj = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>obj</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getModuleDecendentsWildcard
<font color = #5f5f5f size = 3pt>
<i>
Collect all given module dendents using a 'wild-card' search method. <br>
   This will collect all relatives using a * search within the root decendents, and return all of the passed in node types. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getModuleDecendentsWildcard(guideRoot, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>list (matching decendents)</td></tr>
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
<font color = #5f5f5f size = 3pt>
<i>
This method will attempt to collect a related PyModule from the given guideRoot passed in. <br>
This method will not return the module's methods, only the PyModule as an object. <br>
This method also contains override optional arguments to specify a direct path or module name. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getModuleFromGuide(guideRoot, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>PyModule (object)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>guideRoot</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
<td><ul>
<li><b>methodName</b>(<i>str</i>) ; [default: jointStructure]</li>
<li><b>modPath</b>(<i>str</i>) ; [default: None]</li>
<li><b>modName</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
</table></font>
<hr width = 100%>
###getModuleGuideDecendents
<font color = #5f5f5f size = 3pt>
<i>
Collect all of the root guide module relatives for the passed in moduleRoot (or rootGuide). <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getModuleGuideDecendents(guideRoot)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>list (sorted by ID module decendents)</td></tr>
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
<font color = #5f5f5f size = 3pt>
<i>
Collect all the given moduleRoot's 'interpolationJoints' relatives. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getModuleInterpJoints(guideRoot, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>list (matching interJoints)</td></tr>
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
###getModuleRoot
<font color = #5f5f5f size = 3pt>
<i>
Attempt to collect the root guide relative from the given node. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getModuleRoot(objectA)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>PyNode (rootGuide)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>objectA</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getModuleRootCtrl
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getModuleRootCtrl(obj = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>obj</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getModuleRootForSel
<font color = #5f5f5f size = 3pt>
<i>
Attempt to collect a 'root guide' relative from the current selection <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getModuleRootForSel()</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>PyNode (moduleRoot)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getModuleScale
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getModuleScale(MnsBuildModule)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>MnsBuildModule</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getModuleSettings
<font color = #5f5f5f size = 3pt>
<i>
Get passed in module settings. <br>
First get the default settings and values from the build-module directory, <br>
then compare against the rootGuide attributes, and return the filtered and altered settings. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getModuleSettings(rootGuide, firstAttempt = True, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td> dict,int (optionalArguments, spilt index - for dynUI)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rootGuide</b></li>
<li><b>firstAttempt</b>(<i>bool</i>) ; [default: True]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getModuleTopForCtrl
<font color = #5f5f5f size = 3pt>
<i>
Collect the 'Module Top Group' related to the passed in control. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getModuleTopForCtrl(ctrl = None, nameMatch = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsNameStd (Module Top Group)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>ctrl</b>(<i>str</i>) ; [default: None]</li>
<li><b>nameMatch</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getModuleTopFromRootGuide
<font color = #5f5f5f size = 3pt>
<i>
Attempt to collect 'Module Top Group' from a given root guide. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getModuleTopFromRootGuide(rootGuide = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsNameStd (Module Top Group)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rootGuide</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getNodeRelationshipNodeFromObject
<font color = #5f5f5f size = 3pt>
<i>
Collect the related 'mnsNodeRelationship' node from the given input node. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getNodeRelationshipNodeFromObject(node)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>PyNode</td></tr>
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
<font color = #5f5f5f size = 3pt>
<i>
Collect the offsetGroup related to the passed in control, if it exists. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getOffsetGrpForCtrl(ctrl, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsNameStd (offset group)</td></tr>
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
###getOffsetSkeletonGrpFromRigTop
<font color = #5f5f5f size = 3pt>
<i>
Attempt to collect the 'Picker Title Group' from the passed in rigTop. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getOffsetSkeletonGrpFromRigTop(rigTop = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsNameStd (Offset Skeleton Grp)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rigTop</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getOppositeSideControl
<font color = #5f5f5f size = 3pt>
<i>
Attempt to collect the opposite related mns object if it exists. <br>
Only non 'ceneter components' will be tested of course. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getOppositeSideControl(obj = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsNameStd (Opposite object)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>obj</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getPickerGuidesGrpFromRigTop
<font color = #5f5f5f size = 3pt>
<i>
Attempt to collect the 'Picker Guide Group' from the passed in rigTop. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getPickerGuidesGrpFromRigTop(rigTop = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsNameStd (Picker Guide Group)</td></tr>
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
<font color = #5f5f5f size = 3pt>
<i>
Attempt to collect the 'Picker Layout Base guide' from the passed in rigTop. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getPickerLayoutBaseFromRigTop(rigTop = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsNameStd (Picker Layout Base guide)</td></tr>
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
<font color = #5f5f5f size = 3pt>
<i>
Attempt to collect the 'Picker Layout Camera' from the passed in rigTop. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getPickerLayoutCamFromRigTop(rigTop = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsNameStd (Picker Layout Base guide)</td></tr>
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
<font color = #5f5f5f size = 3pt>
<i>
Attempt to collect the 'Picker Projection Camera' from the passed in rigTop. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getPickerProjectionCamFromRigTop(rigTop = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsNameStd (Picker Projection Camera)</td></tr>
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
<font color = #5f5f5f size = 3pt>
<i>
Attempt to collect the 'Picker Title Group' from the passed in rigTop. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getPickerTitleGrpFromRigTop(rigTop = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsNameStd (Picker Title Group))</td></tr>
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
<font color = #5f5f5f size = 3pt>
<i>
Attempt to collect the 'puppet group' from the passed in rigTop. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getPuppetBaseFromRigTop(rigTop = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsNameStd (puppet base)</td></tr>
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
<font color = #5f5f5f size = 3pt>
<i>
Attempt to collect the 'Puppet World Control' from the passed in rigTop. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getPuppetRootFromRigTop(rigTop = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsNameStd (Puppet world control)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rigTop</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getPyModuleFromGuide
<font color = #5f5f5f size = 3pt>
<i>
Attempt to collect a 'Python Module' (or package) related to the given guide node passed in. <br>
If a related module was found, this method will return it as a PyModule object not as a directory. <br>
This method will also return the module's methods in a dictionary in order to run directly from it. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getPyModuleFromGuide(guide)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>PyModule, dict (module methods as keys and method objects as entries)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>guide</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getRelatedNodeFromObject
<font color = #5f5f5f size = 3pt>
<i>
Collect a related node from the 'messageOut' attribute of the given node's 'mnsNodeRelationship' node. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getRelatedNodeFromObject(node)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>PyNode</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>node</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getRelatedVolJntSourcesForSelection
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getRelatedVolJntSourcesForSelection()</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getRelationMasterFromSlave
<font color = #5f5f5f size = 3pt>
<i>
Collect the delete master from a slave's related 'mnsNodeRelationship' node, if there is one. <br>
   This method will collect the master connected to the 'masterIn' attribute of the node. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getRelationMasterFromSlave(slave)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsNameStd (master)</td></tr>
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
<font color = #5f5f5f size = 3pt>
<i>
Attempt to get a rigTop node from the passed in node to check. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getRigTop(objectA)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsNameStd (rigTop)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>objectA</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getRigTopAssemblies
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getRigTopAssemblies()</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getRigTopForSel
<font color = #5f5f5f size = 3pt>
<i>
Attempt to get a rigTop node from current selection <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getRigTopForSel(**kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsNameStd (rigTop)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getRootGuideFromCtrl
<font color = #5f5f5f size = 3pt>
<i>
Attempt to collect the related 'rootGuide' from the given control passed in. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getRootGuideFromCtrl(obj)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsNameStd (rootGuide)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>obj</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getRootGuideFromRigTop
<font color = #5f5f5f size = 3pt>
<i>
Attempt to collect the rig's root guide from the passed in rigTop node <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getRootGuideFromRigTop(rigTop = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsNameStd (rig root guide)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rigTop</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getRootJointsFromModuleRoot
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getRootJointsFromModuleRoot(guideRoot)</td></tr>
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
###getSettings
<font color = #5f5f5f size = 3pt>
<i>
Get setting for the requested setting path. <br>
   The settings are being filtered and set according to a node passed in. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getSettings(settingsPath, node, blkType)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>list (optionalArgumentsFromFile), string (current side place holder)</td></tr>
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
###getSideModuleBranchRoot
<font color = #5f5f5f size = 3pt>
<i>
For a non "center" component passed in, recursively attempt to collect the 'side-branch' root guide. <br>
In essence look for the highest rootGuide in the selected 'side' heirarchy that has a 'center' component parent- meaning it's the top of the requested branch. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getSideModuleBranchRoot(guide = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsNameStd (branch root)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>guide</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getSimpleRivetsNodeForMesh
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getSimpleRivetsNodeForMesh(mesh = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td> PyNode</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>mesh</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getSymAttrBasedOnSymMapping
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getSymAttrBasedOnSymMapping(attr = None, attrMapping = {})</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>attr</b>(<i>str</i>) ; [default: None]</li>
<li><b>attrMapping</b>(<i>dict</i>) ; [default: {}]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getSymmetricalVolumeJoint
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getSymmetricalVolumeJoint(vJnt = None, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td> mnsNameStd (symmetrical volume-joint)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>vJnt</b>(<i>str</i>) ; [default: None]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getVJntSources
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getVJntSources(vJnt = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>vJnt</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getVJointData
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getVJointData(vJnt)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>vJnt</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###handleInterpLocsStructureReturn
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>handleInterpLocsStructureReturn(rigTop = None, interpLocs = [], guides = [], **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rigTop</b>(<i>str</i>) ; [default: None]</li>
<li><b>interpLocs</b>(<i>list</i>) ; [default: []]</li>
<li><b>guides</b>(<i>list</i>) ; [default: []]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###importCtrlShapes
<font color = #5f5f5f size = 3pt>
<i>
Simple import method for control shapes. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>importCtrlShapes()</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###importGuidePreset
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>importGuidePreset(presetName = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>presetName</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###importPickerData
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>importPickerData(**kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###injectPlgPropertiesFromData
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>injectPlgPropertiesFromData(plg = None, data = {})</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>plg</b>(<i>str</i>) ; [default: None]</li>
<li><b>data</b>(<i>dict</i>) ; [default: {}]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###insertGuides
<font color = #5f5f5f size = 3pt>
<i>
This method is used primarily through Block UI, to insert guides above/below any guide selection. <br>
This will handle all exceptions, as well as re-analyze and re-orgenize each module based on the action performed. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>insertGuides(amount = 0, mode = "above", **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>amount</b>(<i>int</i>) ; [default: 0]</li>
<li><b>mode</b>(<i>str</i>) ; [default: "above"]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###jointRotateToOrientTrigger
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>jointRotateToOrientTrigger(rigTop = None)</td></tr>
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
###limbMatchFkIK
<font color = #5f5f5f size = 3pt>
<i>
mode 0 - Match FK to IK <br>
mode 1 - Match IK to FK <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>limbMatchFkIK(limbCtrl, mode = 0, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>limbCtrl</b></li>
<li><b>mode</b>(<i>int</i>) ; [default: 0]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###loadDefaultsForCtrl
<font color = #5f5f5f size = 3pt>
<i>
Load all default attributes for the given control, taking mnsDefaults (custom) into acount <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadDefaultsForCtrl(ctrl, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>ctrl</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###loadPerspCam
<font color = #5f5f5f size = 3pt>
<i>
Set Maya's main camera panel, to the default 'persp' camera. <br>
</i>
<br>
</font>
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
<font color = #5f5f5f size = 3pt>
<i>
Set the main maya camera view to the 'picker projection camera', based on the scene selection (or the related rigTop to selection). <br>
</i>
<br>
</font>
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
<font color = #5f5f5f size = 3pt>
<i>
Block's load pose wrapper. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadPoseForGuides(guides = [], poseSet = "T", **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>guides</b>(<i>list</i>) ; [default: []]</li>
<li><b>poseSet</b>(<i>str</i>) ; [default: "T"]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###loadResetValuesForOffsetJoint
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadResetValuesForOffsetJoint(offsetJnt = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>offsetJnt</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###loadRigDefaults
<font color = #5f5f5f size = 3pt>
<i>
Load controls predefined and custom defaults: <br>
0: All <br>
1: Modules <br>
2: Selected <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadRigDefaults(mode = 0, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>mode</b>(<i>int</i>) ; [default: 0]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###loadRigInfo
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadRigInfo(puppetRoot = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>puppetRoot</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###locateCnsForCtrl
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>locateCnsForCtrl(ctrl = None, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>ctrl</b>(<i>str</i>) ; [default: None]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###locatePLGBaseVisMdNodes
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>locatePLGBaseVisMdNodes(baseLayoutGuide = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td> MnsNameStd (bodyMdNode), MnsNameStd (facialMDNode)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>baseLayoutGuide</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###matchExtractedSkeletonToBaseSkeleton
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>matchExtractedSkeletonToBaseSkeleton()</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###matchGuidesToTargetSkeleton
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>matchGuidesToTargetSkeleton(defenitionDict = {}, blockNameSpace = "", targetNameSpace = "")</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>defenitionDict</b>(<i>dict</i>) ; [default: {}]</li>
<li><b>blockNameSpace</b>(<i>str</i>) ; [default: ""]</li>
<li><b>targetNameSpace</b>(<i>str</i>) ; [default: ""]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###matchKeyableAttributes
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>matchKeyableAttributes(source = None, target = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>source</b>(<i>str</i>) ; [default: None]</li>
<li><b>target</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###mirrorCtrls
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>mirrorCtrls(ctrls = [], direction = 0, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>ctrls</b>(<i>list</i>) ; [default: []]</li>
<li><b>direction</b>(<i>int</i>) ; [default: 0]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###missingModuleActionTrigger
<font color = #5f5f5f size = 3pt>
<i>
Action trigger for an invalid module path fix attempt <br>
</i>
<br>
</font>
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
###muteLocalTransformations
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>muteLocalTransformations(ctrl = None, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>ctrl</b>(<i>str</i>) ; [default: None]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###namePuppet
<font color = #5f5f5f size = 3pt>
<i>
This method is used to create the rig's curves puppet title and connect it to to it's world control as additional shape nodes. <br>
</i>
<br>
</font>
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
###orientGuides
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>orientGuides(guides = [], **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>guides</b>(<i>list</i>) ; [default: []]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###pickerButtonClickAction
<font color = #5f5f5f size = 3pt>
<i>
The global action trigger for any picker UI button click trigger. <br>
   This method will trigger the "controls selection" and the "action script" for the passed in QPushButton passed in. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>pickerButtonClickAction(btn, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>btn</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###pickerLayoutAdjust
<font color = #5f5f5f size = 3pt>
<i>
Load a new Maya panel, with the 'Picker Layout Camera' related to the scene selction. <br>
   This will also set the panel settings before loading it, based on the rigTop and 'layout base' attributes. <br>
</i>
<br>
</font>
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
<font color = #5f5f5f size = 3pt>
<i>
Toggle between PLG 'control' view, to 'title' view. <br>
</i>
<br>
</font>
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
<font color = #5f5f5f size = 3pt>
<i>
A simple method to check for argument duplicates within an argument dict <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>preCheckNameForUI(arguments, suffix)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>dict (recompiled arguments)</td></tr>
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
###projectPickerLayout
<font color = #5f5f5f size = 3pt>
<i>
A wrapper method that handles plg projection from scene objects based on mode. <br>
mode 0 = selected <br>
mode 1 = module <br>
mode 2 = branch <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>projectPickerLayout(mode = 0, msgPrompt = True)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>mode</b>(<i>int</i>) ; [default: 0]</li>
<li><b>msgPrompt</b>(<i>bool</i>) ; [default: True]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###projectPickerLayoutPos
<font color = #5f5f5f size = 3pt>
<i>
Get the passed in Ctrl PLG position, relative to the rig's 'layoutBase'. <br>
   This method 'projects' the ctrl position based on the rig's 'Projection Camera' into the layout base space, and returns it's processed position. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>projectPickerLayoutPos(ctrl, cam, layoutBase)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>tuple[3] (posX), tuple[3] (posY)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>ctrl</b></li>
<li><b>cam</b></li>
<li><b>layoutBase</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###projectSelectedPickerLayout
<font color = #5f5f5f size = 3pt>
<i>
A wrapper method that handles plg projection from selected scene objects. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>projectSelectedPickerLayout(msgPrompt = True)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>msgPrompt</b>(<i>bool</i>) ; [default: True]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###rebuildJointStructure
<font color = #5f5f5f size = 3pt>
<i>
modes: <br>
0 = All <br>
1 = Branch <br>
2 = Module <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>rebuildJointStructure(mode = 0)</td></tr>
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
###recGetModuleTopForCtrl
<font color = #5f5f5f size = 3pt>
<i>
Recursively attempt to collect the 'Module Top Group' related to the ctrl passed in within it's related parents. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>recGetModuleTopForCtrl(ctrl = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsNameStd (Module Top Group)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>ctrl</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###recGetParentJoint
<font color = #5f5f5f size = 3pt>
<i>
Recursivly attempt to get a parent joint starting with a given root object, scaling up the heirarchy. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>recGetParentJoint(rootObject = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>mnsNameStd</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rootObject</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###recRenameLowerIndex
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>recRenameLowerIndex(root = None, moduleGuides = [], moduleJoints = [])</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>root</b>(<i>str</i>) ; [default: None]</li>
<li><b>moduleGuides</b>(<i>list</i>) ; [default: []]</li>
<li><b>moduleJoints</b>(<i>list</i>) ; [default: []]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###recSearchForGuideRootInParents
<font color = #5f5f5f size = 3pt>
<i>
Recusrsivly look for a 'rootGuide' from the given node's parent relatives. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>recSearchForGuideRootInParents(obj)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td> PyNode (rootGuide)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>obj</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###removeAlienMatchesFromList
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>removeAlienMatchesFromList(guideRoot, currentMatches = [])</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>guideRoot</b></li>
<li><b>currentMatches</b>(<i>list</i>) ; [default: []]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###removeAllAuthority
<font color = #5f5f5f size = 3pt>
<i>
This method is used to delete all 'Authority' from the passsed in slave, if there are any. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>removeAllAuthority(slave = None, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsNameStd (oldAuthority)</td></tr>
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
###removeCnsFromCtrls
<font color = #5f5f5f size = 3pt>
<i>
This method is used to remove existing CNS controls/sub-controls for existing puppet controls. <br>
If you have CNS controls you want to remove, use this method. <br>
Pass in a list of controls you want to remove sub-controls from, and run. <br>
This method is also the one used by the CNS Tool. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>removeCnsFromCtrls(ctrls = [])</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td> bool (success state)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>ctrls</b>(<i>list</i>) ; [default: []]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###removeGuides
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>removeGuides(**kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###removeModuleVisAttrFromPuppetTop
<font color = #5f5f5f size = 3pt>
<i>
This method will remove the corresponding "module vis" channel from the given puppet base control. <br>
   This method is used when a 'partial deconstruction' is initiated, keeping only relevant vis channels in place, removing the 'deconstructed' modules vis channels. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>removeModuleVisAttrFromPuppetTop(moduleTopNode = None, puppetTop = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>moduleTopNode</b>(<i>str</i>) ; [default: None]</li>
<li><b>puppetTop</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###repositionShape
<font color = #5f5f5f size = 3pt>
<i>
Simple method to re-center a control shape to its natural pivot <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>repositionShape(targets = [])</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>targets</b>(<i>list</i>) ; [default: []]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###resetAllControlForRigTop
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>resetAllControlForRigTop(rigTop = None, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rigTop</b>(<i>str</i>) ; [default: None]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###resetControls
<font color = #5f5f5f size = 3pt>
<i>
reset all keyable attributes to default value. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>resetControls(controls=[], **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>controls</b>(<i>list</i>) ; [default: []]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###resetOffsetSkeleton
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>resetOffsetSkeleton(rigTop = None)</td></tr>
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
###saveLoadDagPose
<font color = #5f5f5f size = 3pt>
<i>
mode 0 = Save <br>
mode 1 = Load <br>
mode 2 = Delete <br>
 <br>
poses: Bind, T, A <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>saveLoadDagPose(rootJoint = None, mode = 1, poseName = "Bind")</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rootJoint</b>(<i>str</i>) ; [default: None]</li>
<li><b>mode</b>(<i>int</i>) ; [default: 1]</li>
<li><b>poseName</b>(<i>str</i>) ; [default: "Bind"]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###saveLoadPose
<font color = #5f5f5f size = 3pt>
<i>
This is the main wrapper for all pose 'save & load' triggers of BLOCK. <br>
</i>
<br>
</font>
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
<li><b>mode</b>(<i>int</i>)</li>
<li><b>saveLoad</b>(<i>int</i>)</li>
<li><b>msgPrompt</b>(<i>bool</i>)</li>
<li><b>pose</b>(<i>str</i>) ; [default: T]</li>
</ul></td>
</tr>
</table></font>
<hr width = 100%>
###savePoseForGuides
<font color = #5f5f5f size = 3pt>
<i>
Block's save pose wrapper. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>savePoseForGuides(guides = [], poseSet = "T", msgPrompt = False, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>guides</b>(<i>list</i>) ; [default: []]</li>
<li><b>poseSet</b>(<i>str</i>) ; [default: "T"]</li>
<li><b>msgPrompt</b>(<i>bool</i>) ; [default: False]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###searchForRootGuideInRelatives
<font color = #5f5f5f size = 3pt>
<i>
Search for a 'guide authority' or 'rootGuide' in the given node's decendents <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>searchForRootGuideInRelatives(obj)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>PyNode (rootGuide)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>obj</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###selectAllCtrls
<font color = #5f5f5f size = 3pt>
<i>
Select all controls for the given rig top. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>selectAllCtrls(rigTop = None, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rigTop</b>(<i>str</i>) ; [default: None]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###selectRelatedControls
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>selectRelatedControls(controlsToSelect, mode = "replace")</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>controlsToSelect</b></li>
<li><b>mode</b>(<i>str</i>) ; [default: "replace"]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###selectSlaveControls
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>selectSlaveControls(rigTop = None, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>rigTop</b>(<i>str</i>) ; [default: None]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###setCtrlCol
<font color = #5f5f5f size = 3pt>
<i>
Attempt to collect the passed in node's color (based on its type), and set it if seccessfull. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setCtrlCol(ctrl, rigTop, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsNameStd (ctrl)</td></tr>
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
###setCurrentStateAsDefaultForCtrl
<font color = #5f5f5f size = 3pt>
<i>
Set custom defaults for keyable attributes for the given control, based on it's current state. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setCurrentStateAsDefaultForCtrl(ctrl, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>ctrl</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###setResetValuesForOffsetJoint
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setResetValuesForOffsetJoint(offsetJnt = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>offsetJnt</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###setRigDefaults
<font color = #5f5f5f size = 3pt>
<i>
Set controls custom defaults based on given state: <br>
0: All <br>
1: Modules <br>
2: Branches <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setRigDefaults(mode = 0, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>mode</b>(<i>int</i>) ; [default: 0]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###setgCtrlColorForModule
<font color = #5f5f5f size = 3pt>
<i>
For all relevant decendents of the passed in moduleRoot, get and set it's color. <br>
</i>
<br>
</font>
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
<font color = #5f5f5f size = 3pt>
<i>
Set ALL relevnt controls within a rigTop, to their color based on their type. <br>
</i>
<br>
</font>
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
###symmetrizeCGShape
<font color = #5f5f5f size = 3pt>
<i>
A simple method to symmetrize custom guides nurbs shapes when aplicable <br>
Mode= <br>
0: All <br>
1: Modules <br>
2: Branches <br>
3: selection <br>
Direction= <br>
0: L -> R <br>
1: R -> L <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>symmetrizeCGShape(mode = 0, direction = 0, cGuides = [])</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>mode</b>(<i>int</i>) ; [default: 0]</li>
<li><b>direction</b>(<i>int</i>) ; [default: 0]</li>
<li><b>cGuides</b>(<i>list</i>) ; [default: []]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###symmetrizePlg
<font color = #5f5f5f size = 3pt>
<i>
Block 'plg symmetrize' button trigger. <br>
   This method will handle validation and creation of PLG related symmetrical plg. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>symmetrizePlg(guide = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>guide</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###symmetrizePlgs
<font color = #5f5f5f size = 3pt>
<i>
A simple wrapper method to symmetrize multiple PLG's (based on scene selection). <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>symmetrizePlgs()</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###symmetrizeVJ
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>symmetrizeVJ(vJnt = None, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>vJnt</b>(<i>str</i>) ; [default: None]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###toggleGuideCtrl
<font color = #5f5f5f size = 3pt>
<i>
Atempt to toggle between a selection guide and main joint if possible. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>toggleGuideCtrl(**kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###toggleGuideJoint
<font color = #5f5f5f size = 3pt>
<i>
Atempt to toggle between a selection guide and main joint if possible. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>toggleGuideJoint(**kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###togglePickerCtrlBodyFacial
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>togglePickerCtrlBodyFacial()</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###transferAuthorityToCtrl
<font color = #5f5f5f size = 3pt>
<i>
This is a very important method used in BLOCK cosntruction. <br>
This method will find the current 'guide control' from the given joint slave. and transfer it's authority to a newly created 'control authority'. <br>
This method will be called on every module build and it is the main trigger to flag a module construction. <br>
The 'authority' attribute for every guide or control is used to distiguish the module state, and jnt state. <br>
When transfering an authority to a ctrl, a 'old authority' attr (of sort) is created, in order for the procedural 'deconstruct' to look for and tranfer the jnt authority back to it's orignal guide,  <br>
before deleting the constructed module. <br>
See also parallel: 'transferAuthorityToGuide' Method. <br>
</i>
<br>
</font>
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
###transferAuthorityToGuide
<font color = #5f5f5f size = 3pt>
<i>
This is a very important method used in BLOCK de-construction. <br>
This method will find the current 'control' from the given joint slave. and transfer it's authority to a it's original 'guide' authority. <br>
This method will be called procedurally on any module deconstruction, before deleting the constructed module. <br>
See also parallel: 'transferAuthorityToCtrl' Method. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>transferAuthorityToGuide(ctrl = None, **kwargs)	</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>ctrl</b>(<i>str</i>) ; [default: None]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###transferAuthorityToOffsetSkeleton
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>transferAuthorityToOffsetSkeleton(rigTop = None)</td></tr>
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
###transferAuthorityToPuppet
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>transferAuthorityToPuppet(rigTop = None)</td></tr>
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
###upParentAllPlgTrigger
<font color = #5f5f5f size = 3pt>
<i>
OBSELETE. PLG parenting is no longer in use. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>upParentAllPlgTrigger()</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###updateRigStructure
<font color = #5f5f5f size = 3pt>
<i>
Rig structure update required trigger. <br>
This method will be called in case any 'jntStructMember' attribute was altered, which means the internal joint structure of the module needs to be rebuilt. <br>
This method will locate and filter the existing module related joint structure, destroy it, and re-build it using the updated settings.  <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>updateRigStructure(softMod = False, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>softMod</b>(<i>bool</i>) ; [default: False]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###volumeJointAngleSymmetryMapping
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>volumeJointAngleSymmetryMapping(symmetryDelta = pm.datatypes.Vector(1.0, 1.0, 1.0))</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>symmetryDelta</b>(<i>str</i>) ; [default: pm.datatypes.Vector(1.0]</li>
<li><b>1.0</b></li>
<li><b>1.0)</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
