<!-- source: swdocmgrapi/SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument22~GetFileAvgTime.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Document Manager API Help | Send comments on this topic. |
| GetFileAvgTime Method (ISwDMDocument22) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdocumentmgr Namespace](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr_namespace.html) > [ISwDMDocument22 Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument22.html) : GetFileAvgTime Method (ISwDMDocument22) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*bsFileTime*
:   Last open time; "*mm* mins *ss* secs" or "unknown"

*bsLWFileTime*
:   Last lightweight open time; "*mm* mins *ss* secs" or "unknown LW"

Gets the amount of time it took to open this document the last time.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetFileAvgTime( _    ByRef bsFileTime As System.String, _    ByRef bsLWFileTime As System.String _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwDMDocument22 Dim bsFileTime As System.String Dim bsLWFileTime As System.String   instance.GetFileAvgTime(bsFileTime, bsLWFileTime) ``` | |

| C# |  |
| --- | --- |
| ``` void GetFileAvgTime(     out System.string bsFileTime,    out System.string bsLWFileTime ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetFileAvgTime(  &   [Out] System.String^ bsFileTime, &   [Out] System.String^ bsLWFileTime ) ``` | |

#### Parameters

*bsFileTime*
:   Last open time; "*mm* mins *ss* secs" or "unknown"

*bsLWFileTime*
:   Last lightweight open time; "*mm* mins *ss* secs" or "unknown LW"

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwDMDocument22::GetFileAvgTime.

# ![](dotnetimages/collapse.gif)Example

See the [ISwDMDocument22](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument22.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwDMDocument22 Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument22.html)

[ISwDMDocument22 Members](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument22_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Document Manager API 2018 SP0