<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody~ICreatePsplineSurfaceDLL.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ICreatePsplineSurfaceDLL Method (IBody) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBody Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody.html) : ICreatePsplineSurfaceDLL Method (IBody) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Dim*

*UOrder*

*VOrder*

*Ncol*

*Nrow*

*Coeffs*

*Basis*

*Xform*

*ScaleFactor*

Obsolete. Superseded by [IBody2::ICreatePsplineSurfaceDLL](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~ICreatePsplineSurfaceDLL.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ICreatePsplineSurfaceDLL( _    ByVal Dim As System.Integer, _    ByVal UOrder As System.Integer, _    ByVal VOrder As System.Integer, _    ByVal Ncol As System.Integer, _    ByVal Nrow As System.Integer, _    ByRef Coeffs As System.Double, _    ByVal Basis As System.Integer, _    ByRef Xform As System.Double, _    ByVal ScaleFactor As System.Double _ ) As Surface ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBody Dim Dim As System.Integer Dim UOrder As System.Integer Dim VOrder As System.Integer Dim Ncol As System.Integer Dim Nrow As System.Integer Dim Coeffs As System.Double Dim Basis As System.Integer Dim Xform As System.Double Dim ScaleFactor As System.Double Dim value As Surface   value = instance.ICreatePsplineSurfaceDLL(Dim, UOrder, VOrder, Ncol, Nrow, Coeffs, Basis, Xform, ScaleFactor) ``` | |

| C# |  |
| --- | --- |
| ``` Surface ICreatePsplineSurfaceDLL(     System.int Dim,    System.int UOrder,    System.int VOrder,    System.int Ncol,    System.int Nrow,    ref System.double Coeffs,    System.int Basis,    ref System.double Xform,    System.double ScaleFactor ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Surface^ ICreatePsplineSurfaceDLL(  &   System.int Dim, &   System.int UOrder, &   System.int VOrder, &   System.int Ncol, &   System.int Nrow, &   System.double% Coeffs, &   System.int Basis, &   System.double% Xform, &   System.double ScaleFactor ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Dim*

*UOrder*

*VOrder*

*Ncol*

*Nrow*

*Coeffs*

*Basis*

*Xform*

*ScaleFactor*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Body::ICreatePsplineSurfaceDLL.

# ![](dotnetimages/collapse.gif)See Also

####

[IBody Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody.html)

[IBody Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody_members.html)