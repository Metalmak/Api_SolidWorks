<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRenamedDocumentReferences~UpdateWhereUsedReferences.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| UpdateWhereUsedReferences Property (IRenamedDocumentReferences) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IRenamedDocumentReferences Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRenamedDocumentReferences.html) : UpdateWhereUsedReferences Property (IRenamedDocumentReferences) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets whether to update the references to the new file name.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property UpdateWhereUsedReferences As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IRenamedDocumentReferences Dim value As System.Boolean   instance.UpdateWhereUsedReferences = value   value = instance.UpdateWhereUsedReferences ``` | |

| C# |  |
| --- | --- |
| ``` System.bool UpdateWhereUsedReferences {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool UpdateWhereUsedReferences {    System.bool get();    void set ( &   System.bool value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

True to update the references to the new file name, false to continue to reference the old file name

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See RenamedDocumentReferences::UpdateWhereUsedReferences.

# ![](dotnetimages/collapse.gif)Example

[Rename Component and Update References (C#)](Rename_Component_and_Update_References_Example_CSharp.htm)

[Rename Component and Update References (VB.NET)](Rename_Component_and_Update_References_Example_VBNET.htm)

[Rename Component and Update References (VBA)](Rename_Component_and_Update_References_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IRenamedDocumentReferences Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRenamedDocumentReferences.html)

[IRenamedDocumentReferences Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRenamedDocumentReferences_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2016 FCS, Revision Number 24.0