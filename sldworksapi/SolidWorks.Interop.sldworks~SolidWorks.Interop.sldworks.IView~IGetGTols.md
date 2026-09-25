<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~IGetGTols.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetGTols Method (IView) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html) : IGetGTols Method (IView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NumGTol*
:   Total number of geometric tolerances on this drawing view.

Gets all of the geometric tolerances on this drawing view.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetGTols( _    ByVal NumGTol As System.Integer _ ) As Gtol ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IView Dim NumGTol As System.Integer Dim value As Gtol   value = instance.IGetGTols(NumGTol) ``` | |

| C# |  |
| --- | --- |
| ``` Gtol IGetGTols(     System.int NumGTol ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Gtol^ IGetGTols(  &   System.int NumGTol ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*NumGTol*
:   Total number of geometric tolerances on this drawing view.

#### Return Value

* in-process, unmanaged C++: Pointer to an array of [geometric tolerances](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IGtol.html)* VBA, VB.NET, C#, and C++/CLI: Not supported

See In-process Methods for details about this type of method.

# ![](dotnetimages/collapse.gif)Remarks

Use this method to obtain the array of geometric tolerances all at once instead of calling [IView::GetFirstGTOL](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~GetFirstGTOL.html) and then repeatedly calling [IGtol::GetNextGTOL](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IGtol~GetNextGTOL.html) to obtain the remaining geometric tolerances in the drawing view.

Before calling this method, call [IView::GetGTolCount](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~GetGtolCount.html) to get the value for numGTol.

# ![](dotnetimages/collapse.gif)See Also

####

[IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html)

[IView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView_members.html)

[IView::GetGTols Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetGTols.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 SP1, Revision Number 17.1