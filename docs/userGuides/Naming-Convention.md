<b><i>Mansur-Rig</i></b> is following strict naming convention rules. These rules are followed throught the toolset and in most cases the provided tools will handle the names so you won't have to.
<br>
The naming convention format is as follows (components seperated by an underscore):
<br>
<table border = 1>
	<tr>
		<td><b>Component</b></td>
		<td><b>Valid Examples</b></td>
		<td><b>Comments</b></td>
		<td><b>Constructed Name</b></td>
	</tr>
	<tr>
		<td>Side</td>
		<td>c, l, r</td>
		<td>Lower case. Only the three listed components are valid.</td>
		<td><i>l\_</i> ...</td>
	</tr>
	<tr>
		<td>Body</td>
		<td>arm, spine, frontHair, indexFinger</td>
		<td>ANY camel-cased name is valid.</td>
		<td><i>l\_arm\_</i> ...</td>
	</tr>
	<tr>
		<td>Alpha ID</td>
		<td>A, F, KB, DAC, G</td>
		<td>All upper case, base 26, up to 3 letters.</td>
		<td><i>l\_arm\_A</i> ...</td>
	</tr>
	<tr>
		<td>Component ID</td>
		<td>001, 039, 014, 005, 147</td>
		<td>Integer index, represneted in 3 numbers. This component isn't seperated</td>
		<td><i>l\_arm\_A001</i> ...</td>
	</tr>
	<tr>
		<td>Suffix</td>
		<td>ctrl, grp, plg, blkRig</td>
		<td>This suffix represents the type of object.</td>
		<td><i><b>l\_arm\_A001\_ctrl</b></i></td>
	</tr>
</table>