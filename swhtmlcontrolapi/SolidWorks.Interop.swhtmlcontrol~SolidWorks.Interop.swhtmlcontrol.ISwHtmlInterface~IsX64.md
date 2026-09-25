<!-- source: swhtmlcontrolapi/SolidWorks.Interop.swhtmlcontrol~SolidWorks.Interop.swhtmlcontrol.ISwHtmlInterface~IsX64.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS HTML Control Type Library | Send comments on this topic. |
| IsX64 Method (ISwHtmlInterface) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swhtmlcontrol Namespace](SolidWorks.Interop.swhtmlcontrol~SolidWorks.Interop.swhtmlcontrol_namespace.html) > [ISwHtmlInterface Interface](SolidWorks.Interop.swhtmlcontrol~SolidWorks.Interop.swhtmlcontrol.ISwHtmlInterface.html) : IsX64 Method (ISwHtmlInterface) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets whether you are running SOLIDWORKS (32-bit) or SOLIDWORKS x64 (64-bit).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IsX64() As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwHtmlInterface Dim value As System.Integer   value = instance.IsX64() ``` | |

| C# |  |
| --- | --- |
| ``` System.int IsX64() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int IsX64(); ``` | |

#### Return Value

TRUE if you are running SOLIDWORKS x64, FALSE if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwHtmlInterface::IsX64.

# ![](dotnetimages/collapse.gif)Remarks

|  |  |
| --- | --- |
| If running... | Then this method returns... |
| SOLIDWORKS on 32-bit machine | FALSE |
| SOLIDWORKS on a 64-bit machine | FALSE |
| SOLIDWORKS x64 on a 64-bit machine | TRUE |

# ![](dotnetimages/collapse.gif)See Also

####

[ISwHtmlInterface Interface](SolidWorks.Interop.swhtmlcontrol~SolidWorks.Interop.swhtmlcontrol.ISwHtmlInterface.html)

[ISwHtmlInterface Members](SolidWorks.Interop.swhtmlcontrol~SolidWorks.Interop.swhtmlcontrol.ISwHtmlInterface_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 SP3, Revision Number 14.3