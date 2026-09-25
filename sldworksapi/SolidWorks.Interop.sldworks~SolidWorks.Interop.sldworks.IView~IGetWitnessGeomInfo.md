<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~IGetWitnessGeomInfo.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetWitnessGeomInfo Method (IView) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html) : IGetWitnessGeomInfo Method (IView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ArraySize*
:   Size of the virtual sharp witness line geometry data array (see **Remarks**)

Gets the geometry data for all of the virtual sharp witness lines in this drawing view.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetWitnessGeomInfo( _    ByVal ArraySize As System.Integer _ ) As System.Double ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IView Dim ArraySize As System.Integer Dim value As System.Double   value = instance.IGetWitnessGeomInfo(ArraySize) ``` | |

| C# |  |
| --- | --- |
| ``` System.double IGetWitnessGeomInfo(     System.int ArraySize ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.double IGetWitnessGeomInfo(  &   System.int ArraySize ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ArraySize*
:   Size of the virtual sharp witness line geometry data array (see **Remarks**)

#### Return Value

* in-process, unmanaged C++: Pointer to an array of doubles (see **Remarks**)* VBA, VB.NET, C#, and C++/CLI: Not supported

See In-process Methods for details about this type of method.

# ![](dotnetimages/collapse.gif)Remarks

This method returns an array containing the following data for each virtual sharp in the view:

> [*color\_value*,
>
> swLineStyles\_e option (-1 if no line style is specified),
>
> swLineWeights\_e option (-1 if no line weight is specified),
>
> layer ID (-1 if no layer is specified),
>
> swLayerOverride\_e option,
>
> 0 (**NOTE:** 0 = witness line data),
>
> number (m) of witness lines,
>
> witness line 1[start\_point[x,y,z], end\_point[x,y,z&cd;
>
> ...
>
> witness line m[start\_point[x,y,z], end\_point[x,y,z&cd;,
>
> 1 (**NOTE:** 1 = witness arc data),
>
> number (n) of witness arcs,
>
> witness arc 1[start\_point[x,y,z], end\_point[x,y,z], center\_point[x,y,z], normal\_point[x,y,z&cd;
>
> ...
>
> witness arc n[start\_point[x,y,z], end\_point[x,y,z], center\_point[x,y,z], normal\_point[x,y,z&cd;]

Where:

> *color\_value =* MAX(MIN(*red\_rgb\_value*,255),0) *+* MAX(MIN(*green\_rgb\_value*,255),0)\*16\*16 *+* MAX(MIN(*blue\_rgb\_value*,255),0)\*16\*16\*16\*16

Before calling this method, call [IView::GetWitnessEntitiesCount](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~GetWitnessEntitiesCount.html) to get the size of the array returned by this method.

# ![](dotnetimages/collapse.gif)See Also

####

[IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html)

[IView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView_members.html)

[IView::GetWitnessGeomInfo Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetWitnessGeomInfo.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2012 FCS, Revision Number 20.0