<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~IFeatureFillet4.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IFeatureFillet4 Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : IFeatureFillet4 Method (IModelDoc2) |

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

*UniformRadius*

*Ftyp*

*VarRadTyp*

*OverflowType*

*NRadii*

*Radii*

*UseHelpPoint*

*UseTangentHoldLine*

*CornerType*

*SetbackDistCount*

*SetBackDistances*

Obsolete. Superseded by [IFeatureManager::FeatureCut](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~FeatureCut.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IFeatureFillet4( _    ByVal R1 As System.Double, _    ByVal Propagate As System.Boolean, _    ByVal UniformRadius As System.Boolean, _    ByVal Ftyp As System.Integer, _    ByVal VarRadTyp As System.Boolean, _    ByVal OverflowType As System.Integer, _    ByVal NRadii As System.Integer, _    ByRef Radii As System.Double, _    ByVal UseHelpPoint As System.Boolean, _    ByVal UseTangentHoldLine As System.Boolean, _    ByVal CornerType As System.Boolean, _    ByVal SetbackDistCount As System.Integer, _    ByRef SetBackDistances As System.Double _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim R1 As System.Double Dim Propagate As System.Boolean Dim UniformRadius As System.Boolean Dim Ftyp As System.Integer Dim VarRadTyp As System.Boolean Dim OverflowType As System.Integer Dim NRadii As System.Integer Dim Radii As System.Double Dim UseHelpPoint As System.Boolean Dim UseTangentHoldLine As System.Boolean Dim CornerType As System.Boolean Dim SetbackDistCount As System.Integer Dim SetBackDistances As System.Double Dim value As System.Integer   value = instance.IFeatureFillet4(R1, Propagate, UniformRadius, Ftyp, VarRadTyp, OverflowType, NRadii, Radii, UseHelpPoint, UseTangentHoldLine, CornerType, SetbackDistCount, SetBackDistances) ``` | |

| C# |  |
| --- | --- |
| ``` System.int IFeatureFillet4(     System.double R1,    System.bool Propagate,    System.bool UniformRadius,    System.int Ftyp,    System.bool VarRadTyp,    System.int OverflowType,    System.int NRadii,    ref System.double Radii,    System.bool UseHelpPoint,    System.bool UseTangentHoldLine,    System.bool CornerType,    System.int SetbackDistCount,    ref System.double SetBackDistances ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int IFeatureFillet4(  &   System.double R1, &   System.bool Propagate, &   System.bool UniformRadius, &   System.int Ftyp, &   System.bool VarRadTyp, &   System.int OverflowType, &   System.int NRadii, &   System.double% Radii, &   System.bool UseHelpPoint, &   System.bool UseTangentHoldLine, &   System.bool CornerType, &   System.int SetbackDistCount, &   System.double% SetBackDistances ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*R1*

*Propagate*

*UniformRadius*

*Ftyp*

*VarRadTyp*

*OverflowType*

*NRadii*

*Radii*

*UseHelpPoint*

*UseTangentHoldLine*

*CornerType*

*SetbackDistCount*

*SetBackDistances*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::IFeatureFillet4.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)