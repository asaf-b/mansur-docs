There are known issues with using 4K monitors and Maya.  
The problem is a global one, and not related specifically to Mansur-Rig.  
If you are experiencing issues with your 4K monitor, here 2 possible fixes:

#### Solution Fix 1
This fix is a Global fix within Maya's environment, and this guide below is a direct copy of [*This Guide*](https://help.autodesk.com/view/MAYAUL/2023/ENU/?guid=GUID-03BF2E0E-6FB1-438E-A238-3298994CFADB) published by Autodesk.

1. Open the Preferences window (select Windows > Settings/Preferences > Preferences).
2. Select the Interface preferences category, if it's not already selected.
3. Adjust the settings in the Interface Scaling section.
	<figure>
	  <img src="../userGuidesImages/4kMonitors/mayaScale.png"/>
	  <figcaption>Maya Scale</figcaption>
	</figure>
4. Restart Maya

#### Solution Fix 2
**Available from version 2.4.2 onwards.**  
If the above did not help, you can also try Mansur-Rig's attempt to fixing this issue locally.  
Although this fix is not robust, and may only work in some cases.  
Once again this is a global Maya issue and it is very difficult to solve on the local software scope.

1. Open Mansur-Rig's Preferences (Mansur-Rig's Menu -> Preferences)
2. Under global tab, turn *Attempt 4K Monitors Fix* setting ON.
3. Click *Save* at the button of the dialog.
	<figure>
	  <img src="../userGuidesImages/4kMonitors/attemp4KPref.png"/>
	  <figcaption>Mansur-Rig's Preferences</figcaption>
	</figure>
