<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDocumentSpecification.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IDocumentSpecification Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDocumentSpecification_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IDocumentSpecification Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Allows you to specify how to open a model document. Use this interface's properties before calling [ISldWorks::OpenDoc7](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~OpenDoc7.html) to specify how you want to open a model document.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface IDocumentSpecification ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDocumentSpecification ``` | |

| C# |  |
| --- | --- |
| ``` public interface IDocumentSpecification ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IDocumentSpecification ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DocumentSpecification.

# ![](dotnetimages/collapse.gif)Example

See the [IPLMObjectSpecification](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPLMObjectSpecification.html) examples.

# ![](dotnetimages/collapse.gif)Example

[Hide All Edges in Drawing View (VBA)](Hide_All_Edges_in_Drawing_View_Example_VB.htm)

[Open Drawing Document Read-only (VBA)](Open_Drawing_Document_Read-only_Example_VB.htm)

[Get Whether Components Are Loaded (C#)](Get_Whether_Components_Are_Loaded_Example_CSharp.htm)

[Get Whether Components Are Loaded (VB.NET)](Get_Whether_Components_Are_Loaded_Example_VBNET.htm)

[Get Whether Components Are Loaded (VBA)](Get_Whether_Components_Are_Loaded_Example_VB.htm)

[Open Assembly Document (C#)](Open_Assembly_Document_Example_CSharp.htm)

[Open Assembly Document (VB.NET)](Open_Assembly_Document_Example_VBNET.htm)

[Open Assembly Document (VBA)](Open_Assembly_Document_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

The following properties are not valid when opening a 3DEXPERIENCE file using SOLIDWORKS Connected:

* [IDocumentSpecification::FileName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDocumentSpecification~FileName.html)* [IDocumentSpecification::ConfigurationName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDocumentSpecification~ConfigurationName.html)* [IDocumentSpecification::DocumentType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDocumentSpecification~DocumentType.html)* [IDocumentSpecification::DisplayState](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDocumentSpecification~DisplayState.html)* [IDocumentSpecification::InteractiveAdvancedOpen](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDocumentSpecification~InteractiveAdvancedOpen.html)* [IDocumentSpecification::InteractiveComponentSelection](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDocumentSpecification~InteractiveComponentSelection.html)* [IDocumentSpecification::LoadExternalReferencesInMemory](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDocumentSpecification~LoadExternalReferencesInMemory.html)

# ![](dotnetimages/collapse.gif)Accessors

[ISldWorks::GetOpenDocSpec](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~GetOpenDocSpec.html)

# ![](dotnetimages/collapse.gif)Access Diagram

[DocumentSpecification](SWObjectModel.pdf#DocumentSpecification)

# ![](dotnetimages/collapse.gif)See Also

####

[IDocumentSpecification Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDocumentSpecification_members.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)

[ISldWorks::OpenDoc6 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~OpenDoc6.html)