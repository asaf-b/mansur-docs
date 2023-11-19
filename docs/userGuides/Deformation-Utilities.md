#### General
Mansur-Rig contains skin/deformation tools to enhence your workflow as well as speed it up.  
The toolset is quite simple, although quite important.  
Use this tool-set to Export/Import skin data, Copy skin-data between meshes and Re-Bind skins.  
A few more useful utilities are included which will be covered below.

#### UI
Mansur-Rig's skin/deformation tools are located inside of Block-Builder
Open Block, and move to *Deformation* tab.

<figure>
  <img src="../userGuidesImages/deformationTools/menuEntry.png"/>
  <figcaption>Menu Entry</figcaption>
</figure>

<figure>
  <img src="../userGuidesImages/deformationTools/mainUI.png"/>
  <figcaption>UI Legend</figcaption>
</figure>

#### User Guide

##### Lists Relations
<ol type="A">
	<li> This list is related to Export, Unbind, and Re-Bind Actions.</li>
	<li> This list is the source list for Copy-Skin action.</li>
	<li> This list is the target list for Copy-Skin action.</li>
</ol>

##### Skin Export/Import (#1, #2)
1. Skin Import-
2. Skin Export- 
	* Select/Load(To *A* List) the skinned meshes you want to export skins from, and click *Export Skin*. 
	* In the opened file-dialog, select the path and file name you want to export to, and click *Save*. 
	* The selcted meshes' skin-data will be exported to the selected file as *.mnsSkin* format.

##### Copy Skin (#3)
<ol start="3">
	<li>
		Copy Skin -
		<ul>
			<li>Copy skin-weights from Source-list (**B**) to target-list (**C**), based on the parameters selected:
				<ul>
					<li>Surface Association- The surfaceAssociation flag controls how the weights are transferred between the surfaces: "closestPoint", "rayCast", or "closestComponent".</li>
					<li>Influence Association- The influenceAssociation flag controls how the influences on the source and target skins are matched up. The flag can be included multiple times to specify multiple association schemes that will be invoked one after the other until all influences have been matched up. Supported values are "closestJoint", "closestBone", "label", "name", "oneToOne".</li>
				</ul>
			</li>
			<li>This is a very important and powerful utility, that will allow you to transfer skin data between meshes, reagdless of topology.</li>
			<li>This utility will attempt to transfer skin weights between meshes. For example- transfer skin weights from a body mesh to clothing, transfer skin data from a head mesh to a hair mesh.
			<li>You can transfer from a single source to a single target, multiple sources to a single target, or a single source to multiple targets.</li>
			<li>When choosing to transfer from multiple sources, this action will avarage the source weights based on proximity, to the targets selected.</li>
		</ul>
 	</li>
</ol>

##### Selection (#4, #5)
<ol start="4">
	<li>
		Select Skinning Joints -
		<ul>
			<li>Based on the selected mode (*Module*/*Branch*), all related skinning joints will be selected.</li>
			<li>In Block, not all joints within the heirarchy are designed to be a part of the skin. This utility will select only the ones that are. In case there are only *Main-Joints*- These will be the skinning joint for the module. In case there are *Interpolation-Joints*- the interpulation joints will be the skinning joint for the module, while the *Main-Joints* will not.
		 	<li>This is different then *Delete-History* as it gets the selected meshes back to bind pose before removing their Skin-Clusters.</li>
	 	</ul>
 	</li>
	<li>
		Select Main Joints -
		<ul>
			<li>Based on the selected mode (*Module*/*Branch*), all related main joints will be selected.</li>
			<li>In Block, not all joints within the heirarchy are designed to be a part of the skin. This utility will select only the *Main-Joints* related to the module, regardless if there are *Interpolation-Joints* present or not.</li>
		</ul>
	</li>
</ol>

##### Unbind, Rebind (#6, #7)
<ol start="6">
	<li>
		Unbind -
		<ul>
			<li>Select/Load (To **A** List) the skinned meshes you want to unbind, and click *Unbind*. </li>
		 	<li>This is different then *Delete-History* as it gets the selected meshes back to bind pose before removing their Skin-Clusters.</li>
	 	</ul>
 	</li>
	<li>
		Rebind -
		<ul>
			<li>Select/Load(To **A** List) the skinned meshes you want to rebind, and click *Rebind*.</li>
			<li>This action will simply re-bind the meshes using the current state of their skin-cluster joints. In case you moved a joint for example after you bound your skin, and want to reset the skin data to this position, use this utility.</li>
			<li> This action will restore the meshes' bind pose, with the current skin-data. In essence resetting the skin-cluster to the current state.</li>
		</ul>
	</li>
</ol>

##### Load Buttons (#8)
<ol start="8">
	<li>
		Load Meshes -
		<ul>
			<li>Load the current scene-selected meshes into the relevant list (**A**/**B**/**C**)</li>
		</ul>
 	</li>
</ol>

##### Mirror skin to detached components (#9)
<ol start="9">
	<li>
		Mirror skin to detached components -
		<ul>
			<li>This utility will allow you to mirror skin weights between meshes that are not combined.</li>
			<li>For example, you have a character wearing shoes. The shoes meshes are split to *l_shoe_geo* and *r_shoe_geo* (the meshes are not combined). You skin-painted *l_shoe_geo*, and now you want to transfer the weights to *l_shoe_geo*:
				<ol>
					<li>Load *l_shoe_geo* into the source field (by selecting it, then pressing the *<* button next to the field)</li>
					<li>Load *r_shoe_geo* into the target field (by selecting it, then pressing the *<* button next to the field)</li>
					<li>Click *Mirror skin to detached components* button.</li>
					<li>This action will attempt to mirror the weights from the source to the target, taking into consideration that the influence joints should be mirrored as well.</li>
				</ol>
			</li>
		</ul>
 	</li>
</ol>
