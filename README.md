# UnityUIToolkitExtensionsPackage

Additional UI Toolkit Elements and Features.

Custom Elements:
- GradientElement
- TableElement
- RowElement
- DraggableTargetElement

Element Templates:
- Table Info Container

## Installation
To include element templates in the UI Builder, the "Packages\Unity UI Toolkit Extensions\CustomElementTemplates" directory must be copied to your Assets folder after retrieving through the package manager (via git url).

## Examples
There are example scenes found in the Examples folder.  This can be excluded on import.

## Tables
In order for tables to be formatted correctly, a GameObject with the TableElementProcessor component must be added.  Sample data can be generated for a table by adding the SampleTableGenerator component to a GameObject in the scene.

## Drag and Drop
The DraggableTargetElement is a modified version of the Unity UI Toolkit example on drag and drop found here https://docs.unity3d.com/Manual/UIE-create-drag-and-drop-ui.html.  I found that this example had some positioning issues when draggable elements were not positioned in the very top-left corner of their container.

To use, add DraggableTargetElements into your document hierarchy and use as though they were regular visual elements.  Add a class that will be used to restrict which draggables can go to which draggable targets.  Initialize your draggable with the DragAndDropManipulator from any MonoBehaviour.

Known Issues:
- Tables do not display correctly when a document is hidden and displayed
