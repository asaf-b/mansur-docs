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
The best way to explain how to use this tool is by examples:

##### Example 1- create-offset-group 
Let's say that you are happy with your Block rig, but for some pipeline requirements you need to create an additional offset-group for one of the contorls.  
This tool is the easiest way to do that.    
Here is what you do:  

1. Load the *Dynamic UI Creator* from Mansur-Rig's main menu.
2. In the search field, type- *createOffset*. This will filter all methods with this text in it.
	<figure>
	  <img src="../userGuidesImages/dynUI/createOffsetFilter.png"/>
	  <figcaption>*createOffset* Filter</figcaption>
	</figure>
3. In the filtered results, you can see there is a method named *createOffsetGroup* which looks like what we are looking for.  
4. Now you could simply try and see if that works, but even better is to take a look at this method's documentation.
5. In order to do that, oepn a browser and go to the [*Code-Documentation*](../Maya-Plugins.md) section in Mansur-Rig's docs page.
6. If you know where this method is located within the Python library, you can simply navigate to it, but this is most likely not the case.
7. So in top-right-hand side you'll see a search bar- simply type the name of the method into it -*createOffsetGroup*, and click search.
	<figure>
	  <img src="../userGuidesImages/dynUI/docsSearchBar.png"/>
	  <figcaption>Documentation page search bar</figcaption>
	</figure>
8. There you can simply find the documentation for the given method:
	<figure>
	  <img src="../userGuidesImages/dynUI/createOffsetSearch.png"/>
	  <figcaption>Method's Documentation Search</figcaption>
	</figure>
9. Now click the method's link to navigate directly to [it's documentation](../utility.md#createoffsetgroup)
	<figure>
	  <img src="../userGuidesImages/dynUI/createOffsetDocs.png"/>
	  <figcaption>Method's Documentation</figcaption>
	</figure>
10. Reading the description of the documentation it is clear this is the method we are looking for. You can also see all arguments and keyword argumets definitions within. For this specific case we see a single *argument*:
	- transformObject 
	
	and 2 *keyword argumets*: 
		
	- type
	- bodySuffix

11. Going back to Maya, click the *Create UI* button while the method is selected, or double click the method to initiate the UI.
12. Now we see a UI representing the method, with a row for every argument and keyword argument for this method:
	<figure>
	  <img src="../userGuidesImages/dynUI/createOffsetUI.png"/>
	  <figcaption>Method's UI</figcaption>
	</figure>
13. The UI correlates directly to the method's documentation, and is being dynamically created after fetching the method's informaion directly from the Python library. Also, each row within the UI is being created based on the value type for each argument.
14. Now let finallly test it out:
	- Select one of your Block-Rig's controls, and click the *<* button next to the *transformObject* argument row, to insert it into the UI 
		<figure>
		  <img src="../userGuidesImages/dynUI/offsetCtrlLoad.png"/>
		  <figcaption>Ctrl Load</figcaption>
		</figure>
	- Click *Run* button- And this is the result. An offset group was created for the target control.
	<figure>
		  <img src="../userGuidesImages/dynUI/offsetResult.png"/>
		  <figcaption>Result</figcaption>
	</figure>
15. This will be equivalent to doing this using Python:
	```
	from mansur.core import utility as mnsUtils  
	mnsUtils.createOffsetGroup("c_freeControl_A001_ctrl")
	```
16. You can also expand this, once you tested the behavior manually, to automate this process using the [*Custom-Scripts user guide*](Custom-Scripts.md)
17. This is the simplest way to explain how this tool works. In general, this tool will generate a UI for every single method within Mansur-Rig's custom Python library, which is HUGE. You can use this tool to enhece your rigging process, learn how the code works, experiment, and testing manually before automating.
18. Also, you can of course look for methods within Mansur-Rig's [*Documentation Page*](../Maya-Plugins.md) and then test it out using this *Dynamic-UI* tool.

##### Example 2- mnsAnnotateNode
Now lets try a differt example, where you need to create a node, whether one from Mansur-Rig's custom plugin library, or a native Maya node, easily without dealing with code or node-connections.  
In this example, we will be ceating a simple mnsAnnotate node.  

1. Lets start by assuming you watch this [*mnsAnnotate Node*](https://www.youtube.com/watch?v=k6KQ4HGIoYc) You-Tube video, and you would like to to try it out yourself. The easiest way to do that would be to use this Dynamic-UI tool.
2. Once again open the Dynamic-UI tool and type mnsAnnotate within the search bar
	<figure>
		  <img src="../userGuidesImages/dynUI/annotateSearch.png"/>
		  <figcaption>mnsAnnotate Search</figcaption>
	</figure>
3. Once you found the relevant method, double click it to load the UI.
4. Let's compare again against the [*Method's Documentation*](../nodes.md#mnsannotatenode)
	<figure>
		  <img src="../userGuidesImages/dynUI/mnsAnnotateUI.png"/>
		  <figcaption>mnsAnnotate UI</figcaption>
	</figure>
5. Once again we see a direct correlation between the method's definition and UI created, as well as all arguments represnted, based on their type, within the UI.
6. After reading the [*Method's Documentation*](../nodes.md#mnsannotatenode) and seeing the [*Video*](https://www.youtube.com/watch?v=k6KQ4HGIoYc) it is clear the most important argument is the *Attributes* argument, which is the list of attributes you want to annotate.
7. So now make a channel-box selection of the attributes you would like to annotate:
	<figure>
		  <img src="../userGuidesImages/dynUI/annotateCBSelection.png"/>
		  <figcaption>Channel-Box Selection</figcaption>
	</figure>
8. Now click the *<* button to the right of the *Attributes* argument row, to input your selection into the UI:
	<figure>
		  <img src="../userGuidesImages/dynUI/CBInsert.png"/>
		  <figcaption>Channel-Box Attributes Inserted</figcaption>
	</figure>
9. Click *Run* button.
10. And as easily as that, a mnsAnnotate node was created, as requested, with all connections made automatically, to the requested attribues.
	<figure>
		  <img src="../userGuidesImages/dynUI/mnsAnnotateResult.png"/>
		  <figcaption>Result</figcaption>
	</figure>
11. Once again this will be equivalent to this Python code:
	```
	from mansur.core import nodes as mnsNodes
	mnsNodes.mnsAnnotateNode(attributes = ["locator1.tx", "locator1.ty", "locator1.tz"])
	```
