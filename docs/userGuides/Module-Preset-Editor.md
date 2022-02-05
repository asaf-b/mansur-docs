###User-Guide
This tool was designed to manage module presets.
<br>
As Mansur-Rig modules comatin many attrbiutes, it is sometimes more convenient to use a predefined preset to speed up the wrokflow.
<br>
Mansur-Rig includes some module presets, although this was designed mainly to allow usesrs to create their own presets, essentially saving the module settings' state in order to re-use later.
<br>

!!! Important Note
    Module preset actions are only relevant to the <i>Module Settings</i> tab within the module settings window.
    All common attributes (first tab) will be ignored.

####UI
Access this Tool via the "Preset Editor" button within any module settings window.

<figure>
  <img src="../userGuidesImages/modulePresetEditor/accessMPE.png"/>
  <figcaption>Tool Load Button</figcaption>
</figure>

<figure>
  <img src="../userGuidesImages/modulePresetEditor/MPEWindow.png"/>
  <figcaption>Module Preset Editor Dialog</figcaption>
</figure>

####Preferences setup
In case you want to use custom-presets, it is recomended to setup a local folder which you want to save your presets in, and add the path to Mansur-Rig's module preset paths variable.
<br>
At deafult, the tool will list presets within the UI only out of Mansur-Rig predefined preset folder <i><$MNS_INSTALL_PATH>/scripts/mansur/block/modulePresetEditor/mnsModulePresets </i>
<br>
Since the system has no way of knowing where to find additional custom presets, you need to tell the system where to look.
<br>
The process is very easy:
<br>
<ol>
  <li>Open <i>Block Builder</i> from Mansur's main menu.</li>
  <li>Move to <i>Utility</i> tab.</li>
  <li>Open the <i>Module Presets Paths</i> dropdown menu.</li>
  <li>Press the <i>Add Path (+)</i> button</li>
  <li>Navigate to the custom directory you want to add and click <i>Select-Folder</i></li>
  <li>The directory will be added to the main preset directories list.</li>
  <li>Click <i>Apply</i>.</li>
</ol>
The path you selected is now added into Mansur-Rig's preferences as a variable, and once you reload <i>Module Presets Editor</i>, presets you saved within this folder will be listed in the UI.
<br>
You will not need to repeat this step when restarting Block, nor when restarting Maya, this prefernce will be saved locally within Mansur-Rig's preferences folder.
<br>
You can add as many paths as you require.
<br>
Also, you can always go back to this dropdown menu to edit your custom preset paths.
<br><br>
<figure>
  <img src="../userGuidesImages/modulePresetEditor/customPathVars.png"/>
  <figcaption>Custom Presets Paths UI</figcaption>
</figure>

####Export Workflow
<ol>
  <li>Edit your module settings to best represent your preset.</li>
  <li>Open the module preset editor.</li>
  <li>Click <i>Export</i>.</li>
  <li>Input required information in the prompted dialog (Author, Preset Description).</li>
  <li>Press <i>Export</i> in the dialog.</li>
  <li>Chose the file name and the location where you ant to save it.</li>
  <li>Your new preset is now saved and ready to be re-used.</li>
</ol>
<br>
####Import Workflow
<ol>
  <li>Open any module's settings.</li>
  <li>Open the module preset editor.</li>
  <li>It is recommended to follow <i>Preferences Setup</i> guide above to load custom presets folders information into the UI.</li>
  <li>Select the preset you want to use.</li>
  <li>Click <i>Load</i> button.</li>
  <li>The settings window will now consist of all data saved in your selected preset.</li>
  <li>To finalize, click <i>Update Settings</i> in the module settings window to apply your changes.</li>
  <li>Alternatively, if your preset isn't found in the UI, you can manually load it from file using the <i>Import</i> button.</li>
</ol>
<br>
####Legend
<figure>
  <img src="../userGuidesImages/modulePresetEditor/presetEditorLegend.png"/>
  <figcaption>Module Preset Editor Legend</figcaption>
</figure>

<ol>
  <li>
    <b><i>Available Presets</b></i>- All available presets, within all Module Presets Paths. Only relevant module preset types will be displayed. Meaning that if you loaded the preset editor from an <i>FKChain</i> type module settings window, only presets saved for <i>FKChain</i> type module will be displayed.
  </li>
  <li>
    <b><i>Preset Author and Description</b></i>- Information about the current selected module preset.
  </li>
  <li>
    <b><i>Load</b></i>- Update the module settings window with the currently selected preset.
  </li>
  <li>
    <b><i>Import</b></i>- Import module preset from a file.
  </li>
  <li>
    <b><i>Export</b></i>- Export the current module settings values into a module preset file.
  </li>
  <li>
    <b><i>Close</b></i>- Close Dialog.
  </li>
</ol>

