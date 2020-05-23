<body>
#plgSettings
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur === <br>
mnsPickerSettings UI Class <br>
This is simple UI class built to handle user manipulation to PLG settings easily. <br>
The settings window (at freest state) handles: <br>
- Color <br>
- Side <br>
- Control goruping (body/facial) <br>
- scaleX, scaleY <br>
- Button text <br>
- font size, color <br>
- font bold, italic, underline <br>
- controls select  <br>
- Action script (pre/post) <br>
 <br>
</font>
</i>
<hr width = 100%>
##Classes
<hr width = 100%>
<h5 id = "MnsPLGSettingsUI TARGET"></h5>
###MnsPLGSettingsUI [Class]
<font color = #5f5f5f size = 3pt>
<i>
mnsPickerSettings UI Class. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>MnsPLGSettingsUI(<b>parent</b>(<i>str</i>) ; [default: mnsUIUtils.get_maya_window()])</td></tr>
<tr><td><b><font color = #4caf50>Inherits from:  </font></b></td><td>form_class, base_class</td></tr>
<tr><td><b><font color = #4caf50>Class Members:  </font></b></td>
<td><ul>
<ul>
<li>iconsDir</li>
<li>pickerWin</li>
<li>relatedButton</li>
<li>currentPlgNode</li>
</ul>
</td></tr>
<tr><td><b><font color = #4caf50>Methods:  </font></b></td><td><ul>
<li><b><a href="#clearScriptTARGET">clearScript </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#clearControlsTARGET">clearControls </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#createAndLoadPlgTARGET">createAndLoadPlg </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#runScriptTARGET">runScript </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#acquirePickerWinTARGET">acquirePickerWin </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#acquireRelatedButtonForPlgTARGET">acquireRelatedButtonForPlg </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#addSceneSelectedControlsTARGET">addSceneSelectedControls </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#updateControlsSelectTARGET">updateControlsSelect </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#updateActionScriptTARGET">updateActionScript </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#updateButtonColorTARGET">updateButtonColor </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#updateCtrlGroupTARGET">updateCtrlGroup </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#updatePreTARGET">updatePre </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#updateScaleTARGET">updateScale </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#updateSideTARGET">updateSide </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#updateButtonTextTARGET">updateButtonText </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#updateButtonTextColorTARGET">updateButtonTextColor </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#updateButtonFontTARGET">updateButtonFont </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#updateButtonFontSizeTARGET">updateButtonFontSize </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#connectSignalsTARGET">connectSignals </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#refreshPickerWindowTARGET">refreshPickerWindow </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#initViewTARGET">initView </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadSelectionTARGET">loadSelection </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#removeSceneSelectedControlsTARGET">removeSceneSelectedControls </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#replaceControlsTARGET">replaceControls </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#selectControlsTARGET">selectControls </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadWindowTARGET">loadWindow </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#clearViewTARGET">clearView </b></a> <font size = 2pt><i>[method]</i></font></li>
</ul>
</td>
</tr>
</table></font>
####MnsPLGSettingsUI  methods
<hr width = 50%>
<h5 id = "clearScriptTARGET"></h5><font color = 464646 size = 3><b>clearScript <font size = 2pt> [<a href="#MnsPLGSettingsUI TARGET">MnsPLGSettingsUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>'Clear' (ActionScript) button trigger.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>clearScript(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "clearControlsTARGET"></h5><font color = 464646 size = 3><b>clearControls <font size = 2pt> [<a href="#MnsPLGSettingsUI TARGET">MnsPLGSettingsUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>'Clear' (Controls Select) button trigger.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>clearControls(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "createAndLoadPlgTARGET"></h5><font color = 464646 size = 3><b>createAndLoadPlg <font size = 2pt> [<a href="#MnsPLGSettingsUI TARGET">MnsPLGSettingsUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>'Create PLG' button trigger.</i><br>
<i>A simple wrapper to create a new free plg, then selecting it and loading it into the UI.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createAndLoadPlg(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "runScriptTARGET"></h5><font color = 464646 size = 3><b>runScript <font size = 2pt> [<a href="#MnsPLGSettingsUI TARGET">MnsPLGSettingsUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>'Run Script' button trigger.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>runScript(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "acquirePickerWinTARGET"></h5><font color = 464646 size = 3><b>acquirePickerWin <font size = 2pt> [<a href="#MnsPLGSettingsUI TARGET">MnsPLGSettingsUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>A simple method to acquire a 'Picker' UI from global if exists.</i><br>
<i>This is done to manipultae a live picker in turn, instead of needing to refresh the picker.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>acquirePickerWin(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "acquireRelatedButtonForPlgTARGET"></h5><font color = 464646 size = 3><b>acquireRelatedButtonForPlg <font size = 2pt> [<a href="#MnsPLGSettingsUI TARGET">MnsPLGSettingsUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Acquire the related button to plg from a picker UI, if it exists.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>acquireRelatedButtonForPlg(self, plg)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>plg</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "addSceneSelectedControlsTARGET"></h5><font color = 464646 size = 3><b>addSceneSelectedControls <font size = 2pt> [<a href="#MnsPLGSettingsUI TARGET">MnsPLGSettingsUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Add current scene selection into the controls to select list.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>addSceneSelectedControls(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "updateControlsSelectTARGET"></h5><font color = 464646 size = 3><b>updateControlsSelect <font size = 2pt> [<a href="#MnsPLGSettingsUI TARGET">MnsPLGSettingsUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Button 'controls select' update requested trigger.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>updateControlsSelect(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "updateActionScriptTARGET"></h5><font color = 464646 size = 3><b>updateActionScript <font size = 2pt> [<a href="#MnsPLGSettingsUI TARGET">MnsPLGSettingsUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Button Action-script update requested trigger.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>updateActionScript(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "updateButtonColorTARGET"></h5><font color = 464646 size = 3><b>updateButtonColor <font size = 2pt> [<a href="#MnsPLGSettingsUI TARGET">MnsPLGSettingsUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Button color update requested trigger.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>updateButtonColor(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "updateCtrlGroupTARGET"></h5><font color = 464646 size = 3><b>updateCtrlGroup <font size = 2pt> [<a href="#MnsPLGSettingsUI TARGET">MnsPLGSettingsUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Button group update requested trigger.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>updateCtrlGroup(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "updatePreTARGET"></h5><font color = 464646 size = 3><b>updatePre <font size = 2pt> [<a href="#MnsPLGSettingsUI TARGET">MnsPLGSettingsUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Button pre checkbox update requested trigger.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>updatePre(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "updateScaleTARGET"></h5><font color = 464646 size = 3><b>updateScale <font size = 2pt> [<a href="#MnsPLGSettingsUI TARGET">MnsPLGSettingsUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Button scale update requested trigger.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>updateScale(self, size, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>size</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "updateSideTARGET"></h5><font color = 464646 size = 3><b>updateSide <font size = 2pt> [<a href="#MnsPLGSettingsUI TARGET">MnsPLGSettingsUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Button side update requested trigger.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>updateSide(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "updateButtonTextTARGET"></h5><font color = 464646 size = 3><b>updateButtonText <font size = 2pt> [<a href="#MnsPLGSettingsUI TARGET">MnsPLGSettingsUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Button text update requested trigger.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>updateButtonText(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "updateButtonTextColorTARGET"></h5><font color = 464646 size = 3><b>updateButtonTextColor <font size = 2pt> [<a href="#MnsPLGSettingsUI TARGET">MnsPLGSettingsUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Button text-color update requested trigger.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>updateButtonTextColor(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "updateButtonFontTARGET"></h5><font color = 464646 size = 3><b>updateButtonFont <font size = 2pt> [<a href="#MnsPLGSettingsUI TARGET">MnsPLGSettingsUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Button text-font update requested trigger.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>updateButtonFont(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "updateButtonFontSizeTARGET"></h5><font color = 464646 size = 3><b>updateButtonFontSize <font size = 2pt> [<a href="#MnsPLGSettingsUI TARGET">MnsPLGSettingsUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Button text-size update requested trigger.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>updateButtonFontSize(self, size)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>size</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "connectSignalsTARGET"></h5><font color = 464646 size = 3><b>connectSignals <font size = 2pt> [<a href="#MnsPLGSettingsUI TARGET">MnsPLGSettingsUI </a> class method] </font></font></b>
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
<h5 id = "refreshPickerWindowTARGET"></h5><font color = 464646 size = 3><b>refreshPickerWindow <font size = 2pt> [<a href="#MnsPLGSettingsUI TARGET">MnsPLGSettingsUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>In case a picker window is aquired, call it's 'refresh' method.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>refreshPickerWindow(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "initViewTARGET"></h5><font color = 464646 size = 3><b>initView <font size = 2pt> [<a href="#MnsPLGSettingsUI TARGET">MnsPLGSettingsUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Initialize view:</i><br>
<i>- Set title</i><br>
<i>- Set Icons</i><br>
<i>- Initialize sides comboBox</i><br>
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
<h5 id = "loadSelectionTARGET"></h5><font color = 464646 size = 3><b>loadSelection <font size = 2pt> [<a href="#MnsPLGSettingsUI TARGET">MnsPLGSettingsUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Main UI method- load current selection into the UI.</i><br>
<i>This method will handle reading, and acquiring all settings into the UI from the selected PLG (only it is a plg type).</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadSelection(self, **kwargs)</td></tr>
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
<h5 id = "removeSceneSelectedControlsTARGET"></h5><font color = 464646 size = 3><b>removeSceneSelectedControls <font size = 2pt> [<a href="#MnsPLGSettingsUI TARGET">MnsPLGSettingsUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Remove current selection from the controls list.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>removeSceneSelectedControls(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "replaceControlsTARGET"></h5><font color = 464646 size = 3><b>replaceControls <font size = 2pt> [<a href="#MnsPLGSettingsUI TARGET">MnsPLGSettingsUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Replace current 'controls list' with the current scene selection.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>replaceControls(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "selectControlsTARGET"></h5><font color = 464646 size = 3><b>selectControls <font size = 2pt> [<a href="#MnsPLGSettingsUI TARGET">MnsPLGSettingsUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Select current controls list btn trigger.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>selectControls(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "loadWindowTARGET"></h5><font color = 464646 size = 3><b>loadWindow <font size = 2pt> [<a href="#MnsPLGSettingsUI TARGET">MnsPLGSettingsUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Show windoe method.</i><br>
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
<h5 id = "clearViewTARGET"></h5><font color = 464646 size = 3><b>clearView <font size = 2pt> [<a href="#MnsPLGSettingsUI TARGET">MnsPLGSettingsUI </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>This method clears all setting from the UI, and restores 'empty' state.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>clearView(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
