<body>
#chassis Settings
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
Author: Asaf Ben-Zur <br>
Best used for: chassis <br>
This module will yield four corner controls, which will be avaraged determine the main control's translation and orientation.  <br>
The aim of this module is creating an easy to use control for a chassis orientation on a vehicle. <br>
Using the four corner controls, the main joint will be avaraged to detrmine the best orientation and translation for the module. <br>
Best used alongside geometry constraints to follow a ground mesh for automatic orientation and translation of vehicles.   <br>
</i>
<br>
</font>
<hr width = 100%>
##Attributes
</table></font>
###GlobalSettings
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>forwardAxis</td>
<td>2</td>
<td>Forward direction of the vehicle. This will determine the up direction for the slave orientation.</td></tr>
<tr><td>pivotsControlShape</td>
<td>diamond</td>
<td>Chasis pivots control shape</td></tr>
<tr><td>slaveControlShape</td>
<td>cube</td>
<td>Main slave control shape</td></tr>
</table></font>
###groundControls
<table><tr><td><b><font size = 3pt color = #4caf50>Attribute Name</td><td><font color = #4caf50><b>Default</td><td><font color = #4caf50><b>Description</td></tr>
<tr><td>doGroundCtrls</td>
<td>False</td>
<td>Create ground controls</td></tr>
<tr><td>groundControlShape</td>
<td>arrow</td>
<td>ground controls shape</td></tr>
</table></font>
