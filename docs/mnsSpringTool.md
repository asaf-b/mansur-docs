<body>
#mnsSpringTool
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur === <br>
 <br>
</font>
</i>
<hr width = 100%>
##Classes
<hr width = 100%>
<h5 id = "MnsGradientWidget TARGET"></h5>
###MnsGradientWidget [Class]
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>MnsGradientWidget(<b>parent</b>(<i>str</i>) ; [default: None])</td></tr>
<tr><td><b><font color = #4caf50>Inherits from:  </font></b></td><td>QtWidgets.QWidget</td></tr>
<tr><td><b><font color = #4caf50>Class Members:  </font></b></td>
<td><ul>
<ul>
<li>initialized</li>
<li>currentSpringNodes</li>
<li>refSpringNode</li>
<li>attrName</li>
<li>origValues</li>
</ul>
</td></tr>
<tr><td><b><font color = #4caf50>Methods:  </font></b></td><td><ul>
<li><b><a href="#gatherCurrentValuesTARGET">gatherCurrentValues </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#paintEventTARGET">paintEvent </b></a> <font size = 2pt><i>[method]</i></font></li>
</ul>
</td>
</tr>
</table></font>
####MnsGradientWidget  methods
<hr width = 50%>
<h5 id = "gatherCurrentValuesTARGET"></h5><font color = 464646 size = 3><b>gatherCurrentValues <font size = 2pt> [<a href="#MnsGradientWidget TARGET">MnsGradientWidget </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>gatherCurrentValues(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "paintEventTARGET"></h5><font color = 464646 size = 3><b>paintEvent <font size = 2pt> [<a href="#MnsGradientWidget TARGET">MnsGradientWidget </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>paintEvent(self, event)</td></tr>
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
<h5 id = "MnsSpringTool TARGET"></h5>
###MnsSpringTool [Class]
<font color = #5f5f5f size = 3pt>
<i>
Spring Tool UI Class. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>MnsSpringTool(<b>parent</b>(<i>str</i>) ; [default: mnsUIUtils.get_maya_window()])</td></tr>
<tr><td><b><font color = #4caf50>Inherits from:  </font></b></td><td>form_class, base_class</td></tr>
<tr><td><b><font color = #4caf50>Class Members:  </font></b></td>
<td><ul>
<ul>
<li>rigTops</li>
<li>rigTop</li>
<li>puppetRoot</li>
<li>namespace</li>
<li>springNodes</li>
<li>springNodesByIndex</li>
<li>currentSpringNodes</li>
<li>drawType</li>
<li>stifGradCtrl</li>
<li>dampingGradCtrl</li>
</ul>
</td></tr>
<tr><td><b><font color = #4caf50>Methods:  </font></b></td><td><ul>
<li><b><a href="#collectSpringNodesTARGET">collectSpringNodes </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#connectSignalsTARGET">connectSignals </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#drawCommonAttrsToUiTARGET">drawCommonAttrsToUi </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#drawCurveSpringNodeToUITARGET">drawCurveSpringNodeToUI </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#drawTransformSpringNodeToUITARGET">drawTransformSpringNodeToUI </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#filterViewTARGET">filterView </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getCurrentSpringNodesTARGET">getCurrentSpringNodes </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getGradientControlTARGET">getGradientControl </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#initializeDataTARGET">initializeData </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#initializeSpringsTARGET">initializeSprings </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#initializeViewTARGET">initializeView </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadWindowTARGET">loadWindow </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setRigTopTARGET">setRigTop </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setSpringNodeTARGET">setSpringNode </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setValueTriggerTARGET">setValueTrigger </b></a> <font size = 2pt><i>[method]</i></font></li>
</ul>
</td>
</tr>
</table></font>
####MnsSpringTool  methods
<hr width = 50%>
<h5 id = "collectSpringNodesTARGET"></h5><font color = 464646 size = 3><b>collectSpringNodes <font size = 2pt> [<a href="#MnsSpringTool TARGET">MnsSpringTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>collectSpringNodes(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "connectSignalsTARGET"></h5><font color = 464646 size = 3><b>connectSignals <font size = 2pt> [<a href="#MnsSpringTool TARGET">MnsSpringTool </a> class method] </font></font></b>
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
<h5 id = "drawCommonAttrsToUiTARGET"></h5><font color = 464646 size = 3><b>drawCommonAttrsToUi <font size = 2pt> [<a href="#MnsSpringTool TARGET">MnsSpringTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>drawCommonAttrsToUi(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "drawCurveSpringNodeToUITARGET"></h5><font color = 464646 size = 3><b>drawCurveSpringNodeToUI <font size = 2pt> [<a href="#MnsSpringTool TARGET">MnsSpringTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>drawCurveSpringNodeToUI(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "drawTransformSpringNodeToUITARGET"></h5><font color = 464646 size = 3><b>drawTransformSpringNodeToUI <font size = 2pt> [<a href="#MnsSpringTool TARGET">MnsSpringTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>drawTransformSpringNodeToUI(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "filterViewTARGET"></h5><font color = 464646 size = 3><b>filterView <font size = 2pt> [<a href="#MnsSpringTool TARGET">MnsSpringTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>filterView(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getCurrentSpringNodesTARGET"></h5><font color = 464646 size = 3><b>getCurrentSpringNodes <font size = 2pt> [<a href="#MnsSpringTool TARGET">MnsSpringTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getCurrentSpringNodes(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getGradientControlTARGET"></h5><font color = 464646 size = 3><b>getGradientControl <font size = 2pt> [<a href="#MnsSpringTool TARGET">MnsSpringTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getGradientControl(self, attr = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>attr</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "initializeDataTARGET"></h5><font color = 464646 size = 3><b>initializeData <font size = 2pt> [<a href="#MnsSpringTool TARGET">MnsSpringTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>initializeData(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "initializeSpringsTARGET"></h5><font color = 464646 size = 3><b>initializeSprings <font size = 2pt> [<a href="#MnsSpringTool TARGET">MnsSpringTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>initializeSprings(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "initializeViewTARGET"></h5><font color = 464646 size = 3><b>initializeView <font size = 2pt> [<a href="#MnsSpringTool TARGET">MnsSpringTool </a> class method] </font></font></b>
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
<h5 id = "loadWindowTARGET"></h5><font color = 464646 size = 3><b>loadWindow <font size = 2pt> [<a href="#MnsSpringTool TARGET">MnsSpringTool </a> class method] </font></font></b>
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
<h5 id = "setRigTopTARGET"></h5><font color = 464646 size = 3><b>setRigTop <font size = 2pt> [<a href="#MnsSpringTool TARGET">MnsSpringTool </a> class method] </font></font></b>
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
<h5 id = "setSpringNodeTARGET"></h5><font color = 464646 size = 3><b>setSpringNode <font size = 2pt> [<a href="#MnsSpringTool TARGET">MnsSpringTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setSpringNode(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setValueTriggerTARGET"></h5><font color = 464646 size = 3><b>setValueTrigger <font size = 2pt> [<a href="#MnsSpringTool TARGET">MnsSpringTool </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setValueTrigger(self, attr, value)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>attr</b></li>
<li><b>value</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
##Defenitions
<hr width = 100%>
###loadSpringTool
<font color = #5f5f5f size = 3pt>
<i>
Load the Def Serach UI from globals, avoid UI duplication. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>loadSpringTool() </td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
