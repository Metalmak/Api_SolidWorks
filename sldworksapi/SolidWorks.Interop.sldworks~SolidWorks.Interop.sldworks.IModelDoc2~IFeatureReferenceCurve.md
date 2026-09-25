<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~IFeatureReferenceCurve.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IFeatureReferenceCurve Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : IFeatureReferenceCurve Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NumOfCurves*
:   Number of curves from which to create the object

*BaseCurves*
:   Array of [curves](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve.html)

*Merge*
:   True creates a single reference curve feature, false creates a reference curve feature for each curve in the array

*FromFileName*
:   Not used

*ErrorCode*
:   Error code as defined in swFeatureError\_e

Creates a reference curve feature from an array of curves.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IFeatureReferenceCurve( _    ByVal NumOfCurves As System.Integer, _    ByRef BaseCurves As Curve, _    ByVal Merge As System.Boolean, _    ByVal FromFileName As System.String, _    ByRef ErrorCode As System.Integer _ ) As ReferenceCurve ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim NumOfCurves As System.Integer Dim BaseCurves As Curve Dim Merge As System.Boolean Dim FromFileName As System.String Dim ErrorCode As System.Integer Dim value As ReferenceCurve   value = instance.IFeatureReferenceCurve(NumOfCurves, BaseCurves, Merge, FromFileName, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` ReferenceCurve IFeatureReferenceCurve(     System.int NumOfCurves,    ref Curve BaseCurves,    System.bool Merge,    System.string FromFileName,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` ReferenceCurve^ IFeatureReferenceCurve(  &   System.int NumOfCurves, &   Curve^% BaseCurves, &   System.bool Merge, &   System.String^ FromFileName, &   [Out] System.int ErrorCode ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*NumOfCurves*
:   Number of curves from which to create the object

*BaseCurves*
:   Array of [curves](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve.html)

*Merge*
:   True creates a single reference curve feature, false creates a reference curve feature for each curve in the array

*FromFileName*
:   Not used

*ErrorCode*
:   Error code as defined in swFeatureError\_e

#### Return Value

[Reference curve](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IReferenceCurve.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::IFeatureReferenceCurve.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

[IModelDoc2::FeatureReferenceCurve Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~FeatureReferenceCurve.html)