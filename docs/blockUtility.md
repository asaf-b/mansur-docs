<body>
#blockUtility
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
###createModuleTopNode
<font color = #5f5f5f size = 3pt>
<i>
This method is used to create the genric 'module top group' on module construction. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createModuleTopNode(MnsBuildModuleA = None, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsNameStd (Module Top Group)</td></tr>
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
###createPickerLayoutGuide
<font color = #5f5f5f size = 3pt>
<i>
The main creation method for PLG creation. <br>
   This method will create a new 'Pikcer Layout Guide' based on the passed in parameters. <br>
   1. get picker layout base. <br>
   2. collect projection position if requested. <br>
   3. create and set all attributes <br>
   4. create the related title (mnsAnnotate node) <br>
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
###ctrlPickerGuideToggle
<font color = #5f5f5f size = 3pt>
<i>
Atempt to toggle between a selection "control" and "PLG" if possible. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>ctrlPickerGuideToggle()</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
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
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>extractControlShapes(ctrls = [], rigTop = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>list (controls)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>ctrls</b>(<i>list</i>) ; [default: []]</li>
<li><b>rigTop</b>(<i>str</i>) ; [default: None]</li>
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
###getCtrlCol
<font color = #5f5f5f size = 3pt>
<i>
Get the passed in node's color based on it's type, heirarchy and attributes. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getCtrlCol(ctrl, rigTop)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>tuple[3] (color)</td></tr>
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
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getModuleInterpJoints(guideRoot)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>list (matching interJoints)</td></tr>
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
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsNameNameStd (rigTop)</td></tr>
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
<font color = #5f5f5f size = 3pt>
<i>
Attempt to get a rigTop node from current selection <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getRigTopForSel()</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsNameStd (rigTop)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
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
###removeModuleVisAttrFromPuppetTop
<font color = #5f5f5f size = 3pt>
<i>
This method will remove the corresponding "module vis" channel from the given puppet base control. <br>
   This method is used when a 'partial deconstruction' is initiated, keeping only relevant vis channels in place, removing the 'deconstructed' modules vis channels. <br>
   a <br>
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
<li><b>delete</b>(<i>bool</i>)</li>
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
