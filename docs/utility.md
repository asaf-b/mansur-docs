<body>
#utility
<hr width = 100%>
<font color = #5f5f5f size = 3pt>
<i>
=== Author: Assaf Ben Zur === <br>
Global Core MNS utility module. <br>
This module holds any 'global' function used within MNS. <br>
A 'misc' style module. <br>
</font>
</i>
<hr width = 100%>
##Defenitions
<hr width = 100%>
###addAttrToObj
<font color = #5f5f5f size = 3pt>
<i>
A global conditioned wrapper for adding attributes to object/objects <br>
 <br>
Exceptions: <br>
1. Object to add attr to was found non-existing or invalid. Abort. <br>
2. The 'replace' flag wasn't set, and the attribute already exists. Abort. <br>
3. Attr name wasn't passed in. Abort. <br>
4. The attribute type passed doesn't match the attribute value passed. Abort. <br>
5. min/max values were passed in, although the attr type is not an Int or a Float. Skip min/max values. <br>
6. min/max values were passed, and the attr type is Int or Float, although the min/max values passed arn't matching the data type. Skip min/max. <br>
7. The replace flag was set to True, but the attribute doesn't exist. Ignore replace flag. <br>
 <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>addAttrToObj(objects = [], **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td> list (added attributes 'attr' objects list)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>objects</b>(<i>list</i>) ; [default: []]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
<td><ul>
<li><b>name</b>(<i>str</i>) - Added attribute name</li>
<li><b>replace</b>(<i>bool</i>) - If attr exists and this flag is set to True- delete the existing attribute then recreate according to parameters</li>
<li><b>type</b>(<i>str</i>) ; [default: string] - Added attribute type</li>
<li><b>value</b>(<i>str</i>) ; [default: None] - Added attribute value</li>
<li><b>max</b>(<i>str</i>) ; [default: None] - Added attribute max (only if float or int)</li>
<li><b>min</b>(<i>str</i>) ; [default: None] - Added attribute min (only if float or int)</li>
<li><b>locked</b>(<i>bool</i>) - Added attribute lock state</li>
<li><b>cb</b>(<i>bool</i>) ; [default: True] - Added attribute channelBox/Displayed state</li>
<li><b>keyable</b>(<i>bool</i>) ; [default: True] - Added attribute keyable state</li>
<li><b>enumDefault</b>(<i>int</i>) - If added attr is enum, set its default to this value</li>
</ul></td>
</tr>
</table></font>
<hr width = 100%>
###addBlockClasIDToObj
<font color = #5f5f5f size = 3pt>
<i>
Add a 'blkClassId' Attribute to the given input. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>addBlockClasIDToObj(objectA, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>PyAttribute ('blkClassID')</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>objectA</b></li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###applyChennelControlAttributesToTransform
<font color = #5f5f5f size = 3pt>
<i>
This method applies a 'channelControl' dict attributes into the given transform. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>applyChennelControlAttributesToTransform(transform = None, ccDict = {})</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>transform</b>(<i>str</i>) ; [default: None]</li>
<li><b>ccDict</b>(<i>dict</i>) ; [default: {}]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###checkFunctionRedundencyForPackage
<font color = #5f5f5f size = 3pt>
<i>
Check for any method redundency within the given python package. <br>
Loop through the entire code libarary, and for every method, check whether it is being called anywhere. <br>
In case the tested method isn't called once throught the entire code libarary, it is being flagged as redundent. <br>
NO ACTION IS PERFORMED. This is a query only method. <br>
This method doesn't return anything, it will only print the processed results in the command window. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>checkFunctionRedundencyForPackage(package, printRedundentOnly = True)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>package</b></li>
<li><b>printRedundentOnly</b>(<i>bool</i>) ; [default: True]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###checkIfObjExistsAndSet
<font color = #5f5f5f size = 3pt>
<i>
For the object passed in- <br>
three main cases: <br>
1. If it is a 'PyNode' object, set it as the object to check. <br>
2. If it is an MnsNameStd object,set it's .node property as the object to check. <br>
3. If it is a string, assign it into a 'PyNode' obhect and set it as the object to check. <br>
Check whether the object exists in the current scene and valid. <br>
If so, return it. Else return None. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>checkIfObjExistsAndSet(objB = None, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>PyNode if valid, None if not. </td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>objB</b>(<i>str</i>) ; [default: None]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
<td><ul>
<li><b>obj</b>(<i>str</i>) ; [default: objB] - object to act on and return</li>
</ul></td>
</tr>
</table></font>
<hr width = 100%>
###checkLocalAxisPairing
<font color = #5f5f5f size = 3pt>
<i>
This method will check and return local axis pairing. <br>
Main use is for pre-connection check for pocNode and curveVarNode tweakers (inputs), <br>
in order to link local axes correctly, avoiding the need to check aim and up axes, as well as the offset axes. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>checkLocalAxisPairing(origin = None, target = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td> dict (pairingDict - {"x", "y","z"})</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>origin</b>(<i>str</i>) ; [default: None]</li>
<li><b>target</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###connectShapeColorRGB
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>connectShapeColorRGB(source = None, target = None)</td></tr>
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
###convertAlphaToInt
<font color = #5f5f5f size = 3pt>
<i>
Recursive. Convert an Alpha input into an Int ID. Infinite. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>convertAlphaToInt(alpha = "A")</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>int</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>alpha</b>(<i>str</i>) ; [default: "A"]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###convertIntToAlpha
<font color = #5f5f5f size = 3pt>
<i>
Recursive. Convert an Int input into an Alpha ID. Infinite. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>convertIntToAlpha(intA = 0)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>string</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>intA</b>(<i>int</i>) ; [default: 0]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###convertNodeToNameStd
<font color = #5f5f5f size = 3pt>
<i>
Attempt to convert a given node into a MnsNameStd object. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>convertNodeToNameStd(node)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>node</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###createAxisLamberts
<font color = #5f5f5f size = 3pt>
<i>
An axes colored lambert shaders creation function. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createAxisLamberts(**kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>dict ('X': xAxisLambert, 'Y': yAixsLambert, 'Z': zAxisLambert)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
<td><ul>
<li><b>doX</b>(<i>bool</i>) ; [default: True]</li>
<li><b>doY</b>(<i>bool</i>) ; [default: True]</li>
<li><b>doZ</b>(<i>bool</i>) ; [default: True]</li>
<li><b>deleteAll</b>(<i>bool</i>) - If true, do not attempt to create any objects- instead look for any existing objects and delete them</li>
</ul></td>
</tr>
</table></font>
<hr width = 100%>
###createFreeOffsetGroup
<font color = #5f5f5f size = 3pt>
<i>
For the given transform, create a free offset group transform parent. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createFreeOffsetGroup(transformObject)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsNameStd (offsetGrp)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>transformObject</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###createNodeReturnNameStd
<font color = #5f5f5f size = 3pt>
<i>
A core major MNS function. <br>
This function creates a new node, based on it's type passed in, and it's name parameters passed in, and returns it as a MnsNameStd object. <br>
This function also contains the 'search for next valid name' functionallity: <br>
In case the given parameter set returns an object name that already exists within the current scene a 'Handle' functionallity will be triggered: <br>
- In case the 'IncrementAlpha' argument is Flase, recursivly increment the ID value until a new name slot is available within the scene. <br>
- In case it's Flase, do the same while incrementing the Alpha value instead. <br>
Unlike Maya's core behavior- This function tests whether an object name exists whithin the entire scene- not only whether it exists whithin the current hirarchy level. <br>
In a sequence manner creation- the Alpha/ID should be incremented within the caller function loop- meaning while bulding an item sequence the 'search' functionallity should not be used. <br>
Another funtionallity of this function is the 'Fix Shape Name' functionallity: <br>
A simple shpe children name test of an object (after creation) and a renaming them. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createNodeReturnNameStd(**kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsNameStd</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
<td><ul>
<li><b>side</b>(<i>str</i>) ; [default: center] - side flag</li>
<li><b>body</b>(<i>str</i>) ; [default: pointsOnCurve] - Node's name body.</li>
<li><b>alpha</b>(<i>str</i>) ; [default: A] - Node's Alpha id</li>
<li><b>id</b>(<i>int</i>) ; [default: 1] - Node's ID</li>
<li><b>incrementAlpha</b>(<i>bool</i>) - Search new node name incrementing Alpha instead of the id if True</li>
<li><b>buildType</b>(<i>int</i>)</li>
<li><b>createBlkClassID</b>(<i>bool</i>)</li>
<li><b>createBlkCtrlTypeID</b>(<i>bool</i>)</li>
<li><b>blkCtrlTypeID</b>(<i>int</i>)</li>
<li><b>parentNode</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
</table></font>
<hr width = 100%>
###createOffsetGroup
<font color = #5f5f5f size = 3pt>
<i>
For the given transform, create a predefined offset group transform parent. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createOffsetGroup(transformObject, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsNameStd (offsetGrp)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>transformObject</b></li>
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
###deleteFile
<font color = #5f5f5f size = 3pt>
<i>
A delete file global function that includes a pre-defined log write. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>deleteFile(file)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>file</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###distBetween
<font color = #5f5f5f size = 3pt>
<i>
Measure the distance between to maya transforms. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>distBetween(transformA = None, transformB = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>float (distance)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>transformA</b>(<i>str</i>) ; [default: None]</li>
<li><b>transformB</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###fixShapesName
<font color = #5f5f5f size = 3pt>
<i>
Simple shape name fix function based on parent's name. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>fixShapesName(objects = [])</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>objects</b>(<i>list</i>) ; [default: []]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getFirstLevelParentForObject
<font color = #5f5f5f size = 3pt>
<i>
Get the top level parent for a given object. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getFirstLevelParentForObject(obj)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>pyNode (top level parent)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>obj</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getNumLinesForDir
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getNumLinesForDir(directory = "D/mansurProject/mansurRig/scripts/mansur")</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>directory</b>(<i>str</i>) ; [default: "D:/mansurProject/mansurRig/scripts/mansur"]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getSideFromNode
<font color = #5f5f5f size = 3pt>
<i>
Attempt to collect the given input's side. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getSideFromNode(node)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>string (side)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>node</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getTopParentForObj
<font color = #5f5f5f size = 3pt>
<i>
Recursively attempt to fet the top node of the maya heirarchy, from the given input upwards. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getTopParentForObj(obj)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsNameStd (Top Parent)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>obj</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getTopParentForSel
<font color = #5f5f5f size = 3pt>
<i>
get the top node of the current selected object's maya heirarchy. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getTopParentForSel()</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsNameStd (Top Parent)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###importModuleFromPath
<font color = #5f5f5f size = 3pt>
<i>
Attempt to import the given path as a python package into the global scope. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>importModuleFromPath(path)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>pythonPkg</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>path</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###jointOrientToRotation
<font color = #5f5f5f size = 3pt>
<i>
Transfer all jointOrient attributes for the jnt hirerchy to rotations. <br>
Essentially bake the joint orient attributes for the joints. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>jointOrientToRotation(topNode = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>topNode</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###lockAndHideAllTransforms
<font color = #5f5f5f size = 3pt>
<i>
Lock and hide all of the given node's attributes. <br>
Override flags can be inserted to skip requested channels. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>lockAndHideAllTransforms(node = None, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>bool</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>node</b>(<i>str</i>) ; [default: None]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
<td><ul>
<li><b>lock</b>(<i>bool</i>)</li>
<li><b>keyable</b>(<i>bool</i>)</li>
<li><b>cb</b>(<i>bool</i>)</li>
<li><b>t</b>(<i>bool</i>) ; [default: True]</li>
<li><b>r</b>(<i>bool</i>) ; [default: True]</li>
<li><b>s</b>(<i>bool</i>) ; [default: True]</li>
<li><b>t</b>(<i>bool</i>) ; [default: True]</li>
<li><b>r</b>(<i>bool</i>) ; [default: True]</li>
<li><b>s</b>(<i>bool</i>) ; [default: True]</li>
</ul></td>
</tr>
</table></font>
<hr width = 100%>
###lockAndHideTransforms
<font color = #5f5f5f size = 3pt>
<i>
Based on the given flags, lock/unlock, hide/unhide attributes for the given node. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>lockAndHideTransforms(node = None, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>bool</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>node</b>(<i>str</i>) ; [default: None]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
<td><ul>
<li><b>lock</b>(<i>bool</i>)</li>
<li><b>keyable</b>(<i>bool</i>)</li>
<li><b>cb</b>(<i>bool</i>)</li>
<li><b>tx</b>(<i>bool</i>) ; [default: True]</li>
<li><b>ty</b>(<i>bool</i>) ; [default: True]</li>
<li><b>tz</b>(<i>bool</i>) ; [default: True]</li>
<li><b>rx</b>(<i>bool</i>) ; [default: True]</li>
<li><b>ry</b>(<i>bool</i>) ; [default: True]</li>
<li><b>rz</b>(<i>bool</i>) ; [default: True]</li>
<li><b>sx</b>(<i>bool</i>) ; [default: True]</li>
<li><b>sy</b>(<i>bool</i>) ; [default: True]</li>
<li><b>sz</b>(<i>bool</i>) ; [default: True]</li>
</ul></td>
</tr>
</table></font>
<hr width = 100%>
###objectArrayValidExistsCheckReturn
<font color = #5f5f5f size = 3pt>
<i>
MNS core object array validity check. <br>
Two main Cases for the mode parameter: <br>
1. trueOnlyIfAllValid - Run through the objects and only if ALL of them are found existing and valid, return the array back to the caller. If a single item failed- Return None. <br>
2. trueIfSomeValid - Check all the objects and return any or all of them based on validity. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>objectArrayValidExistsCheckReturn(**kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>List (Valid object list), None (If found invalid)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
<td><ul>
<li><b>objectArray</b>(<i>list</i>) ; [default: [' ']] - Objects input list</li>
<li><b>mode</b>(<i>int</i>) - Validity return mode</li>
</ul></td>
</tr>
</table></font>
<hr width = 100%>
###readJson
<font color = #5f5f5f size = 3pt>
<i>
Read the input json path into formatted python variables. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>readJson(fullPath)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>FormattedPythonJson</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>fullPath</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###readSetteingFromFile
<font color = #5f5f5f size = 3pt>
<i>
Read mns setting from a given file and collect into a dict. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>readSetteingFromFile(settingsPath)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>dict (arguments)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>settingsPath</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###returnIndexFromSideDict
<font color = #5f5f5f size = 3pt>
<i>
Return the corresponding index from the pre-defined input dictionary, for the given input elenment. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>returnIndexFromSideDict(dict, searchElement)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>int (index)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>dict</b></li>
<li><b>searchElement</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###returnKeyFromElementTypeDict
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>returnKeyFromElementTypeDict(dict, searchElement)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>dict</b></li>
<li><b>searchElement</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###returnNameStdChangeElement
<font color = #5f5f5f size = 3pt>
<i>
global MnsNameStd utility- <br>
Use this function to change any elemnt within a given MnsNameStd object based on keyword args given <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>returnNameStdChangeElement(nameStd = None, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsNameStd</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>nameStd</b>(<i>str</i>) ; [default: None]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
<td><ul>
<li><b>autoRename</b>(<i>bool</i>) ; [default: True]</li>
<li><b>bodyPattern</b>(<i>str</i>) ; [default: None]</li>
<li><b>node</b>(<i>str</i>) ; [default: nameStd.node] - change node parameter</li>
<li><b>side</b>(<i>str</i>) ; [default: nameStd.side] - change side parameter</li>
<li><b>body</b>(<i>str</i>) ; [default: nameStd.body] - change body parameter</li>
<li><b>type</b>(<i>str</i>) ; [default: nameStd.type] - change type parameter</li>
<li><b>id</b>(<i>str</i>) ; [default: nameStd.id] - change id parameter</li>
<li><b>alpha</b>(<i>str</i>) ; [default: nameStd.alpha] - change alpha parameter</li>
<li><b>suffix</b>(<i>str</i>) ; [default: nameStd.suffix] - change suffix</li>
<li><b>comment</b>(<i>str</i>) ; [default: nameStd.comment] - change comment parameter</li>
</ul></td>
</tr>
</table></font>
<hr width = 100%>
###setAttr
<font color = #5f5f5f size = 3pt>
<i>
mns set attr. <br>
Simple method to set attributes.  <br>
two cases: <br>
1. attribute isn't locked - set the value <br>
2. attribute is locked - unlock the attribute, set it's value, and re-lock the attribute. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setAttr(attr, value)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>attr</b></li>
<li><b>value</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###setCtrlColorIdx
<font color = #5f5f5f size = 3pt>
<i>
Global utility function: <br>
Change the shape color override to index type, and set to the input value index <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setCtrlColorIdx(objects = [], colorIdx = 0)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>objects</b>(<i>list</i>) ; [default: []]</li>
<li><b>colorIdx</b>(<i>int</i>) ; [default: 0]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###setCtrlColorRGB
<font color = #5f5f5f size = 3pt>
<i>
Global utility function: <br>
Change the shape color override to RGB type, and set to the input value RGB <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>setCtrlColorRGB(objects = [], color = (1,1,1))</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>objects</b>(<i>list</i>) ; [default: []]</li>
<li><b>color</b>(<i>str</i>) ; [default: (1]</li>
<li><b>1</b></li>
<li><b>1)</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###sortNameStdArrayByID
<font color = #5f5f5f size = 3pt>
<i>
Attempt to sort the given array based on it's content ID's. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>sortNameStdArrayByID(nameStdArray)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>list (sorted list)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>nameStdArray</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###sorted_alphanumeric
<font color = #5f5f5f size = 3pt>
<i>
returns an alphanumeric ordered data from input given <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>sorted_alphanumeric(data)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>data</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###splitDateTimeStringToList
<font color = #5f5f5f size = 3pt>
<i>
Split a 'dateTime' string to a major/minor/patch/timestemp list <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>splitDateTimeStringToList(dateTime = "")</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>list</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>dateTime</b>(<i>str</i>) ; [default: ""]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###splitEnumAttrToChannelControlList
<font color = #5f5f5f size = 3pt>
<i>
Split a pre-defined 'channel-control' enum attribute into a formatted python dict. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>splitEnumAttrToChannelControlList(enumAttrName, node)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>dict (formatted dictionary)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>enumAttrName</b></li>
<li><b>node</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###splitEnumAttrToColorSchemeFloatTupleList
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>splitEnumAttrToColorSchemeFloatTupleList(enumAttrName, node)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>list (formatted list of tuples)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>enumAttrName</b></li>
<li><b>node</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###splitEnumToStringList
<font color = #5f5f5f size = 3pt>
<i>
Split the given enum attribute is a formated python list. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>splitEnumToStringList(enumAttrName, node)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>list (formated list)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>enumAttrName</b></li>
<li><b>node</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###splitNameStringToNameStd
<font color = #5f5f5f size = 3pt>
<i>
Split a given string object and return a MnsNameStd based on it's structure. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>splitNameStringToNameStd(nameString = "")</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsNameStd</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>nameString</b>(<i>str</i>) ; [default: ""]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###validateAttrAndGet
<font color = #5f5f5f size = 3pt>
<i>
For the given transform (or nameStd)- check whether the given attr exists. <br>
If the attr exist, get it and return it. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>validateAttrAndGet(transform = None, attrName = "", default = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td> bool (return status), unknownType (value)</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>transform</b>(<i>str</i>) ; [default: None]</li>
<li><b>attrName</b>(<i>str</i>) ; [default: ""]</li>
<li><b>default</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###validateNameStd
<font color = #5f5f5f size = 3pt>
<i>
For any input - string/PyNode/MnsNameStd - Validate it and attempt to convert it into a MnsNameStd Object. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>validateNameStd(objectA)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>MnsNameStd</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>objectA</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###writeJson
<font color = #5f5f5f size = 3pt>
<i>
Write the input data into the input json file path. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>writeJson(directory, fileName, data = {}, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>directory</b></li>
<li><b>fileName</b></li>
<li><b>data</b>(<i>dict</i>) ; [default: {}]</li>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###zeroJointOrient
<font color = #5f5f5f size = 3pt>
<i>
Zero all jointOrient attributes for the jnt hirerchy to rotations. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>zeroJointOrient(topNode = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>topNode</b>(<i>str</i>) ; [default: None]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###zeroTransforms
<font color = #5f5f5f size = 3pt>
<i>
Zero all available transforms for the given object passed in. <br>
</i>
<br>
</font>
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>zeroTransforms(transform = "")</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>bool</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>transform</b>(<i>str</i>) ; [default: ""]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
