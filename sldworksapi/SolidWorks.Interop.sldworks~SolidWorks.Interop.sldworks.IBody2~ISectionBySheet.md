<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~ISectionBySheet.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ISectionBySheet Method (IBody2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html) : ISectionBySheet Method (IBody2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Sheet*
:   Pointer to the sheet body used to perform the section

*NumMaxSections*
:   Maximum number of sections to create

*SectionedBodies*
:   Pointer to an array of [bodies](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html) created during the section operation

Sections a body using a sheet (surface) body.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ISectionBySheet( _    ByVal Sheet As Body2, _    ByVal NumMaxSections As System.Integer, _    ByRef SectionedBodies As Body2 _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBody2 Dim Sheet As Body2 Dim NumMaxSections As System.Integer Dim SectionedBodies As Body2 Dim value As System.Integer   value = instance.ISectionBySheet(Sheet, NumMaxSections, SectionedBodies) ``` | |

| C# |  |
| --- | --- |
| ``` System.int ISectionBySheet(     Body2 Sheet,    System.int NumMaxSections,    ref Body2 SectionedBodies ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int ISectionBySheet(  &   Body2^ Sheet, &   System.int NumMaxSections, &   Body2^% SectionedBodies ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Sheet*
:   Pointer to the sheet body used to perform the section

*NumMaxSections*
:   Maximum number of sections to create

*SectionedBodies*
:   Pointer to an array of [bodies](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html) created during the section operation

#### Return Value

Number of bodies created during the operation

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Body2::ISectionBySheet.

# ![](dotnetimages/collapse.gif)Remarks

Before using this method, [make a copy of the body](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~Copy.html) because the sheet body becomes invalid after using this method. COM applications should release all bodies after calling this method.

# ![](dotnetimages/collapse.gif)See Also

####

[IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html)

[IBody2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0