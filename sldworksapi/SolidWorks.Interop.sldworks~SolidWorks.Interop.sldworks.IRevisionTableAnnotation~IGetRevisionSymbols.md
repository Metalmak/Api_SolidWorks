<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRevisionTableAnnotation~IGetRevisionSymbols.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetRevisionSymbols Method (IRevisionTableAnnotation) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IRevisionTableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRevisionTableAnnotation.html) : IGetRevisionSymbols Method (IRevisionTableAnnotation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*RevisionId*
:   Revision ID

*Count*
:   Number of revision symbols

Gets the revision symbols associated with the specified revision ID.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetRevisionSymbols( _    ByVal RevisionId As System.Integer, _    ByVal Count As System.Integer _ ) As Note ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IRevisionTableAnnotation Dim RevisionId As System.Integer Dim Count As System.Integer Dim value As Note   value = instance.IGetRevisionSymbols(RevisionId, Count) ``` | |

| C# |  |
| --- | --- |
| ``` Note IGetRevisionSymbols(     System.int RevisionId,    System.int Count ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Note^ IGetRevisionSymbols(  &   System.int RevisionId, &   System.int Count ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*RevisionId*
:   Revision ID

*Count*
:   Number of revision symbols

#### Return Value

* in-process, unmanaged C++: Pointer to an array of revision symbols

- VBA, VB.NET, C#, and C++/CLI: Not supported

  See In-process Methods for details about this type of method.

# ![](dotnetimages/collapse.gif)Remarks

Call [IRevisionTableAnnotation::GetRevisionSymbolCount](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IRevisionTableAnnotation~GetRevisionSymbolCount.html) before calling this method to get the value of Count.

# ![](dotnetimages/collapse.gif)See Also

####

[IRevisionTableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRevisionTableAnnotation.html)

[IRevisionTableAnnotation Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRevisionTableAnnotation_members.html)

[IRevisionTableAnnotation::GetRevisionSymbols Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRevisionTableAnnotation~GetRevisionSymbols.html)

[IRevisionTableAnnotation::CurrentRevision Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRevisionTableAnnotation~CurrentRevision.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12.0