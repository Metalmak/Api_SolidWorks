<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc~ICreateSplinesByEqnParams.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ICreateSplinesByEqnParams Method (IModelDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html) : ICreateSplinesByEqnParams Method (IModelDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*PropArray*

*KnotsArray*

*CntrlPntCoordArray*

Obsolete. Superseded by [IModelDoc2::ICreateSplinesByEqnParams](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~ICreateSplinesByEqnParams.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ICreateSplinesByEqnParams( _    ByRef PropArray As System.Integer, _    ByRef KnotsArray As System.Double, _    ByRef CntrlPntCoordArray As System.Double _ ) As EnumSketchSegments ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc Dim PropArray As System.Integer Dim KnotsArray As System.Double Dim CntrlPntCoordArray As System.Double Dim value As EnumSketchSegments   value = instance.ICreateSplinesByEqnParams(PropArray, KnotsArray, CntrlPntCoordArray) ``` | |

| C# |  |
| --- | --- |
| ``` EnumSketchSegments ICreateSplinesByEqnParams(     ref System.int PropArray,    ref System.double KnotsArray,    ref System.double CntrlPntCoordArray ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` EnumSketchSegments^ ICreateSplinesByEqnParams(  &   System.int% PropArray, &   System.double% KnotsArray, &   System.double% CntrlPntCoordArray ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*PropArray*

*KnotsArray*

*CntrlPntCoordArray*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc::ICreateSplinesByEqnParams.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html)

[IModelDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc_members.html)