<body>
#webAppSimulator
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
PluginRelease UI Class. <br>
=== Author: Assaf Ben Zur === <br>
 <br>
</font>
</i>
<hr width = 100%>
##Classes
<hr width = 100%>
<h5 id = "MnsWebAppSimulator TARGET"></h5>
###MnsWebAppSimulator [Class]
<font color = #5f5f5f size = 3pt>
<i>
pluginRelease UI class <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>MnsWebAppSimulator(<b>parent</b>(<i>str</i>) ; [default: mnsUIUtils.get_maya_window()])</td></tr>
<tr><td><b><font color = #4caf50>Inherits from:  </font></b></td><td>form_class, base_class</td></tr>
<tr><td><b><font color = #4caf50>Class Members:  </font></b></td>
<td><ul>
<ul>
<li>mainFolderPath</li>
<li>keygenDBFilePath</li>
<li>TCODBFilePath</li>
</ul>
</td></tr>
<tr><td><b><font color = #4caf50>Methods:  </font></b></td><td><ul>
<li><b><a href="#assignLicenseTARGET">assignLicense </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#clearDBsTARGET">clearDBs </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#createNewUserTARGET">createNewUser </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getLicenseSelectionTARGET">getLicenseSelection </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getNewTCOCustomerIDTARGET">getNewTCOCustomerID </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getSubSelectionTARGET">getSubSelection </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getUserSelectionTARGET">getUserSelection </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#initDisplayTARGET">initDisplay </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#licenseExpiredTriggerTARGET">licenseExpiredTrigger </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#readKeygenDBTARGET">readKeygenDB </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#readTCODBTARGET">readTCODB </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#refreshDataTARGET">refreshData </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#retreiveLicenseTARGET">retreiveLicense </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setLicenseActionsTARGET">setLicenseActions </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setSubActionsTARGET">setSubActions </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#setUserActionsTARGET">setUserActions </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#subRenewTriggerTARGET">subRenewTrigger </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#tcoLicExpiredTriggerTARGET">tcoLicExpiredTrigger </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#writeKeygenDBTARGET">writeKeygenDB </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#writeTCODBTARGET">writeTCODB </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getHexFromInputTARGET">getHexFromInput </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getLicenseTARGET">getLicense </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getLicenseDirectOwnerIdentifierTARGET">getLicenseDirectOwnerIdentifier </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#displayMessageTARGET">displayMessage </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getLicenseOwnerTARGET">getLicenseOwner </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#createLicenseTARGET">createLicense </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#convertStringToBoolTARGET">convertStringToBool </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getSeatPriceTARGET">getSeatPrice </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#launch2COInlinePaymentTARGET">launch2COInlinePayment </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getUserLicensesTARGET">getUserLicenses </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getUserPayedLicensesTARGET">getUserPayedLicenses </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#getUserIdentifierFromUsernameTARGET">getUserIdentifierFromUsername </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#connectSignalsTARGET">connectSignals </b></a> <font size = 2pt><i>[method]</i></font></li>
<li><b><a href="#loadWindowTARGET">loadWindow </b></a> <font size = 2pt><i>[method]</i></font></li>
</ul>
</td>
</tr>
</table></font>
####MnsWebAppSimulator  methods
<hr width = 50%>
<h5 id = "assignLicenseTARGET"></h5><font color = 464646 size = 3><b>assignLicense <font size = 2pt> [<a href="#MnsWebAppSimulator TARGET">MnsWebAppSimulator </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>assignLicense(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "clearDBsTARGET"></h5><font color = 464646 size = 3><b>clearDBs <font size = 2pt> [<a href="#MnsWebAppSimulator TARGET">MnsWebAppSimulator </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>clearDBs(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "createNewUserTARGET"></h5><font color = 464646 size = 3><b>createNewUser <font size = 2pt> [<a href="#MnsWebAppSimulator TARGET">MnsWebAppSimulator </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createNewUser(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getLicenseSelectionTARGET"></h5><font color = 464646 size = 3><b>getLicenseSelection <font size = 2pt> [<a href="#MnsWebAppSimulator TARGET">MnsWebAppSimulator </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getLicenseSelection(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getNewTCOCustomerIDTARGET"></h5><font color = 464646 size = 3><b>getNewTCOCustomerID <font size = 2pt> [<a href="#MnsWebAppSimulator TARGET">MnsWebAppSimulator </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getNewTCOCustomerID(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getSubSelectionTARGET"></h5><font color = 464646 size = 3><b>getSubSelection <font size = 2pt> [<a href="#MnsWebAppSimulator TARGET">MnsWebAppSimulator </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getSubSelection(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getUserSelectionTARGET"></h5><font color = 464646 size = 3><b>getUserSelection <font size = 2pt> [<a href="#MnsWebAppSimulator TARGET">MnsWebAppSimulator </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getUserSelection(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "initDisplayTARGET"></h5><font color = 464646 size = 3><b>initDisplay <font size = 2pt> [<a href="#MnsWebAppSimulator TARGET">MnsWebAppSimulator </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>initDisplay(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "licenseExpiredTriggerTARGET"></h5><font color = 464646 size = 3><b>licenseExpiredTrigger <font size = 2pt> [<a href="#MnsWebAppSimulator TARGET">MnsWebAppSimulator </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>licenseExpiredTrigger(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "readKeygenDBTARGET"></h5><font color = 464646 size = 3><b>readKeygenDB <font size = 2pt> [<a href="#MnsWebAppSimulator TARGET">MnsWebAppSimulator </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>readKeygenDB(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "readTCODBTARGET"></h5><font color = 464646 size = 3><b>readTCODB <font size = 2pt> [<a href="#MnsWebAppSimulator TARGET">MnsWebAppSimulator </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>readTCODB(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "refreshDataTARGET"></h5><font color = 464646 size = 3><b>refreshData <font size = 2pt> [<a href="#MnsWebAppSimulator TARGET">MnsWebAppSimulator </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>refreshData(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "retreiveLicenseTARGET"></h5><font color = 464646 size = 3><b>retreiveLicense <font size = 2pt> [<a href="#MnsWebAppSimulator TARGET">MnsWebAppSimulator </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>retreiveLicense(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setLicenseActionsTARGET"></h5><font color = 464646 size = 3><b>setLicenseActions <font size = 2pt> [<a href="#MnsWebAppSimulator TARGET">MnsWebAppSimulator </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setLicenseActions(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setSubActionsTARGET"></h5><font color = 464646 size = 3><b>setSubActions <font size = 2pt> [<a href="#MnsWebAppSimulator TARGET">MnsWebAppSimulator </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setSubActions(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "setUserActionsTARGET"></h5><font color = 464646 size = 3><b>setUserActions <font size = 2pt> [<a href="#MnsWebAppSimulator TARGET">MnsWebAppSimulator </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setUserActions(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "subRenewTriggerTARGET"></h5><font color = 464646 size = 3><b>subRenewTrigger <font size = 2pt> [<a href="#MnsWebAppSimulator TARGET">MnsWebAppSimulator </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>subRenewTrigger(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "tcoLicExpiredTriggerTARGET"></h5><font color = 464646 size = 3><b>tcoLicExpiredTrigger <font size = 2pt> [<a href="#MnsWebAppSimulator TARGET">MnsWebAppSimulator </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>tcoLicExpiredTrigger(self)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "writeKeygenDBTARGET"></h5><font color = 464646 size = 3><b>writeKeygenDB <font size = 2pt> [<a href="#MnsWebAppSimulator TARGET">MnsWebAppSimulator </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>writeKeygenDB(self, data = {})</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>data</b>(<i>dict</i>) ; [default: {}]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "writeTCODBTARGET"></h5><font color = 464646 size = 3><b>writeTCODB <font size = 2pt> [<a href="#MnsWebAppSimulator TARGET">MnsWebAppSimulator </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>writeTCODB(self, data = {})</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>data</b>(<i>dict</i>) ; [default: {}]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getHexFromInputTARGET"></h5><font color = 464646 size = 3><b>getHexFromInput <font size = 2pt> [<a href="#MnsWebAppSimulator TARGET">MnsWebAppSimulator </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getHexFromInput(self, inputA = "")</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>inputA</b>(<i>str</i>) ; [default: ""]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getLicenseTARGET"></h5><font color = 464646 size = 3><b>getLicense <font size = 2pt> [<a href="#MnsWebAppSimulator TARGET">MnsWebAppSimulator </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getLicense(self, licIdentifier = "")</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>licIdentifier</b>(<i>str</i>) ; [default: ""]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getLicenseDirectOwnerIdentifierTARGET"></h5><font color = 464646 size = 3><b>getLicenseDirectOwnerIdentifier <font size = 2pt> [<a href="#MnsWebAppSimulator TARGET">MnsWebAppSimulator </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getLicenseDirectOwnerIdentifier(self, licIdentifier = "")</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>licIdentifier</b>(<i>str</i>) ; [default: ""]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "displayMessageTARGET"></h5><font color = 464646 size = 3><b>displayMessage <font size = 2pt> [<a href="#MnsWebAppSimulator TARGET">MnsWebAppSimulator </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>displayMessage(self, message = ["Test Message"], append = False)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>message</b>(<i>list</i>) ; [default: ["TestMessage"]]</li>
<li><b>append</b>(<i>bool</i>) ; [default: False]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getLicenseOwnerTARGET"></h5><font color = 464646 size = 3><b>getLicenseOwner <font size = 2pt> [<a href="#MnsWebAppSimulator TARGET">MnsWebAppSimulator </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getLicenseOwner(self, ownerIdentifier = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>ownerIdentifier</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "createLicenseTARGET"></h5><font color = 464646 size = 3><b>createLicense <font size = 2pt> [<a href="#MnsWebAppSimulator TARGET">MnsWebAppSimulator </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createLicense(self, policy = "Single-Seat")</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>policy</b>(<i>str</i>) ; [default: "Single-Seat"]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "convertStringToBoolTARGET"></h5><font color = 464646 size = 3><b>convertStringToBool <font size = 2pt> [<a href="#MnsWebAppSimulator TARGET">MnsWebAppSimulator </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>convertStringToBool(self, stringInput = "")</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>stringInput</b>(<i>str</i>) ; [default: ""]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getSeatPriceTARGET"></h5><font color = 464646 size = 3><b>getSeatPrice <font size = 2pt> [<a href="#MnsWebAppSimulator TARGET">MnsWebAppSimulator </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getSeatPrice(self, userIdentifier = "")</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>userIdentifier</b>(<i>str</i>) ; [default: ""]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "launch2COInlinePaymentTARGET"></h5><font color = 464646 size = 3><b>launch2COInlinePayment <font size = 2pt> [<a href="#MnsWebAppSimulator TARGET">MnsWebAppSimulator </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>launch2COInlinePayment(self, userIdentifier = "")</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>userIdentifier</b>(<i>str</i>) ; [default: ""]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getUserLicensesTARGET"></h5><font color = 464646 size = 3><b>getUserLicenses <font size = 2pt> [<a href="#MnsWebAppSimulator TARGET">MnsWebAppSimulator </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getUserLicenses(self, userIdentifier = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>userIdentifier</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getUserPayedLicensesTARGET"></h5><font color = 464646 size = 3><b>getUserPayedLicenses <font size = 2pt> [<a href="#MnsWebAppSimulator TARGET">MnsWebAppSimulator </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getUserPayedLicenses(self, userIdentifier = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>userIdentifier</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "getUserIdentifierFromUsernameTARGET"></h5><font color = 464646 size = 3><b>getUserIdentifierFromUsername <font size = 2pt> [<a href="#MnsWebAppSimulator TARGET">MnsWebAppSimulator </a> class method] </font></font></b>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getUserIdentifierFromUsername(self, username = "")</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>self</b></li>
<li><b>username</b>(<i>str</i>) ; [default: ""]</li>
</ul></td>
</tr>
<tr><td><b><font color = #4caf50>Optional Arguments:  </font></b></td>
</tr>
</table></font>
<h5 id = "connectSignalsTARGET"></h5><font color = 464646 size = 3><b>connectSignals <font size = 2pt> [<a href="#MnsWebAppSimulator TARGET">MnsWebAppSimulator </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Connect all the UI signals</i><br>
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
<h5 id = "loadWindowTARGET"></h5><font color = 464646 size = 3><b>loadWindow <font size = 2pt> [<a href="#MnsWebAppSimulator TARGET">MnsWebAppSimulator </a> class method] </font></font></b>
<font size = 2pt color= 595959><br>
<i>Main window load</i><br>
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
