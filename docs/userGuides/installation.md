* Download the latest release of Mansur-Rig from <a href = "https://github.com/asaf-b/Mansur-Rig/releases" target = "_blank">Git-Hub</a>.
* Extract the .zip library to your preferred location.
   * If you have another version already installed, preferably extract to the same location (version root folder should be placed in the same root folder of the previous version) 
   * .../ANY_DIRECTORY
      * .../ANY_DIRECTORY/mansurRig_1.0.1
      * .../ANY_DIRECTORY/mansurRig_1.0.2
      * .../ANY_DIRECTORY/mansurRig_1.0.3
* Go into the main version directory
* Drag and Drop the "mansurRig_DragAndDrop_install.mel" into any supported Maya version
* Follow the prompt instructions
* Restart Maya

!!!Updates
	Please make sure to update as appropriate. <a href="../Version-Updates/" class="md-nav__link"><b> Version Updates Guide </b></a>

##Manual Installation
* Download and extract Mansur-Rig as described above. 
* For the target Maya version, locate "Maya.env" file. For example (On Windows): "C:\Users\xxx\Documents\maya\2022\Maya.env"
* Open the file for editting using any text editor software (e.g. Notepad)
* Insert the following variable, changing the directory to your Mansur-Rig extracted version location:
MAYA_MODULE_PATH = D:\mansurRig\mansurRig_1.3.6

##Uninstallation
* Locate any installation directory of Mansur-Rig in your file system
* Go into the main version (any version) directory
* Drag and Drop the "mansurRig_DragAndDrop_UNINSTALL.mel" into any supported Maya version
* Follow the prompt instructions
* Restart Maya


## Linux Notes
* As opposed to the Windows installer, the Linux version will install Mansur-Rig on the choosen maya version only. 
* The Linux installer is using the local Maya.env file to append the new envioronment variable instead of installing a system-wide persistant variable, as the installer can not assume system write permissions.
* In case you want to install Mansur-Rig on multiple versions of Maya, please repeat the installation (drag-drop) on every required Maya version.