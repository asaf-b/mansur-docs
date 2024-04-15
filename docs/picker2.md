<body>
#picker2
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
<h5 id = "MnsPicker2 TARGET"></h5>
###MnsPicker2 [Class]
<font color = #5f5f5f size = 3pt>
<i>
Picker UI Class. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>MnsPicker2(<b>parent</b>(<i>str</i>) ; [default: mnsUIUtils.get_maya_window()])</td></tr>
<tr><td><b><font color = #4caf50>Inherits from:  </font></b></td><td>form_class, base_class</td></tr>
<tr><td><b><font color = #4caf50>Class Members:  </font></b></td>
<td><ul>
<ul>
<li>puppetPickersDict</li>
<li>currentTabWidget</li>
<li>bodyQGV</li>
<li>faceQGV</li>
<li>pickerWidth</li>
<li>pickerHeight</li>
<li>rigTops</li>
<li>rigTop</li>
<li>puppetRoot</li>
<li>pickerBase</li>
<li>namespace</li>
<li>tnPath</li>
<li>visRelationMapByRigTopKey</li>
<li>mayaSelectCallBack</li>
<li>newSceneCallback</li>
<li>sceneOpenedCallback</li>
</ul>
</td></tr>
<tr><td><b><font color = #4caf50>Methods:  </font></b></td><td><ul>
<li><b><a href="#attemptToGetImagesTARGET">attemptToGetImages </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#connectSignalsTARGET">connectSignals </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#createVisMapTARGET">createVisMap </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#createVisRelationMapForRigTopTARGET">createVisRelationMapForRigTop </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#deleteCallBacksTARGET">deleteCallBacks </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#destroyActionTARGET">destroyAction </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#displayHowToUseGuideTARGET">displayHowToUseGuide </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#drawPlgButtonTARGET">drawPlgButton </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#eventFilterTARGET">eventFilter </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getControllersInViewTARGET">getControllersInView </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getPlgPositionandSizeTARGET">getPlgPositionandSize </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#gridToggleTriggerTARGET">gridToggleTrigger </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#initializePuppetPickerTARGET">initializePuppetPicker </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#initializeUITARGET">initializeUI </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadWindowTARGET">loadWindow </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#newInstanceTARGET">newInstance </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#recSetInstanceNameTARGET">recSetInstanceName </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#refreshBtnStateTARGET">refreshBtnState </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#refreshButtonVisibilityTARGET">refreshButtonVisibility </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setBGImagesTARGET">setBGImages </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setBtnVisStateBasedOnPupetRootTARGET">setBtnVisStateBasedOnPupetRoot </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setBtnVisStateBasedOnPupetRootAttrTARGET">setBtnVisStateBasedOnPupetRootAttr </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setLocalVarsBasedOnCurrentRigTopTARGET">setLocalVarsBasedOnCurrentRigTop </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setRigTopTARGET">setRigTop </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setThumbnailTARGET">setThumbnail </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setWindowSizeTARGET">setWindowSize </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#validateVisCtrlTARGET">validateVisCtrl </b></a> <font size = 2pt><i>[method]</i></font></li>
</ul>
</td>
</tr>
</table></font>
####MnsPicker2  methods
<hr width = 50%>
<h5 id = "attemptToGetImagesTARGET"></h5><font color = 464646 size = 3><b>attemptToGetImages <font size = 2pt> [<a href="#MnsPicker2 TARGET">MnsPicker2 </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>attemptToGetImages(self, originPath, bodyBgImage, faceBgImage, tn, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>originPath</b></li>
<li><b>bodyBgImage</b></li>
<li><b>faceBgImage</b></li>
<li><b>tn</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "connectSignalsTARGET"></h5><font color = 464646 size = 3><b>connectSignals <font size = 2pt> [<a href="#MnsPicker2 TARGET">MnsPicker2 </a> class method] </font></font></b>
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
<h5 id = "createVisMapTARGET"></h5><font color = 464646 size = 3><b>createVisMap <font size = 2pt> [<a href="#MnsPicker2 TARGET">MnsPicker2 </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createVisMap(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "createVisRelationMapForRigTopTARGET"></h5><font color = 464646 size = 3><b>createVisRelationMapForRigTop <font size = 2pt> [<a href="#MnsPicker2 TARGET">MnsPicker2 </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createVisRelationMapForRigTop(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "deleteCallBacksTARGET"></h5><font color = 464646 size = 3><b>deleteCallBacks <font size = 2pt> [<a href="#MnsPicker2 TARGET">MnsPicker2 </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>deleteCallBacks(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "destroyActionTARGET"></h5><font color = 464646 size = 3><b>destroyAction <font size = 2pt> [<a href="#MnsPicker2 TARGET">MnsPicker2 </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>destroyAction(self, dummy = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>dummy</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "displayHowToUseGuideTARGET"></h5><font color = 464646 size = 3><b>displayHowToUseGuide <font size = 2pt> [<a href="#MnsPicker2 TARGET">MnsPicker2 </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>displayHowToUseGuide(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "drawPlgButtonTARGET"></h5><font color = 464646 size = 3><b>drawPlgButton <font size = 2pt> [<a href="#MnsPicker2 TARGET">MnsPicker2 </a> class method] </font></font></b>
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
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>drawPlgButton(self, plg, bodyQGV, faceQGV)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>plg</b></li>
<li><b>bodyQGV</b></li>
<li><b>faceQGV</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "eventFilterTARGET"></h5><font color = 464646 size = 3><b>eventFilter <font size = 2pt> [<a href="#MnsPicker2 TARGET">MnsPicker2 </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Override event filter to catch the close trigger to delete the callback</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>eventFilter(self, source, event)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>source</b></li>
<li><b>event</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getControllersInViewTARGET"></h5><font color = 464646 size = 3><b>getControllersInView <font size = 2pt> [<a href="#MnsPicker2 TARGET">MnsPicker2 </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getControllersInView(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getPlgPositionandSizeTARGET"></h5><font color = 464646 size = 3><b>getPlgPositionandSize <font size = 2pt> [<a href="#MnsPicker2 TARGET">MnsPicker2 </a> class method] </font></font></b>
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
<h5 id = "gridToggleTriggerTARGET"></h5><font color = 464646 size = 3><b>gridToggleTrigger <font size = 2pt> [<a href="#MnsPicker2 TARGET">MnsPicker2 </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>gridToggleTrigger(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "initializePuppetPickerTARGET"></h5><font color = 464646 size = 3><b>initializePuppetPicker <font size = 2pt> [<a href="#MnsPicker2 TARGET">MnsPicker2 </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Main method for the global UI draw.</i><br>
<i>The UI is initialy destroyed, then re-drawen.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>initializePuppetPicker(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "initializeUITARGET"></h5><font color = 464646 size = 3><b>initializeUI <font size = 2pt> [<a href="#MnsPicker2 TARGET">MnsPicker2 </a> class method] </font></font></b>
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
<h5 id = "loadWindowTARGET"></h5><font color = 464646 size = 3><b>loadWindow <font size = 2pt> [<a href="#MnsPicker2 TARGET">MnsPicker2 </a> class method] </font></font></b>
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
<h5 id = "newInstanceTARGET"></h5><font color = 464646 size = 3><b>newInstance <font size = 2pt> [<a href="#MnsPicker2 TARGET">MnsPicker2 </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>newInstance(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "recSetInstanceNameTARGET"></h5><font color = 464646 size = 3><b>recSetInstanceName <font size = 2pt> [<a href="#MnsPicker2 TARGET">MnsPicker2 </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>recSetInstanceName(self, idx = 0)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>idx</b>(<i>int</i>) ; [default: 0]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "refreshBtnStateTARGET"></h5><font color = 464646 size = 3><b>refreshBtnState <font size = 2pt> [<a href="#MnsPicker2 TARGET">MnsPicker2 </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>refreshBtnState(self, dummy = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>dummy</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "refreshButtonVisibilityTARGET"></h5><font color = 464646 size = 3><b>refreshButtonVisibility <font size = 2pt> [<a href="#MnsPicker2 TARGET">MnsPicker2 </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>refreshButtonVisibility(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setBGImagesTARGET"></h5><font color = 464646 size = 3><b>setBGImages <font size = 2pt> [<a href="#MnsPicker2 TARGET">MnsPicker2 </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Sets the bg image for the UI, in case there is one within the rig-top's attributes.</i><br>
<i>The bg cannot be set to multiple layouts, hence, a 'tab changed' trigger is connected to this method,</i><br>
<i>in order to toggle between the body and facial background images.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setBGImages(self, bodyQGV = None, faceQGV = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>bodyQGV</b>(<i>str</i>) ; [default: None]</li>
<li><b>faceQGV</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setBtnVisStateBasedOnPupetRootTARGET"></h5><font color = 464646 size = 3><b>setBtnVisStateBasedOnPupetRoot <font size = 2pt> [<a href="#MnsPicker2 TARGET">MnsPicker2 </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setBtnVisStateBasedOnPupetRoot(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setBtnVisStateBasedOnPupetRootAttrTARGET"></h5><font color = 464646 size = 3><b>setBtnVisStateBasedOnPupetRootAttr <font size = 2pt> [<a href="#MnsPicker2 TARGET">MnsPicker2 </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setBtnVisStateBasedOnPupetRootAttr(self, visAttr)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>visAttr</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setLocalVarsBasedOnCurrentRigTopTARGET"></h5><font color = 464646 size = 3><b>setLocalVarsBasedOnCurrentRigTop <font size = 2pt> [<a href="#MnsPicker2 TARGET">MnsPicker2 </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setLocalVarsBasedOnCurrentRigTop(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setRigTopTARGET"></h5><font color = 464646 size = 3><b>setRigTop <font size = 2pt> [<a href="#MnsPicker2 TARGET">MnsPicker2 </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setRigTop(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setThumbnailTARGET"></h5><font color = 464646 size = 3><b>setThumbnail <font size = 2pt> [<a href="#MnsPicker2 TARGET">MnsPicker2 </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setThumbnail(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setWindowSizeTARGET"></h5><font color = 464646 size = 3><b>setWindowSize <font size = 2pt> [<a href="#MnsPicker2 TARGET">MnsPicker2 </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setWindowSize(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "validateVisCtrlTARGET"></h5><font color = 464646 size = 3><b>validateVisCtrl <font size = 2pt> [<a href="#MnsPicker2 TARGET">MnsPicker2 </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>validateVisCtrl(self, node)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>node</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
<h5 id = "MnsPickerGraphicViewWidget TARGET"></h5>
###MnsPickerGraphicViewWidget [Class]
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>MnsPickerGraphicViewWidget(<b>parent</b>(<i>str</i>) ; [default: mnsUIUtils.get_maya_window()])</td></tr>
<tr><td><b><font color = #4caf50>Inherits from:  </font></b></td><td>QtWidgets.QGraphicsView</td></tr>
<tr><td><b><font color = #4caf50>Class Members:  </font></b></td>
<td><ul>
<ul>
<li>bgImage</li>
<li>graphicsPixmapItem</li>
<li>pickerWindowObj</li>
<li>sceneWidth</li>
<li>sceneHeight</li>
<li>mousePosition</li>
<li>isPanActive</li>
<li>isZoomActive</li>
<li>isRubberBandActive</li>
<li>topLeftPosition</li>
<li>zoomDelta</li>
<li>rubberBandGeometry</li>
<li>currentContentRect</li>
<li>tabWidget</li>
<li>tnPath</li>
</ul>
</td></tr>
<tr><td><b><font color = #4caf50>Methods:  </font></b></td><td><ul>
<li><b><a href="#connectSignalsTARGET">connectSignals </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#determaineSelectionTARGET">determaineSelection </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#drawConstantFGTARGET">drawConstantFG </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#drawForegroundTARGET">drawForeground </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#fitContentTARGET">fitContent </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getContentBoundingRectTARGET">getContentBoundingRect </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getControllersInViewTARGET">getControllersInView </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getSceneCenterPositionTARGET">getSceneCenterPosition </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getSelectedItemsTARGET">getSelectedItems </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#initializeGraphicsViewTARGET">initializeGraphicsView </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#keyPressEventTARGET">keyPressEvent </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#mouseMoveEventTARGET">mouseMoveEvent </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#mousePressEventTARGET">mousePressEvent </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#mouseReleaseEventTARGET">mouseReleaseEvent </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#resizeEventTARGET">resizeEvent </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setBGImageTARGET">setBGImage </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setCurrentStateRectTARGET">setCurrentStateRect </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#wheelEventTARGET">wheelEvent </b></a> <font size = 2pt><i>[method]</i></font></li>
</ul>
</td>
</tr>
</table></font>
####MnsPickerGraphicViewWidget  methods
<hr width = 50%>
<h5 id = "connectSignalsTARGET"></h5><font color = 464646 size = 3><b>connectSignals <font size = 2pt> [<a href="#MnsPickerGraphicViewWidget TARGET">MnsPickerGraphicViewWidget </a> class method] </font></font></b>
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
<h5 id = "determaineSelectionTARGET"></h5><font color = 464646 size = 3><b>determaineSelection <font size = 2pt> [<a href="#MnsPickerGraphicViewWidget TARGET">MnsPickerGraphicViewWidget </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>determaineSelection(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "drawConstantFGTARGET"></h5><font color = 464646 size = 3><b>drawConstantFG <font size = 2pt> [<a href="#MnsPickerGraphicViewWidget TARGET">MnsPickerGraphicViewWidget </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>drawConstantFG(self, painter, rect, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>painter</b></li>
<li><b>rect</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "drawForegroundTARGET"></h5><font color = 464646 size = 3><b>drawForeground <font size = 2pt> [<a href="#MnsPickerGraphicViewWidget TARGET">MnsPickerGraphicViewWidget </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>drawForeground(self, painter, rect)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>painter</b></li>
<li><b>rect</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "fitContentTARGET"></h5><font color = 464646 size = 3><b>fitContent <font size = 2pt> [<a href="#MnsPickerGraphicViewWidget TARGET">MnsPickerGraphicViewWidget </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>fitContent(self, fromSel = False)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>fromSel</b>(<i>bool</i>) ; [default: False]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getContentBoundingRectTARGET"></h5><font color = 464646 size = 3><b>getContentBoundingRect <font size = 2pt> [<a href="#MnsPickerGraphicViewWidget TARGET">MnsPickerGraphicViewWidget </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getContentBoundingRect(self, fromSel = False)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>fromSel</b>(<i>bool</i>) ; [default: False]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getControllersInViewTARGET"></h5><font color = 464646 size = 3><b>getControllersInView <font size = 2pt> [<a href="#MnsPickerGraphicViewWidget TARGET">MnsPickerGraphicViewWidget </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getControllersInView(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getSceneCenterPositionTARGET"></h5><font color = 464646 size = 3><b>getSceneCenterPosition <font size = 2pt> [<a href="#MnsPickerGraphicViewWidget TARGET">MnsPickerGraphicViewWidget </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getSceneCenterPosition(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getSelectedItemsTARGET"></h5><font color = 464646 size = 3><b>getSelectedItems <font size = 2pt> [<a href="#MnsPickerGraphicViewWidget TARGET">MnsPickerGraphicViewWidget </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getSelectedItems(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "initializeGraphicsViewTARGET"></h5><font color = 464646 size = 3><b>initializeGraphicsView <font size = 2pt> [<a href="#MnsPickerGraphicViewWidget TARGET">MnsPickerGraphicViewWidget </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>initializeGraphicsView(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "keyPressEventTARGET"></h5><font color = 464646 size = 3><b>keyPressEvent <font size = 2pt> [<a href="#MnsPickerGraphicViewWidget TARGET">MnsPickerGraphicViewWidget </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>keyPressEvent(self, event)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>event</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "mouseMoveEventTARGET"></h5><font color = 464646 size = 3><b>mouseMoveEvent <font size = 2pt> [<a href="#MnsPickerGraphicViewWidget TARGET">MnsPickerGraphicViewWidget </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>mouseMoveEvent(self, event)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>event</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "mousePressEventTARGET"></h5><font color = 464646 size = 3><b>mousePressEvent <font size = 2pt> [<a href="#MnsPickerGraphicViewWidget TARGET">MnsPickerGraphicViewWidget </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>mousePressEvent(self, event)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>event</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "mouseReleaseEventTARGET"></h5><font color = 464646 size = 3><b>mouseReleaseEvent <font size = 2pt> [<a href="#MnsPickerGraphicViewWidget TARGET">MnsPickerGraphicViewWidget </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>mouseReleaseEvent(self, event)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>event</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "resizeEventTARGET"></h5><font color = 464646 size = 3><b>resizeEvent <font size = 2pt> [<a href="#MnsPickerGraphicViewWidget TARGET">MnsPickerGraphicViewWidget </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>resizeEvent(self, event) </td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>event</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setBGImageTARGET"></h5><font color = 464646 size = 3><b>setBGImage <font size = 2pt> [<a href="#MnsPickerGraphicViewWidget TARGET">MnsPickerGraphicViewWidget </a> class method] </font></font></b>
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
<h5 id = "setCurrentStateRectTARGET"></h5><font color = 464646 size = 3><b>setCurrentStateRect <font size = 2pt> [<a href="#MnsPickerGraphicViewWidget TARGET">MnsPickerGraphicViewWidget </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setCurrentStateRect(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "wheelEventTARGET"></h5><font color = 464646 size = 3><b>wheelEvent <font size = 2pt> [<a href="#MnsPickerGraphicViewWidget TARGET">MnsPickerGraphicViewWidget </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>wheelEvent(self, event)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>event</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
<h5 id = "MnsPickerGraphicsScene TARGET"></h5>
###MnsPickerGraphicsScene [Class]
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>MnsPickerGraphicsScene(<b>parent</b>(<i>str</i>) ; [default: mnsUIUtils.get_maya_window()],<b>**kwargs</b>)</td></tr>
<tr><td><b><font color = #4caf50>Inherits from:  </font></b></td><td>QtWidgets.QGraphicsScene</td></tr>
<tr><td><b><font color = #4caf50>Class Members:  </font></b></td>
<td><ul>
<ul>
<li>sceneWidth</li>
<li>sceneHeight</li>
</ul>
</td></tr>
</tr>
</table></font>
<hr width = 100%>
<h5 id = "picker2QPushButton TARGET"></h5>
###picker2QPushButton [Class]
<font color = #5f5f5f size = 3pt>
<i>
A simple QPushButton re-implementation. <br>
This reimplementation is used to control the button's mouse events, used in 'Edit' mode. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>picker2QPushButton(<b>parent</b>(<i>str</i>) ; [default: None],<b>plgNode</b>(<i>str</i>) ; [default: None],<b>**kwargs</b>)</td></tr>
<tr><td><b><font color = #4caf50>Inherits from:  </font></b></td><td>QtWidgets.QPushButton</td></tr>
<tr><td><b><font color = #4caf50>Class Members:  </font></b></td>
<td><ul>
<ul>
<li>pickerWin</li>
<li>plgNode</li>
<li>connectedControls</li>
<li>directConnectedCtrl</li>
<li>isFacial</li>
<li>last</li>
<li>plgColor</li>
<li>textColor</li>
<li>text</li>
<li>isBold</li>
<li>isItalic</li>
<li>isUnderline</li>
<li>fontSize</li>
<li>positionH</li>
<li>positionV</li>
<li>scaleH</li>
<li>scaleV</li>
</ul>
</td></tr>
<tr><td><b><font color = #4caf50>Methods:  </font></b></td><td><ul>
<li><b><a href="#btnDoubleClickedTriggerTARGET">btnDoubleClickedTrigger </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#connectSignalsTARGET">connectSignals </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#filterConnectedControlsTARGET">filterConnectedControls </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#mouseDoubleClickEventTARGET">mouseDoubleClickEvent </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#pickerButtonClickActionTARGET">pickerButtonClickAction </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#rightClickedTriggerTARGET">rightClickedTrigger </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setButtonStyleTARGET">setButtonStyle </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setButtonVisTARGET">setButtonVis </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setPositionAndScaleTARGET">setPositionAndScale </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#updateButtonVisTARGET">updateButtonVis </b></a> <font size = 2pt><i>[method]</i></font></li>
</ul>
</td>
</tr>
</table></font>
####picker2QPushButton  methods
<hr width = 50%>
<h5 id = "btnDoubleClickedTriggerTARGET"></h5><font color = 464646 size = 3><b>btnDoubleClickedTrigger <font size = 2pt> [<a href="#picker2QPushButton TARGET">picker2QPushButton </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>The global action trigger for any picker UI button double click trigger.</i><br>
<i>   This method will trigger the "hierarchy selection" and the "action script" for the passed in QPushButton passed in.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>btnDoubleClickedTrigger(self, clickMode = "select")</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>clickMode</b>(<i>str</i>) ; [default: "select"]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "connectSignalsTARGET"></h5><font color = 464646 size = 3><b>connectSignals <font size = 2pt> [<a href="#picker2QPushButton TARGET">picker2QPushButton </a> class method] </font></font></b>
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
<h5 id = "filterConnectedControlsTARGET"></h5><font color = 464646 size = 3><b>filterConnectedControls <font size = 2pt> [<a href="#picker2QPushButton TARGET">picker2QPushButton </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>filterConnectedControls(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "mouseDoubleClickEventTARGET"></h5><font color = 464646 size = 3><b>mouseDoubleClickEvent <font size = 2pt> [<a href="#picker2QPushButton TARGET">picker2QPushButton </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>mouseDoubleClickEvent(self, QMouseEvent)</td></tr>
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
<h5 id = "pickerButtonClickActionTARGET"></h5><font color = 464646 size = 3><b>pickerButtonClickAction <font size = 2pt> [<a href="#picker2QPushButton TARGET">picker2QPushButton </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>The global action trigger for any picker UI button click trigger.</i><br>
<i>   This method will trigger the "controls selection" and the "action script" for the passed in QPushButton passed in.</i><br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>pickerButtonClickAction(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "rightClickedTriggerTARGET"></h5><font color = 464646 size = 3><b>rightClickedTrigger <font size = 2pt> [<a href="#picker2QPushButton TARGET">picker2QPushButton </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>rightClickedTrigger(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setButtonStyleTARGET"></h5><font color = 464646 size = 3><b>setButtonStyle <font size = 2pt> [<a href="#picker2QPushButton TARGET">picker2QPushButton </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setButtonStyle(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setButtonVisTARGET"></h5><font color = 464646 size = 3><b>setButtonVis <font size = 2pt> [<a href="#picker2QPushButton TARGET">picker2QPushButton </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setButtonVis(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setPositionAndScaleTARGET"></h5><font color = 464646 size = 3><b>setPositionAndScale <font size = 2pt> [<a href="#picker2QPushButton TARGET">picker2QPushButton </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setPositionAndScale(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "updateButtonVisTARGET"></h5><font color = 464646 size = 3><b>updateButtonVis <font size = 2pt> [<a href="#picker2QPushButton TARGET">picker2QPushButton </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>updateButtonVis(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
##Defenitions
<hr width = 100%>
###closeAllInstances
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>closeAllInstances(idx = 0)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>idx</b>(<i>int</i>) ; [default: 0]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###loadPicker
<font color = #5f5f5f size = 3pt>
<i>
Load the Def Serach UI from globals, avoid UI duplication. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadPicker() </td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
