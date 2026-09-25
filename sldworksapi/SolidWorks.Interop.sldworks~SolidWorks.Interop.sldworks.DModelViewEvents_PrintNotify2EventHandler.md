<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DModelViewEvents_PrintNotify2EventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DModelViewEvents\_PrintNotify2EventHandler Delegate (SolidWorks.Interop.sldworks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : DModelViewEvents\_PrintNotify2EventHandler Delegate (SolidWorks.Interop.sldworks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*pDC*
:   Pointer to the printer device context used to print the document (**see Remarks**)

*bPreview*
:   True to preview the document, false to not

Notifies the user program when a document is printed.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DModelViewEvents_PrintNotify2EventHandler( _    ByVal pDC As System.Long, _    ByVal bPreview As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DModelViewEvents_PrintNotify2EventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DModelViewEvents_PrintNotify2EventHandler(     System.long pDC,    System.bool bPreview ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DModelViewEvents_PrintNotify2EventHandler(  &   System.int64 pDC, &   System.bool bPreview ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*pDC*
:   Pointer to the printer device context used to print the document (**see Remarks**)

*bPreview*
:   True to preview the document, false to not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PrintNotify2 Event (ModelView).

# ![](dotnetimages/collapse.gif)Remarks

Always return S\_OK in the swViewPrintNotify2 event handler.

If developing a C++ application, use swViewPrintNotify2 to register for this notification.

pDC is the address of an MFC CDC instance, and it can be cast to a CDC\*. C++ applications wanting to use this CDC\* need to dynamically link to the MFC DLLs and use the same version of the Visual C++ compiler that SOLIDWORKS uses.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2014 FCS, Revision Number 22.0