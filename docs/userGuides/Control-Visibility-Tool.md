###General
This simple tool was written to improve accesibility to Block rigs' controllers.<br>
Using this tool you can easily manipulate the visibility of any module visibility within your rigs, helping de-clutter rigs at different stages of animation.
Also, Block rigs are devided into main structure groups- control the visibility state of each group easily within the <i>Rig-Top</i> tab.

####UI
Access this Tool via Mansur-Rig main Maya menu
<figure>
  <img src="../userGuidesImages/controlVisibilityTool/controlVisMenuItem.png"/>
  <figcaption>Menu Entry</figcaption>
</figure>

<figure>
  <img src="../userGuidesImages/controlVisibilityTool/uiInit.png"/>
  <figcaption>UI</figcaption>
</figure>

### User Guide

#### For Rigging- in deconstructed state

<ul>
	<li>
		In deconstructed state, this tool's <i>Body</i> and <i>Facial</i> tabs will be empty, since there are no controls present.
	</li>
	<li>
		But you can still use the <i>Rig-Top</i> tab.
		<figure>
		  <img src="../userGuidesImages/controlVisibilityTool/rigTopTab.png"/>
		  <figcaption>Rig-Top Tab</figcaption>
		</figure>
	</li>
	<li>
		This tab contains all primary sub-groups for the selected Block-Rig.
		Use this UI to easily change the visibility state for each group.
	</li>
	<li>
		Use the first button column to control the group's visibility (True/False)
	</li>
	<li>
		Use the second button column to control the group's readability state (Normal/Template/Reference)
	</li>
</ul>

<br>

#### For Animation- in constructed state
<ul>
	<li>
		In constructed state, this tool's <i>Body</i> and <i>Facial</i> will be be filled with all contrsucted modules. One row for each module. The modules will be split into the two tabs based on their <i>isFacial</i> setting set within Block.
		<figure>
		  <img src="../userGuidesImages/controlVisibilityTool/animState.png"/>
		  <figcaption>Body & Facial Tabs</figcaption>
		</figure>
		<br>
		<figure>
		  <img src="../userGuidesImages/controlVisibilityTool/allOn.png"/>
		  <figcaption>Body & Facial All ON</figcaption>
		</figure>
	</li>
	<li>
		Now using the *Filter* field, you can filter the modules within the UI to turn ON/OFF visibility for the modules related controls.
	</li>
	<li>
		For exmaple, you can turn ALL modules off using the top *ALL* row buttons:
		<figure>
		  <img src="../userGuidesImages/controlVisibilityTool/filteringAllOff.png"/>
		  <figcaption>Visibility filtering- All Off</figcaption>
		</figure>
		<br>
		then filter by *arm*, and turn the arm modules ON- which will result in this:
		<figure>
		  <img src="../userGuidesImages/controlVisibilityTool/filteringArm.png"/>
		  <figcaption>Visibility arm filtering</figcaption>
		</figure>
	</li>
	<li>
		Another example is turning all *Body* modules ON, and turning all *Facial* modules OFF
		<figure>
		  <img src="../userGuidesImages/controlVisibilityTool/bodyOnly.png"/>
		  <figcaption>Body modules ON, facial modules OFF</figcaption>
		</figure>
</ul>