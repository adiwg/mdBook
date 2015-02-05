# Viewer

##Purpose
The mdJSON Schema Viewer is an interactive documenatation tool for the ADIwg JSON standard.

##Viewer Interface
The Viewer interface consists of a graphic hierarchial tree structure that visually portrays ADIwg JSON schema elements and the relationships between elements. Each element is represented as a node within the tree. Nodes are connected visually in a parent-child form. Some nodes are containers for sub-elements, each also being represented as a node. Container nodes can be expanded or collapsed by clicking on the node, relative to the user's desire for more or less detail.

The approach is to not overwhelm the user with the full complexity of the ADIwg JSON schema content. Instead, allow the user to pick what elements are of interest, and choose the degree of detail pertaining to those elements.

###Viewer Buttons

+ text button = Access to information panel (See Information panel topic)
+ "Validator" = Access to mdJSON Validator tool
+ "Translator" = Access to mdTranslator tool
+ "+" button = Zoom in
+ "-" button = Zoom out
+ rotating arrow button = Reset; restores default view
+ "i" = Access to help panel

###Viewer Functions

####Pan
By holding down the left mouse button and simultaneously dragging the mouse will pan the Viewer, exposing more area in the opposite direction of the drag.

####Direct Access to a Node
The web link for direct access to a given node can be accessed and copied. To enable this feature, follow these steps:
+ Expand the node in question
+ Click on the node name
+ Notice the JSON pathname to the node is visible at the bottom of the screen, click on the pathname hyperlink
+ A popup will entire with the full web link displayed
+ Copy the link and save to browser

##Nodes
Nodes are JSON schema elements and are graphically represented in the Viewer as circles, interconnected with lines portraying hierarchial relationship. One navigates this hierarchy to discover elements and their inter-relationship.

###Node Symbology
+ open circle = Indicates the node is in an expanded view, exposing the sub-elements contained within that element
+ closed circle = Indicates the node is in a collapsed view, implying sub-elements can be discovered by expanding it
+ (node name)* = Indicator the element is required by the ADIwg JSON schema
+ (node name){} = Object indicator implying the element is comoposed of multiple sub-elements
+ (node name)[] = Array indicator implying the element is composed of repeating sets of sub-elements
+ (*node name* - grayed out) = Indicator of an abstract property, an internal element to the schema, which cannot be accessed in the viewer

###Node Functions

####Expand Node
Clicking on a closed circle will exapnd the tree to portray the sub-elements.

####Collapse Node
This is a toggle function to Expanding a node. Clicking on an open circle node will collapse the tree, if it is an expanded node. If the node is not expandable (contains no sub-elements) then no expansion occurs and the node is centered in the Viewer window.

####Node Description
Clicking on a node name will display the Information panel, providing acces

##Information
The Information panel provides descriptive documentation relative to a selected element node in the Schema Viewer. The panel has three modal tabs at the top, and a text viewer below.

### Definition Tab
This tab indicates the type of object the selected element is, and a definition for the selected element. If the element is mappable to known metadata standard elements, than that mapping is shown under the Translation heading.

### Example Tab
This tab provides examples of using the selected element. Note that the example is in relation to the hierarchial context in which the element was accessed. Clicking on the "Open in new window" button will bring the full example text up in a new browser window, handy for large example descriptions.

### Schema Tab
This tab provides a view of the ADIwg JSON for the selected element. Note that the example is in relation to the hierarchial context in which the element was accessed. Clicking on the "Open in new window" button will bring the full example text up in a new browser window, handy for large schema descriptions.
