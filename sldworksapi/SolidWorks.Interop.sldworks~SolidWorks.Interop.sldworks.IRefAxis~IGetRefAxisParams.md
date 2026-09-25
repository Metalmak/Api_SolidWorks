<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefAxis~IGetRefAxisParams.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetRefAxisParams Method (IRefAxis) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IRefAxis Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefAxis.html) : IGetRefAxisParams Method (IRefAxis) |

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
| ``` Function IGetRefAxisParams() As System.Double ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IRefAxis Dim value As System.Double   value = instance.IGetRefAxisParams() ``` | |

| C# |  |
| --- | --- |
| ``` System.double IGetRefAxisParams() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.double IGetRefAxisParams(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

* in-process, unmanaged C++: Pointer to an array of doubles (see [Remarks](#Remarks))

- VBA, VB.NET, C#, and C++/CLI: Not supported

  See In-process Methods for details about this type of method.

# ![](dotnetimages/collapse.gif)Example

[Get Info on Plane-Axis (C++)](Get_Info_on_Plane_Axis_Example_CPlusPlus_COM.htm)

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

[IRefAxis::GetRefAxisParams Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefAxis~GetRefAxisParams.html)