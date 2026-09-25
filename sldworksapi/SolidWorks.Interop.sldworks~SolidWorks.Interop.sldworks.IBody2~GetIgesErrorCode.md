<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetIgesErrorCode.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetIgesErrorCode Method (IBody2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html) : GetIgesErrorCode Method (IBody2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Index*
:   Position of the error within the current list of errors

Gets the current IGES error code.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetIgesErrorCode( _    ByVal Index As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBody2 Dim Index As System.Integer Dim value As System.Integer   value = instance.GetIgesErrorCode(Index) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetIgesErrorCode(     System.int Index ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetIgesErrorCode(  &   System.int Index ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Index*
:   Position of the error within the current list of errors

#### Return Value

IGES error code

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Body2::GetIgesErrorCode.

# ![](dotnetimages/collapse.gif)Remarks

This method is intended for use during IGES processing only.

# ![](dotnetimages/collapse.gif)See Also

####

[IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html)

[IBody2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2_members.html)

[IBody2::GetIgesErrorCount Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetIgesErrorCount.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0