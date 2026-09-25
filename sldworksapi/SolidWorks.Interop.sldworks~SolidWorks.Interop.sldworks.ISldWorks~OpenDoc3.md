<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~OpenDoc3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| OpenDoc3 Method (ISldWorks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : OpenDoc3 Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FileName*

*Type*

*ReadOnly*

*ViewOnly*

*RapidDraft*

*Silent*

*Errors*

Obsolete. Superseded by [ISldWorks::OpenDoc6](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~OpenDoc6.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function OpenDoc3( _    ByVal FileName As System.String, _    ByVal Type As System.Integer, _    ByVal ReadOnly As System.Boolean, _    ByVal ViewOnly As System.Boolean, _    ByVal RapidDraft As System.Boolean, _    ByVal Silent As System.Boolean, _    ByRef Errors As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim FileName As System.String Dim Type As System.Integer Dim ReadOnly As System.Boolean Dim ViewOnly As System.Boolean Dim RapidDraft As System.Boolean Dim Silent As System.Boolean Dim Errors As System.Integer Dim value As System.Object   value = instance.OpenDoc3(FileName, Type, ReadOnly, ViewOnly, RapidDraft, Silent, Errors) ``` | |

| C# |  |
| --- | --- |
| ``` System.object OpenDoc3(     System.string FileName,    System.int Type,    System.bool ReadOnly,    System.bool ViewOnly,    System.bool RapidDraft,    System.bool Silent,    out System.int Errors ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ OpenDoc3(  &   System.String^ FileName, &   System.int Type, &   System.bool ReadOnly, &   System.bool ViewOnly, &   System.bool RapidDraft, &   System.bool Silent, &   [Out] System.int Errors ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FileName*

*Type*

*ReadOnly*

*ViewOnly*

*RapidDraft*

*Silent*

*Errors*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::OpenDoc3.

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)