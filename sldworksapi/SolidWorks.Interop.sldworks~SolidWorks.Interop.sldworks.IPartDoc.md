<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IPartDoc Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IPartDoc Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Provides access to functions that perform operations on parts in part documents.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface IPartDoc ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPartDoc ``` | |

| C# |  |
| --- | --- |
| ``` public interface IPartDoc ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IPartDoc ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PartDoc.

# ![](dotnetimages/collapse.gif)Example

[Get Sketches (C++)](Get_Sketches_Example_CPlusPlus_COM.htm)

[Traverse Bodies (C++)](Traverse_Bodies_Example_CPlusPlusCLI.htm)

[Create Imported Surface Body From Sketch (C#)](Create_Imported_Surface_Body_from_Sketch_Example_CSharp.htm)

[Get Differences Between Parts (VBA)](Get_Differences_Between_Parts_Example_VB.htm)

[Import Step File (C#)](Import_STEP_File_Example_CSharp.htm)

[Import Step File (VB.NET)](Import_STEP_File_Example_VBNET.htm)

[Import Step File (VBA)](Import_STEP_File_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This interface provides functions that allow you to:

* create bodies and features.* perform suppress operations.

    * obtain part extents and tessellation.

      * locate entities by name.

The SOLIDWORKS API also has functions that are common to all document types. For example, determining the file name associated with a document would be a common operation. To expose common document-level functions, the SOLIDWORKS API uses the [IModelDoc2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2.html) object.

Events are implemented with delegates in the Microsoft .NET Framework. See the [Overview](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks_namespace.html) topic for a list of delegates for this interface.

# ![](dotnetimages/collapse.gif)Accessors

[IBeltChainFeatureData::AccessBeltPart](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBeltChainFeatureData~AccessBeltPart.html)

# ![](dotnetimages/collapse.gif)Access Diagram

[PartDoc](SWObjectModel.pdf#PartDoc)

# ![](dotnetimages/collapse.gif)See Also

####

[IPartDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc_members.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)