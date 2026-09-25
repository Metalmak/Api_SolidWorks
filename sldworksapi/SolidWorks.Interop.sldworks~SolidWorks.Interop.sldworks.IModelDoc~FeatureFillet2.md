<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc~FeatureFillet2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| FeatureFillet2 Method (IModelDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html) : FeatureFillet2 Method (IModelDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*R1*

*Propagate*

*Ftyp*

*VarRadTyp*

*OverflowType*

*NRadii*

*Radii*

Obsolete. Superseded by [IModelDoc2::FeatureFillet2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~FeatureFillet2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function FeatureFillet2( _    ByVal R1 As System.Double, _    ByVal Propagate As System.Boolean, _    ByVal Ftyp As System.Boolean, _    ByVal VarRadTyp As System.Boolean, _    ByVal OverflowType As System.Integer, _    ByVal NRadii As System.Integer, _    ByVal Radii As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc Dim R1 As System.Double Dim Propagate As System.Boolean Dim Ftyp As System.Boolean Dim VarRadTyp As System.Boolean Dim OverflowType As System.Integer Dim NRadii As System.Integer Dim Radii As System.Object Dim value As System.Integer   value = instance.FeatureFillet2(R1, Propagate, Ftyp, VarRadTyp, OverflowType, NRadii, Radii) ``` | |

| C# |  |
| --- | --- |
| ``` System.int FeatureFillet2(     System.double R1,    System.bool Propagate,    System.bool Ftyp,    System.bool VarRadTyp,    System.int OverflowType,    System.int NRadii,    System.object Radii ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int FeatureFillet2(  &   System.double R1, &   System.bool Propagate, &   System.bool Ftyp, &   System.bool VarRadTyp, &   System.int OverflowType, &   System.int NRadii, &   System.Object^ Radii ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*R1*

*Propagate*

*Ftyp*

*VarRadTyp*

*OverflowType*

*NRadii*

*Radii*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc::FeatureFillet2.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html)

[IModelDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc_members.html)