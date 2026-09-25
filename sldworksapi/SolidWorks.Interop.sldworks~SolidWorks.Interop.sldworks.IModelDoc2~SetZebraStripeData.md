<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~SetZebraStripeData.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetZebraStripeData Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : SetZebraStripeData Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Size*
:   Number of stripes

*Ratio*
:   Width of the stripes

*Color1*
:   First color in zebra stripe design

*Color2*
:   Second color in zebra stripe design

Sets the zebra-line data.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetZebraStripeData( _    ByVal Size As System.Double, _    ByVal Ratio As System.Double, _    ByVal Color1 As System.Integer, _    ByVal Color2 As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim Size As System.Double Dim Ratio As System.Double Dim Color1 As System.Integer Dim Color2 As System.Integer   instance.SetZebraStripeData(Size, Ratio, Color1, Color2) ``` | |

| C# |  |
| --- | --- |
| ``` void SetZebraStripeData(     System.double Size,    System.double Ratio,    System.int Color1,    System.int Color2 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetZebraStripeData(  &   System.double Size, &   System.double Ratio, &   System.int Color1, &   System.int Color2 ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Size*
:   Number of stripes

*Ratio*
:   Width of the stripes

*Color1*
:   First color in zebra stripe design

*Color2*
:   Second color in zebra stripe design

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::SetZebraStripeData.

# ![](dotnetimages/collapse.gif)Remarks

The Size parameter is inversely related; a large size value generates lots of small stripes.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

[IModelDoc2::GetZebraStripeData Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~GetZebraStripeData.html)

[IModelView::DisplayZebraStripes Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView~DisplayZebraStripes.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0