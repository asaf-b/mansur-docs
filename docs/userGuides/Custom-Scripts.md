####General
Mansur-Rig contains the ability to append Python-scripts to it's automated process.  
You can easily add custom Python scripts to Mansur-Rig's process in 4 key stages:
<ol>
	<li>Pre-Construction- The script will be run just before the rig construction is initiated.</li>
	<li>Post-Construction - The script will be run after the construction is finished.</li>
	<li>Pre-Deconstruction - The script will bb run before the rig is deconstructed.</li>
	<li>Post-Deconstruction- The script will be run after deconstruction is finished.</li>
</ol>
<br>
<br>
Inserting custom scripts into any Block-Rig is very easy, follow the guide below.

###User-Guide
<ol>
	<li>
		First, open your Block-Rig's Rig-Settings by selecting your Rig-Top, and clicking the <i>Module/Rig Settings</i> in Block-Builder.
		<figure>
		  <img src="../userGuidesImages/customScripts/rigSettings.png"/>
		  <figcaption>Rig-Settings Button</figcaption>
		</figure>
	</li>
	<li>
		Then move to the <i>Custom-Scripts</i> Tab in the Rig-Settings dialog.
		<figure>
		  <img src="../userGuidesImages/customScripts/customScriptsInit.png"/>
		  <figcaption>Custom-Scripts Tab</figcaption>
		</figure>
	</li>
	<li>
		Then open the dropdown menu for the stage you want to add a custom-script to (you can add as many as you want, and at any combination of stages you choose.)
		<figure>
		  <img src="../userGuidesImages/customScripts/customScriptsOpenDD.png"/>
		  <figcaption>Custom-Scripts Open Drop-Down Menu</figcaption>
		</figure>
	</li>
	<li>
		Then simply use the dialog options to add/remove custom scripts paths into the list.
		<br><br>
		<b>Note:</b> the checkbox above the list named <i>execPostCustruct</i>.<br>
		This checkbox is there for your convenience, in order to choose whether to execute the stage's cutom scripts inserted, or not.<br>
		Notice this checkbox is <i>OFF</i> by default, make sure you turn it <i>ON</i> in order to execute this stage's inserted custom-scripts.
	</li>
	<li>
		Use the <i>+</i> button to choose a script path.<br>
		In the opened dialog, navigate to your script path, and choose <i>Open</i><br>
		The path will be added to the dialog's list.
		<figure>
		  <img src="../userGuidesImages/customScripts/customScriptsaddedScript.png"/>
		  <figcaption>Added Script</figcaption>
		</figure>
		<br>
		<b>Note:</b> For ease of use, in case the path selected is within Maya's current <i>Project-Set</i> directory, a message dialog will be displayed, asking you wether you want to convert the selected path to a <i>Relative-Path</i>. In case you do so, the path will be converted to a relative path from your <i>Project-Set</i> directory onwards. That will mean that if any other artists opens this rig (in a team environment for example) opens this rig and sets his Maya-Project correctly, the script will be found regardless. Use this feature in case it fits your needs. 
		<figure>
		  <img src="../userGuidesImages/customScripts/relativeConvertDialog.png"/>
		  <figcaption>Relative path convertion dialog</figcaption>
		</figure>
	</li>
	<li>
		Then simply check the <i>execPostCunstruct</i> to indicate you want to run your custom-scripts, and click <i>Update-Settings</i> at the bottom of the dialog.
		<figure>
		  <img src="../userGuidesImages/customScripts/execChecked.png"/>
		  <figcaption>Execute checkbox</figcaption>
		</figure>
	</li>
	<li>
		Now once you construct/deconstruct your rig, the custom-scripts will be executed based on the stage you choose to insert them.<br>
		You can add as many as you want, and at any stage, in any combination.
	</li>
</ol>



