<body>
#moduleVisUI
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur === <br>
mnsModuleVisUI <br>
A simple UI to control puppet's module animation controls visibility. <br>
 <br>
</font>
</i>
<hr width = 100%>
##Classes
<hr width = 100%>
<h5 id = "MnsModuleVisUI TARGET"></h5>
###MnsModuleVisUI [Class]
<font color = #5f5f5f size = 3pt>
<i>
Main UI Class <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>MnsModuleVisUI(<b>parent</b>(<i>str</i>) ; [default: mnsUIUtils.get_maya_window()])</td></tr>
<tr><td><b><font color = #4caf50>Inherits from:  </font></b></td><td>form_class, base_class</td></tr>
<tr><td><b><font color = #4caf50>Class Members:  </font></b></td>
<td><ul>
<ul>
<li>iconDir</li>
<li>bodyLOHolder</li>
<li>facialLOHolder</li>
<li>layoutHolders</li>
<li>puppetRoot</li>
<li>rigTop</li>
<li>rigTops</li>
<li>moduleAttrs</li>
<li>btnDict</li>
<li>allBtnDict</li>
<li>layoutByAttrs</li>
</ul>
</td></tr>
<tr><td><b><font color = #4caf50>Methods:  </font></b></td><td><ul>
<li><b><a href="#clearLocalVarsTARGET">clearLocalVars </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#destroyUITARGET">destroyUI </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#drawUITARGET">drawUI </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#filterRowsTARGET">filterRows </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getAttrsFromPuppetRootTARGET">getAttrsFromPuppetRoot </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getUITabStateTARGET">getUITabState </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#initializeRigTopTabTARGET">initializeRigTopTab </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#initializeUITARGET">initializeUI </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#refreshTARGET">refresh </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setGlobAllTriggerTARGET">setGlobAllTrigger </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setGlobPrimariesTriggerTARGET">setGlobPrimariesTrigger </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setGlobSecondariesTriggerTARGET">setGlobSecondariesTrigger </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setGlobTertiariesTriggerTARGET">setGlobTertiariesTrigger </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setRowsVisBasedOnStateTARGET">setRowsVisBasedOnState </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#detarmineAttrTypeTARGET">detarmineAttrType </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#drawRigTopBoolRowTARGET">drawRigTopBoolRow </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#drawRigTopEnumRowTARGET">drawRigTopEnumRow </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#toggleAllStateForRowTARGET">toggleAllStateForRow </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#changeModuleVisStateTARGET">changeModuleVisState </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#drawModuleRowTARGET">drawModuleRow </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setRowVisBasedOnStateTARGET">setRowVisBasedOnState </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setRigTopBoolAttrStateTARGET">setRigTopBoolAttrState </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setRigTopBtnStateTARGET">setRigTopBtnState </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#connectSignalsTARGET">connectSignals </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadWindowTARGET">loadWindow </b></a> <font size = 2pt><i>[method]</i></font></li>
</ul>
</td>
</tr>
</table></font>
####MnsModuleVisUI  methods
<hr width = 50%>
<h5 id = "clearLocalVarsTARGET"></h5><font color = 464646 size = 3><b>clearLocalVars <font size = 2pt> [<a href="#MnsModuleVisUI TARGET">MnsModuleVisUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>clearLocalVars(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "destroyUITARGET"></h5><font color = 464646 size = 3><b>destroyUI <font size = 2pt> [<a href="#MnsModuleVisUI TARGET">MnsModuleVisUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>destroyUI(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "drawUITARGET"></h5><font color = 464646 size = 3><b>drawUI <font size = 2pt> [<a href="#MnsModuleVisUI TARGET">MnsModuleVisUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>drawUI(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "filterRowsTARGET"></h5><font color = 464646 size = 3><b>filterRows <font size = 2pt> [<a href="#MnsModuleVisUI TARGET">MnsModuleVisUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>filterRows(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getAttrsFromPuppetRootTARGET"></h5><font color = 464646 size = 3><b>getAttrsFromPuppetRoot <font size = 2pt> [<a href="#MnsModuleVisUI TARGET">MnsModuleVisUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getAttrsFromPuppetRoot(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getUITabStateTARGET"></h5><font color = 464646 size = 3><b>getUITabState <font size = 2pt> [<a href="#MnsModuleVisUI TARGET">MnsModuleVisUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getUITabState(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "initializeRigTopTabTARGET"></h5><font color = 464646 size = 3><b>initializeRigTopTab <font size = 2pt> [<a href="#MnsModuleVisUI TARGET">MnsModuleVisUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>initializeRigTopTab(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "initializeUITARGET"></h5><font color = 464646 size = 3><b>initializeUI <font size = 2pt> [<a href="#MnsModuleVisUI TARGET">MnsModuleVisUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>initializeUI(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "refreshTARGET"></h5><font color = 464646 size = 3><b>refresh <font size = 2pt> [<a href="#MnsModuleVisUI TARGET">MnsModuleVisUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>refresh(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setGlobAllTriggerTARGET"></h5><font color = 464646 size = 3><b>setGlobAllTrigger <font size = 2pt> [<a href="#MnsModuleVisUI TARGET">MnsModuleVisUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setGlobAllTrigger(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setGlobPrimariesTriggerTARGET"></h5><font color = 464646 size = 3><b>setGlobPrimariesTrigger <font size = 2pt> [<a href="#MnsModuleVisUI TARGET">MnsModuleVisUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setGlobPrimariesTrigger(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setGlobSecondariesTriggerTARGET"></h5><font color = 464646 size = 3><b>setGlobSecondariesTrigger <font size = 2pt> [<a href="#MnsModuleVisUI TARGET">MnsModuleVisUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setGlobSecondariesTrigger(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setGlobTertiariesTriggerTARGET"></h5><font color = 464646 size = 3><b>setGlobTertiariesTrigger <font size = 2pt> [<a href="#MnsModuleVisUI TARGET">MnsModuleVisUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setGlobTertiariesTrigger(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setRowsVisBasedOnStateTARGET"></h5><font color = 464646 size = 3><b>setRowsVisBasedOnState <font size = 2pt> [<a href="#MnsModuleVisUI TARGET">MnsModuleVisUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setRowsVisBasedOnState(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "detarmineAttrTypeTARGET"></h5><font color = 464646 size = 3><b>detarmineAttrType <font size = 2pt> [<a href="#MnsModuleVisUI TARGET">MnsModuleVisUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>detarmineAttrType(self, attr)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>attr</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "drawRigTopBoolRowTARGET"></h5><font color = 464646 size = 3><b>drawRigTopBoolRow <font size = 2pt> [<a href="#MnsModuleVisUI TARGET">MnsModuleVisUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>drawRigTopBoolRow(self, attr)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>attr</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "drawRigTopEnumRowTARGET"></h5><font color = 464646 size = 3><b>drawRigTopEnumRow <font size = 2pt> [<a href="#MnsModuleVisUI TARGET">MnsModuleVisUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>drawRigTopEnumRow(self, attr)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>attr</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "toggleAllStateForRowTARGET"></h5><font color = 464646 size = 3><b>toggleAllStateForRow <font size = 2pt> [<a href="#MnsModuleVisUI TARGET">MnsModuleVisUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>toggleAllStateForRow(self, attr)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>attr</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "changeModuleVisStateTARGET"></h5><font color = 464646 size = 3><b>changeModuleVisState <font size = 2pt> [<a href="#MnsModuleVisUI TARGET">MnsModuleVisUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>changeModuleVisState(self, attr, dummy)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>attr</b></li>
<li><b>dummy</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "drawModuleRowTARGET"></h5><font color = 464646 size = 3><b>drawModuleRow <font size = 2pt> [<a href="#MnsModuleVisUI TARGET">MnsModuleVisUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>drawModuleRow(self, attr = None, layoutParent = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>attr</b>(<i>str</i>) ; [default: None]</li>
<li><b>layoutParent</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setRowVisBasedOnStateTARGET"></h5><font color = 464646 size = 3><b>setRowVisBasedOnState <font size = 2pt> [<a href="#MnsModuleVisUI TARGET">MnsModuleVisUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setRowVisBasedOnState(self, attrKey)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>attrKey</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setRigTopBoolAttrStateTARGET"></h5><font color = 464646 size = 3><b>setRigTopBoolAttrState <font size = 2pt> [<a href="#MnsModuleVisUI TARGET">MnsModuleVisUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setRigTopBoolAttrState(self, btn, attr, setCurrentState = False)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>btn</b></li>
<li><b>attr</b></li>
<li><b>setCurrentState</b>(<i>bool</i>) ; [default: False]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setRigTopBtnStateTARGET"></h5><font color = 464646 size = 3><b>setRigTopBtnState <font size = 2pt> [<a href="#MnsModuleVisUI TARGET">MnsModuleVisUI </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setRigTopBtnState(self, visBtn, typeBtn, attr, btnType = 0, setCurrentState = False)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>visBtn</b></li>
<li><b>typeBtn</b></li>
<li><b>attr</b></li>
<li><b>btnType</b>(<i>int</i>) ; [default: 0]</li>
<li><b>setCurrentState</b>(<i>bool</i>) ; [default: False]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "connectSignalsTARGET"></h5><font color = 464646 size = 3><b>connectSignals <font size = 2pt> [<a href="#MnsModuleVisUI TARGET">MnsModuleVisUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Connect all UI signals</i><br>
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
<h5 id = "loadWindowTARGET"></h5><font color = 464646 size = 3><b>loadWindow <font size = 2pt> [<a href="#MnsModuleVisUI TARGET">MnsModuleVisUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Main UI load</i><br>
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
