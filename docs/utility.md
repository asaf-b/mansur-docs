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
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>addBlockClasIDToObj(objectA, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
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
###checkFunctionRedundencyForPackage
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
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>checkIfObjExistsAndSet(**kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>PyNode if valid, None if not. </td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>**kwargs</b></li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
<td><ul>
<li><b>obj</b>(<i>str</i>) - object to act on and return</li>
</ul></td>
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
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>createOffsetGroup(transformObject, **kwargs)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
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
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>distBetween(transformA = None, transformB = None)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
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
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getNumLinesForDir(directory = "D/mansurProject/mansur")</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>directory</b>(<i>str</i>) ; [default: "D:/mansurProject/mansur"]</li>
</ul></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###getSideFromNode
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getSideFromNode(node)</td></tr>
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
###getTopParentForObj
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getTopParentForObj(obj)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
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
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>getTopParentForSel()</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
</tr>
<tr width=150px><td><b><font color = #4caf50>Keyword Arguments:  </font></b></td>
</tr>
</table></font>
<hr width = 100%>
###importModuleFromPath
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>importModuleFromPath(path)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
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
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>readJson(fullPath)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
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
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>readSetteingFromFile(settingsPath)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
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
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>returnIndexFromSideDict(dict, searchElement)</td></tr>
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
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>sortNameStdArrayByID(nameStdArray)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
<tr><td><b><font color = #4caf50>Arguments:  </font></b></td>
<td><ul>
<li><b>nameStdArray</b></li>
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
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>splitEnumAttrToChannelControlList(enumAttrName, node)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
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
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
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
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>splitEnumToStringList(enumAttrName, node)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
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
###validateNameStd
<font size = 3pt>
<table>
<tr><td><b><font color = #4caf50>Constructor:  </font></b></td><td>validateNameStd(objectA)</td></tr>
<tr><td><b><font color = #4caf50>Return:  </font></b></td><td>None</td></tr>
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
