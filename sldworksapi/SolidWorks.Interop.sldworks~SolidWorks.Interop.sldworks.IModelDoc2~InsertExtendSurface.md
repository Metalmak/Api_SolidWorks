<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~InsertExtendSurface.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertExtendSurface Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : InsertExtendSurface Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ExtendLinear*
:   True to extend surface linearly, false to extend along the same surface

*EndCondition*
:   * 0 - Extend surface by given distance* 1 - Extend surface up to a selected point* 2 - Extend surface up to a selected surface

*Distance*
:   Distance to extend surface along

Extends a surface along the selected faces or edges.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub InsertExtendSurface( _    ByVal ExtendLinear As System.Boolean, _    ByVal EndCondition As System.Integer, _    ByVal Distance As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim ExtendLinear As System.Boolean Dim EndCondition As System.Integer Dim Distance As System.Double   instance.InsertExtendSurface(ExtendLinear, EndCondition, Distance) ``` | |

| C# |  |
| --- | --- |
| ``` void InsertExtendSurface(     System.bool ExtendLinear,    System.int EndCondition,    System.double Distance ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void InsertExtendSurface(  &   System.bool ExtendLinear, &   System.int EndCondition, &   System.double Distance ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ExtendLinear*
:   True to extend surface linearly, false to extend along the same surface

*EndCondition*
:   * 0 - Extend surface by given distance* 1 - Extend surface up to a selected point* 2 - Extend surface up to a selected surface

*Distance*
:   Distance to extend surface along

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::InsertExtendSurface.

# ![](dotnetimages/collapse.gif)Remarks

The selection list can contain faces or edges from the surface. These selected entities will be extended away from the surface according to the input arguments.

The selected point or surface to which to extend should be in the selection list. If EndCondition is to a selected surface, then currently only faces from solids are supported through the API.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

[ISurfaceExtendFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurfaceExtendFeatureData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0