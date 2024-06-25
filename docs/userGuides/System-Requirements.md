### Compatible Platforms
- Windows
- Linux (Tested on CentOS 7.9)

### Compatible Maya versions
<table cellpadding= 0 cellspacing = 0>
	<tr>
		<td></td>
		<td colspan=2>Maya 2018 - 2022</td>
		<td colspan=2>Maya 2023</td>
		<td colspan=2>Maya 2024</td>
	</tr>
	<tr>
		<td></td>
		<td>Win</td><td>Linux</td>
		<td>Win</td><td>Linux</td>
		<td>Win</td><td>Linux</td>
	</tr>
	<tr>
		<td>2.5.0</td>
		<td><span><CENTER>&#10022;</span></td><td><span><CENTER>&#10022;</span></td>
		<td><span><CENTER>&#10022;</span></td><td><span><CENTER>&#10022;</span></td>
		<td><span><CENTER>&#10022;</span></td><td><span><CENTER>&#10022;</span></td>
	</tr>
	<tr>
		<td>2.4.0</td>
		<td><span><CENTER>&#10022;</span></td><td><span><CENTER>&#10022;</span></td>
		<td><span><CENTER>&#10022;</span></td><td><span><CENTER>&#10022;</span></td>
		<td><span><CENTER>&#10022;</span></td><td><span><CENTER>&#10022;</span></td>
	</tr>
	<tr>
		<td>2.3.0</td>
		<td><span><CENTER>&#10022;</span></td><td><span><CENTER>&#10022;</span></td>
		<td><span><CENTER>&#10022;</span></td><td><span><CENTER>&#10022;</span></td>
		<td><span><CENTER>&#10022;</span></td><td><span><CENTER>&#10022;</span></td>
	</tr>
	<tr>
		<td>2.2.0</td>
		<td><span><CENTER>&#10022;</span></td><td><span><CENTER>&#10022;</span></td>
		<td><span><CENTER>&#10022;</span></td><td><span><CENTER>&#10022;</span></td>
		<td><span><CENTER>&#10022;</span></td><td><span><CENTER>&#10022;</span></td>
	</tr>
	<tr>
		<td>2.1.0</td>
		<td><span><CENTER>&#10022;</span></td><td><span><CENTER>&#10022;</span></td>
		<td><span><CENTER>&#10022;</span></td><td><span><CENTER>&#10022;</span></td>
		<td></td><td></td>
	</tr>
	<tr>
		<td>2.0.0</td>
		<td><span><CENTER>&#10022;</span></td><td><span><CENTER>&#10022;</span></td>
		<td></td><td></td>
		<td></td><td></td>
	</tr>
</table>

### Windows - System requirements
- <a href = "https://support.microsoft.com/en-ca/help/2977003/the-latest-supported-visual-c-downloads", target = "_blank">Microsoft Visual C++ Redistributable for Visual Studio 2015-2022</a>

!!! Important Note
    Microsoft Visual C++ Redistributable for Visual Studio 2015-2022 is a part of the native Maya installation.
    In most cases, no action is required to use Mansur-Rig in Maya.
    In some rare cases (incomplete Maya installation), if missing this component needs to be installed manually.

### Maya 2022, 2023 requirements

<ol>
<li>Mansur-Rig requires a native Maya python module - <b>PyMel</b>. For an unknown reason, Maya 2022 (and above) installation has this module for Python 3 presented as an optional feature. Worse then that, it is un-checked by default:</li>

<figure>
  <img src="../userGuidesImages/systemReq/maya2022InstallDialog.png"/>
  <figcaption>Maya 2022 installation dialog example</figcaption>
</figure>

<li>In case you installed Maya 2022 (and above) without this checked, Mansur-Rig manu would not show up once you install it. To check whether you have this component installed, simply run <i><b>'import pymel.core'</b></i> (without the qoutes) in a Python tab within Maya's script editor. if an error is logged, it means this reuqired component is <b>NOT</b> installed, and Mansur-Rig will not function. If this is the case for you, you have a few options available to resolve this issue:
<ol type="a">
	<li>Install PyMel for Python 3 on an existing Maya installation using <a href = "https://knowledge.autodesk.com/support/maya/learn-explore/caas/CloudHelp/cloudhelp/2022/ENU/Maya-Scripting/files/GUID-2AA5EFCE-53B1-46A0-8E43-4CD0B2C72FB4-htm.html" target = "_blank"><u><b>this guide</u></b></a>.</li>
	<li>Re-installing Maya, making sure you tick the PyMel checkbox.</li>
</ol>

</li>
</ol>

### Maya 2024 requirements

<ol>
<li>Mansur-Rig requires a native Maya python module - <b>PyMel</b>. For an unknown reason, Maya 2024 no longer presents PyMel module installation as an option for users.</li>
<li>Please use the following guide to install it:
<ol type="a">
	<li><a href = "https://help.autodesk.com/view/MAYAUL/2024/ENU/?guid=GUID-2AA5EFCE-53B1-46A0-8E43-4CD0B2C72FB4" target = "_blank"><u><b>Install PyMel for Python 3 on an existing Maya 2024 installation</u></b></a>.</li>
</ol>

</li>
</ol>