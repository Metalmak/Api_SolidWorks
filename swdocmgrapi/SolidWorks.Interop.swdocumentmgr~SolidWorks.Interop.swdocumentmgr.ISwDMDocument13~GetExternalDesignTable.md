<!-- source: swdocmgrapi/SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument13~GetExternalDesignTable.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Document Manager API Help | Send comments on this topic. |
| GetExternalDesignTable Method (ISwDMDocument13) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdocumentmgr Namespace](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr_namespace.html) > [ISwDMDocument13 Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument13.html) : GetExternalDesignTable Method (ISwDMDocument13) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*pSrcOption*
:   Pointer to an [ISwDMSerachOption](SOLIDWORKS.Interop.swdocumentmgr~SOLIDWORKS.Interop.swdocumentmgr.ISwDMSearchOption.html) object

*Status*
:   Error status as defined by [SwDmDesignTableDataError](SOLIDWORKS.Interop.swdocumentmgr~SOLIDWORKS.Interop.swdocumentmgr.SwDmDesignTableDataError.html)

Gets the path to an external (i.e., linked) design table, if one exists.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetExternalDesignTable( _    ByVal pSrcOption As SwDMSearchOption, _    ByRef Status As SwDmDesignTableDataError _ ) As System.String ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwDMDocument13 Dim pSrcOption As SwDMSearchOption Dim Status As SwDmDesignTableDataError Dim value As System.String   value = instance.GetExternalDesignTable(pSrcOption, Status) ``` | |

| C# |  |
| --- | --- |
| ``` System.string GetExternalDesignTable(     SwDMSearchOption pSrcOption,    out SwDmDesignTableDataError Status ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.String^ GetExternalDesignTable(  &   SwDMSearchOption^ pSrcOption, &   [Out] SwDmDesignTableDataError Status ) ``` | |

#### Parameters

*pSrcOption*
:   Pointer to an [ISwDMSerachOption](SOLIDWORKS.Interop.swdocumentmgr~SOLIDWORKS.Interop.swdocumentmgr.ISwDMSearchOption.html) object

*Status*
:   Error status as defined by [SwDmDesignTableDataError](SOLIDWORKS.Interop.swdocumentmgr~SOLIDWORKS.Interop.swdocumentmgr.SwDmDesignTableDataError.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwDMDocument13::GetExternalDesignTable.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwDMDocument13 Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument13.html)

[ISwDMDocument13 Members](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument13_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Document Manager API 2009 SP0