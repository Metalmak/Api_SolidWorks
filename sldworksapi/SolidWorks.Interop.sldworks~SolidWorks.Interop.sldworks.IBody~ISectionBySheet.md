<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody~ISectionBySheet.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ISectionBySheet Method (IBody) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBody Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody.html) : ISectionBySheet Method (IBody) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Sheet*

*NumMaxSections*

*SectionedBodies*

Obsolete. Superseded by [IBody2::ISectionBySheet](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~ISectionBySheet.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ISectionBySheet( _    ByVal Sheet As Body, _    ByVal NumMaxSections As System.Integer, _    ByRef SectionedBodies As Body _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBody Dim Sheet As Body Dim NumMaxSections As System.Integer Dim SectionedBodies As Body Dim value As System.Integer   value = instance.ISectionBySheet(Sheet, NumMaxSections, SectionedBodies) ``` | |

| C# |  |
| --- | --- |
| ``` System.int ISectionBySheet(     Body Sheet,    System.int NumMaxSections,    ref Body SectionedBodies ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int ISectionBySheet(  &   Body^ Sheet, &   System.int NumMaxSections, &   Body^% SectionedBodies ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Sheet*

*NumMaxSections*

*SectionedBodies*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Body::ISectionBySheet.

# ![](dotnetimages/collapse.gif)See Also

####

[IBody Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody.html)

[IBody Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody_members.html)