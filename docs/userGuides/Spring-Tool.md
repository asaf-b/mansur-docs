In Mansur-Rig, springs are extremely easy to create. Using this tool, you'll be able to control spring values comfortably while animating.
<br>
This guide will cover the entire tool and how to use it.
<br>
<hr>

###Spring Tool Load
<figure>
  <img src="../userGuidesImages/springTool/springToolMenu.png"/>
  <figcaption>Spring Tool Menu Item</figcaption>
</figure>
<hr>

###How to use
The spring tool is quite intuative, but if ever you get confused, here are a few guidelines.
<br>
<figure>
  <img src="../userGuidesImages/springTool/springToolLegend.png"/>
  <figcaption>Spring Tool Legend</figcaption>
</figure>
<br>
<ol>
  <li><b><i>Rig List</b></i> - The tool is being initalized everytime you open it. When it is initialized, it first looks for any Block-Rigs that exist within the scene (referenced or not). The found rigs will be listed at the <i>puppet</i> combo box at the top of the UI.</li>
  <li><b><i>Spring Nodes List</b></i> - Once a rig is selected from the list, a list of spring nodes associated with the selected rig will be displayed. You can select multiple items, the edit section will be updated according to the selection. In case you have multiple nodes selected, remember that edits within the UI will affect all selected nodes.</li>
  <li><b><i>Display</b></i> - Use these view filters to display only the nodes you need.</li>
  <li><b><i>Auto-Symmetry</b></i> - When this checkbox is selected, the tool will attempt to find a symmetrical spring node within the rig, and match all attribute changes to it as well, automatically. If a symmetrical node is found, it is painted light-green within the list above.</li>
  <li><b><i>Common Attributes</b></i> - This edit section is the common attributes. These attributes exists for all spring node types. Any changes made will affect all selected nodes.</li>
  <li><b><i>Specific Attributes</b></i> - This edit section is the updated based on the selected node(s) type(s). Based on the type(s) selected, an edit UI will be displayed. Any changes made will affect all selected nodes.</li>
</ol>