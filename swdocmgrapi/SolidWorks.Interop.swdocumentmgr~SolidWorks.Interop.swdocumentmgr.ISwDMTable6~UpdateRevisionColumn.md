<!-- source: swdocmgrapi/SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMTable6~UpdateRevisionColumn.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Document Manager API Help | Send comments on this topic. |
| UpdateRevisionColumn Method (ISwDMTable6) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdocumentmgr Namespace](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr_namespace.html) > [ISwDMTable6 Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMTable6.html) : UpdateRevisionColumn Method (ISwDMTable6) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Revision*
:   Revision; if empty, the column in the latest revision row is updated

*ColType*
:   Type of column as defined in [SwDmColumnType](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.SwDmColumnType.html)

*Data*
:   Column data

Updates the specified revision column in this table.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function UpdateRevisionColumn( _    ByVal Revision As System.String, _    ByVal ColType As SwDmColumnType, _    ByVal Data As System.String _ ) As SwDmTableError ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwDMTable6 Dim Revision As System.String Dim ColType As SwDmColumnType Dim Data As System.String Dim value As SwDmTableError   value = instance.UpdateRevisionColumn(Revision, ColType, Data) ``` | |

| C# |  |
| --- | --- |
| ``` SwDmTableError UpdateRevisionColumn(     System.string Revision,    SwDmColumnType ColType,    System.string Data ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` SwDmTableError UpdateRevisionColumn(  &   System.String^ Revision, &   SwDmColumnType ColType, &   System.String^ Data ) ``` | |

#### Parameters

*Revision*
:   Revision; if empty, the column in the latest revision row is updated

*ColType*
:   Type of column as defined in [SwDmColumnType](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.SwDmColumnType.html)

*Data*
:   Column data

#### Return Value

Return code as defined in [swDmTableError](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.SwDmTableError.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwDMTable6::UpdateRevisionColumn.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwDMTable6 Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMTable6.html)

[ISwDMTable6 Members](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMTable6_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Document Manager API 2018 SP0