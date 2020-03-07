<body>
#picker
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur === <br>
mnsPicker UI Class <br>
This is the UI defenition for the dynamic picker UI build. <br>
The picker is essentially defined by the user using scene guides and attributes,  <br>
this class handles the dynamic drawing of the picker into an actual live UI. <br>
- The global width and height attributes of the window is read from the "Picker Layout Base" <br>
- The picker buttons positions are read and interperted from the rig's 'Picker Layout Guides' <br>
- The buttons display settings and actions are drawen from each PLG attributes, which can be editted using the PLG Setting tool. <br>
 <br>
</font>
</i>
<hr width = 100%>
##Classes
<hr width = 100%>
<h5 id = "MnsPicker TARGET"></h5>
###MnsPicker [Class]
<font color = #5f5f5f size = 3pt>
<i>
Picker UI Class. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>MnsPicker(<b>parent</b>(<i>str</i>) ; [default: mnsUIUtils.get_maya_window()])</td></tr>
<tr><td><b><font color = #4caf50>Inherits from:  </font></b></td><td>form_class, base_class</td></tr>
<tr><td><b><font color = #4caf50>Class Members:  </font></b></td>
<td><ul>
<ul>
<li>iconsDir</li>
<li>rigTop</li>
<li>pickerBase</li>
<li>btnDrawDict</li>
</ul>
</td></tr>
<tr><td><b><font color = #4caf50>Methods:  </font></b></td><td><ul>
<li><b><a href="#btnClickedTriggerTARGET">btnClickedTrigger </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#connectSignalsTARGET">connectSignals </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#destroyUITARGET">destroyUI </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#initializeViewTARGET">initializeView </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getPlgPositionandSizeTARGET">getPlgPositionandSize </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#acquirePickerSettingsWinTARGET">acquirePickerSettingsWin </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setBGImageTARGET">setBGImage </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadWindowTARGET">loadWindow </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#openMenuTARGET">openMenu </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#drawPlgButtonTARGET">drawPlgButton </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setButtonHiddenStateBasedOnTypeTARGET">setButtonHiddenStateBasedOnType </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#editBtnTriggerTARGET">editBtnTrigger </b></a> <font size = 2pt><i>[method]</i></font></li>
</ul>
</td>
</tr>
</table></font>
####MnsPicker  methods
<hr width = 50%>
<h5 id = "btnClickedTriggerTARGET"></h5><font color = 464646 size = 3><b>btnClickedTrigger <font size = 2pt> [<a href="#MnsPicker TARGET">MnsPicker </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>A simple trigger method for a button click.</i><br>
<i>This trigger is re-implemented in order to 'catch' the 'edit' case.</i><br>
<i>In case the edit case is True, the button's Actions arn't executed, and the 'mouseMove' event is triggered.</i><br>
<i>In case the edit case is False, the btn's trigger actions is executed normally.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>btnClickedTrigger(self, plgBtn)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>plgBtn</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "connectSignalsTARGET"></h5><font color = 464646 size = 3><b>connectSignals <font size = 2pt> [<a href="#MnsPicker TARGET">MnsPicker </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Connect all UI Signals.</i><br>
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
<h5 id = "destroyUITARGET"></h5><font color = 464646 size = 3><b>destroyUI <font size = 2pt> [<a href="#MnsPicker TARGET">MnsPicker </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Destroys the entire dymanic UI draw.</i><br>
<i>This method is used to 'refresh' or 'redraw' the UI.</i><br>
<i>At any 'refresh' trigger, the UI needs to be completely destroyed then re-drawen with the current settings.</i><br>
</font>
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
<h5 id = "initializeViewTARGET"></h5><font color = 464646 size = 3><b>initializeView <font size = 2pt> [<a href="#MnsPicker TARGET">MnsPicker </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Main method for the global UI draw.</i><br>
<i>The UI is initialy destroyed, then re-drawen.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>initializeView(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getPlgPositionandSizeTARGET"></h5><font color = 464646 size = 3><b>getPlgPositionandSize <font size = 2pt> [<a href="#MnsPicker TARGET">MnsPicker </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Maps a PLG scene position to the UI's local layout position.</i><br>
<i>Since the positions of the PLG within the scene doesn't match the settings of QT,</i><br>
<i>this method maps the passed in plg position, in relation to the main 'Picker Layout Base',</i><br>
<i>and returns the new relative position to the UI layout.</i><br>
<i>This method also retunes the bounding box size of the given plg.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getPlgPositionandSize(self, plg)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td> list, list (plgPosition(x,y), plgSize (width, height))</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>plg</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "acquirePickerSettingsWinTARGET"></h5><font color = 464646 size = 3><b>acquirePickerSettingsWin <font size = 2pt> [<a href="#MnsPicker TARGET">MnsPicker </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Method to acquire the 'pickerSettings' tool from global, and store it.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>acquirePickerSettingsWin(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setBGImageTARGET"></h5><font color = 464646 size = 3><b>setBGImage <font size = 2pt> [<a href="#MnsPicker TARGET">MnsPicker </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Sets the bg image for the UI, in case there is one within the rig-top's attributes.</i><br>
<i>The bg cannot be set to multiple layouts, hence, a 'tab changed' trigger is connected to this method,</i><br>
<i>in order to toggle between the body and facial background images.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setBGImage(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "loadWindowTARGET"></h5><font color = 464646 size = 3><b>loadWindow <font size = 2pt> [<a href="#MnsPicker TARGET">MnsPicker </a> class method] </font></font></b>
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
<h5 id = "openMenuTARGET"></h5><font color = 464646 size = 3><b>openMenu <font size = 2pt> [<a href="#MnsPicker TARGET">MnsPicker </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Simple method to define the 'right-click-context-menu' trigger event.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>openMenu(self, plgBtn, position)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>plgBtn</b></li>
<li><b>position</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "drawPlgButtonTARGET"></h5><font color = 464646 size = 3><b>drawPlgButton <font size = 2pt> [<a href="#MnsPicker TARGET">MnsPicker </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>This is the main dynamic button draw method.</i><br>
<i>Flow:</i><br>
<i>- Acquire PLG</i><br>
<i>- calculate local space position</i><br>
<i>- gather all relevant settings</i><br>
<i>- draw the button based on the gathered settings and position, and connect it's click signal.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>drawPlgButton(self, plg)</td></tr>
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
<h5 id = "setButtonHiddenStateBasedOnTypeTARGET"></h5><font color = 464646 size = 3><b>setButtonHiddenStateBasedOnType <font size = 2pt> [<a href="#MnsPicker TARGET">MnsPicker </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>This method is used to define the 'visibility' state for the given butoon.</i><br>
<i>The state is calculated by the attributes of the btn, and once established, the visibility state is set into the btns.</i><br>
<i>Instead of drawing only valid buttons according to the UI state, ALL of the buttons are drawen every time the UI is,</i><br>
<i>then this method is used to 'show' only valid ones.</i><br>
<i>UI state to process:</i><br>
<i>- 'primaries', 'secodaries' and 'tertiaries' buttons state</i><br>
<i>- Current tab (body or facial)</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setButtonHiddenStateBasedOnType(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "editBtnTriggerTARGET"></h5><font color = 464646 size = 3><b>editBtnTrigger <font size = 2pt> [<a href="#MnsPicker TARGET">MnsPicker </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Trigger method for the 'edit' command.</i><br>
<i>This method will attempt to open the 'PLGSettings Tool' UI, as well as load the selected btn related plg into it, if possible.</i><br>
<i>First the related scene plg is acquired and selected (if requested),</i><br>
<i>then, an 'acquire' attempt is made in order to catch the settings window from global (acquirePickerSettingsWin).</i><br>
<i>If the window was acquired seccessfully, its being loaded and a 'loadSelection' trigger is passed into it,</i><br>
<i>in order to load the requested related plg settings into the UI.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>editBtnTrigger(self, plgBtn)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>plgBtn</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
<h5 id = "pickerQPushButton TARGET"></h5>
###pickerQPushButton [Class]
<font color = #5f5f5f size = 3pt>
<i>
A simple QPushButton re-implementation. <br>
This reimplementation is used to control the button's mouse events, used in 'Edit' mode. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>pickerQPushButton(<b>parent</b>(<i>str</i>) ; [default: None])</td></tr>
<tr><td><b><font color = #4caf50>Inherits from:  </font></b></td><td>QtWidgets.QPushButton</td></tr>
<tr><td><b><font color = #4caf50>Class Members:  </font></b></td>
<td><ul>
<ul>
<li>plgNode</li>
<li>clickOffset</li>
</ul>
</td></tr>
<tr><td><b><font color = #4caf50>Methods:  </font></b></td><td><ul>
<li><b><a href="#mouseMoveEventTARGET">mouseMoveEvent </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#mouseReleaseEventTARGET">mouseReleaseEvent </b></a> <font size = 2pt><i>[method]</i></font></li>
</ul>
</td>
</tr>
</table></font>
####pickerQPushButton  methods
<hr width = 50%>
<h5 id = "mouseMoveEventTARGET"></h5><font color = 464646 size = 3><b>mouseMoveEvent <font size = 2pt> [<a href="#pickerQPushButton TARGET">pickerQPushButton </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Re implementation of the QMouseMove event trigger.</i><br>
<i>In addition to the default event, a 'btn move' implementation is added, in order for the user to move buttons across the UI in edit mode.</i><br>
<i>Once the trigger is called, an initial check of the 'edit' button is performed.</i><br>
<i>If the edit mode is on (editMode_btn.isChecked()), a move processing is established:</i><br>
<i>- A 'Click To Local' offset is calculated (as the position of the btn is dectated by the btn's top left corener)</i><br>
<i>- The button is translated into the new calculatd position (same position)</i><br>
<i>- When the mouse is moved, the btn is translated to it's new position taking the offset into acount.</i><br>
<i>A global boundingbox check is performed with every move, preventing the user from draging the button 'out of bounds'.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>mouseMoveEvent(self, QMouseEvent)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>QMouseEvent</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "mouseReleaseEventTARGET"></h5><font color = 464646 size = 3><b>mouseReleaseEvent <font size = 2pt> [<a href="#pickerQPushButton TARGET">pickerQPushButton </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>This event re-implementation is used to trigger an 'Button Position Edit' Finished event.</i><br>
<i>Once a user moved a button across the UI, and chosen a new position- meaning released the mouse press,</i><br>
<i>this event is triggered and the new position is set.</i><br>
<i>Then a process is called to re-position the related PLG within the scene, to store the new position correctly.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>mouseReleaseEvent(self, QMouseEvent)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>QMouseEvent</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
##Defenitions
<hr width = 100%>
###loadPicker
<font color = #5f5f5f size = 3pt>
<i>
A simple method to acquire any existing picker windows from global, and initiating a UI load based on the gathered data. <br>
This method also dectates the name of the UI object, based on the rig's 'name', to avoid duplicated UI's, <br>
As well as to allow for multiple pickers, connected to multiple rigs to be used at the same time. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadPicker()</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
