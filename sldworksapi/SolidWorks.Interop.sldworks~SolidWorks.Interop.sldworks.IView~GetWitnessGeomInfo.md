<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetWitnessGeomInfo.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetWitnessGeomInfo Method (IView) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html) : GetWitnessGeomInfo Method (IView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the geometry data for all of the virtual sharp witness lines in this drawing view.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetWitnessGeomInfo() As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IView Dim value As System.Object   value = instance.GetWitnessGeomInfo() ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetWitnessGeomInfo() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetWitnessGeomInfo(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

Array of doubles (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See View::GetWitnessGeomInfo.

# ![](dotnetimages/collapse.gif)Example

[Get Virtual Sharp Witness Line Data (C#)](Get_Virtual_Sharp_Witness_Line_Data_Example_CSharp.htm)

[Get Virtual Sharp Witness Line Data (VB.NET)](Get_Virtual_Sharp_Witness_Line_Data_Example_VBNET.htm)

[Get Virtual Sharp Witness Line Data (VBA)](Get_Virtual_Sharp_Witness_Line_Data_Example_VB.htm)

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
> 0 (**NOTE:**  0 = witness line data),
>
> number (m) of witness lines,
>
> witness line 1[start\_point[x,y,z], end\_point[x,y,z&cd;
>
> ...
>
> witness line m[start\_point[x,y,z], end\_point[x,y,z&cd;,
>
> 1 (**NOTE**: 1 = witness arc data),
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

Call [IView::GetWitnessEntitiesCount](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~GetWitnessEntitiesCount.html) to get the size of the array returned by this method.

# ![](dotnetimages/collapse.gif)See Also

####

[IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html)

[IView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView_members.html)

[IView::IGetWitnessGeomInfo Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~IGetWitnessGeomInfo.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2012 FCS, Revision Number 20.0