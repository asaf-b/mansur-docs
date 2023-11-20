#### General
Believe it or not, this is one of the very firsts tool to be developed within Mansur-Rig, and many UI behaviours are based on it.  
It is an extremely powerful tool, despite it's simplicity.  
<br>
This simple UI, hides great strengths.
On initialization, this tool will list **ALL** methods within Mansur-Rig's entire Python library.  
Then, when you choose to *Create-UI*- a simple UI will be created for the method selected.  
This means, that you can run **ANY** of Mansur-Rig's methods, using a UI, instead of calling it through code.  
This tool will live-examine the method you select, acquiring all arguments as well as all keyword-argumets, including all of their settings, and compile them into a simple UI for you to be able to use without even touching code.  
In this guide I'm going to show you how to harness this tool's strengths to your advanatage.  

#### UI
<figure>
  <img src="../userGuidesImages/dynUI/dynUIMenu.png"/>
  <figcaption>Menu Entry</figcaption>
</figure>

<figure>
  <img src="../userGuidesImages/dynUI/UI.png"/>
  <figcaption>UI</figcaption>
</figure>

#### Legend
1. Methods list
2. *Create UI* button- will create a simplified UI for the selected method. Use *Mouse-Double-Click* on a method as a shortcut.
3. Fliter/Search Section
	* Filter methods by entering text into the search field.
	* *A* Checkbox - will determine whether the search is case-sensative or not.
	* *Clear* button will clear the serach field and reset the list.
4. *Pin/Unpin*- Toggle methods betwen pinned and unpinned options. Use *Mouse-Right-Click* on a method as a shortcut.
	*Pinning a method is equivalent to *Saving-To-Favorites*. Whenever you pin a method on the list, it will be marked in bold font, and moved to the top of the list. Use this feature to save your most used methods instead of needing to search them every time you load the tool. Pinned methods will be saved as a global preference, and will be restored when you restart the tool or restart Maya.
	*Un-Pinning a method will remove it from your pinned methods.
	*Use *Clear All Pins* button to clear all of your pinned methods and reset the tool to it's default state.
5. *Reload Library*- Use this method in case you are a developer, and you are making live changes to methods, and want to reload your changes.
6. Toggle between *Pinned Only View* and default. In *Pinned Only View* only pinned methods will be displayed in the methods list.

#### User Guide