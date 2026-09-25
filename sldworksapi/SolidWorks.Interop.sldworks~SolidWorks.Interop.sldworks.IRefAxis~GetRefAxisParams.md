<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefAxis~GetRefAxisParams.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetRefAxisParams Method (IRefAxis) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IRefAxis Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefAxis.html) : GetRefAxisParams Method (IRefAxis) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets information for a reference axis.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetRefAxisParams() As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IRefAxis Dim value As System.Object   value = instance.GetRefAxisParams() ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetRefAxisParams() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetRefAxisParams(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

Array of doubles (see [Remarks](#Remarks))

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See RefAxis::GetRefAxisParams.

# ![](dotnetimages/collapse.gif)Example

[Get Parameters for Reference Axis (VBA)](Get_Parameters_for_Reference_Axis_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

The return value is the following array of doubles:

[ StartPt[3], EndPt[3] ]

where:

* StartPt[3] = array of three values describing the x,y,z start point of the reference axis.

  * EndPt[3] = array of three values describing the x,y,z end point of the reference axis.

# ![](dotnetimages/collapse.gif)See Also

####

[IRefAxis Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefAxis.html)

[IRefAxis Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefAxis_members.html)

[IRefAxis::IGetRefAxisParams Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefAxis~IGetRefAxisParams.html)