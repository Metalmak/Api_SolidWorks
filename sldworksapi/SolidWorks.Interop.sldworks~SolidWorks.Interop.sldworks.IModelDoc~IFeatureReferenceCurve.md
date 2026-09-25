<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc~IFeatureReferenceCurve.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IFeatureReferenceCurve Method (IModelDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html) : IFeatureReferenceCurve Method (IModelDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NumOfCurves*

*BaseCurves*

*Merge*

*FromFileName*

*ErrorCode*

Obsolete. Superseded by [IModelDoc2::IFeatureReferenceCurve](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~IFeatureReferenceCurve.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IFeatureReferenceCurve( _    ByVal NumOfCurves As System.Integer, _    ByVal BaseCurves As System.IntPtr, _    ByVal Merge As System.Boolean, _    ByVal FromFileName As System.String, _    ByRef ErrorCode As System.Integer _ ) As ReferenceCurve ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc Dim NumOfCurves As System.Integer Dim BaseCurves As System.IntPtr Dim Merge As System.Boolean Dim FromFileName As System.String Dim ErrorCode As System.Integer Dim value As ReferenceCurve   value = instance.IFeatureReferenceCurve(NumOfCurves, BaseCurves, Merge, FromFileName, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` ReferenceCurve IFeatureReferenceCurve(     System.int NumOfCurves,    System.IntPtr BaseCurves,    System.bool Merge,    System.string FromFileName,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` ReferenceCurve^ IFeatureReferenceCurve(  &   System.int NumOfCurves, &   System.IntPtr BaseCurves, &   System.bool Merge, &   System.String^ FromFileName, &   [Out] System.int ErrorCode ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*NumOfCurves*

*BaseCurves*

*Merge*

*FromFileName*

*ErrorCode*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc::IFeatureReferenceCurve.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html)

[IModelDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc_members.html)