<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~FeatureFillet3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| FeatureFillet3 Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : FeatureFillet3 Method (IModelDoc2) |

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

*UseHelpPoint*

*UseTangentHoldLine*

Obsolete. Superseded by [IFeatureManager::FeatureFillet](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~FeatureFillet.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function FeatureFillet3( _    ByVal R1 As System.Double, _    ByVal Propagate As System.Boolean, _    ByVal Ftyp As System.Integer, _    ByVal VarRadTyp As System.Boolean, _    ByVal OverflowType As System.Integer, _    ByVal NRadii As System.Integer, _    ByVal Radii As System.Object, _    ByVal UseHelpPoint As System.Boolean, _    ByVal UseTangentHoldLine As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim R1 As System.Double Dim Propagate As System.Boolean Dim Ftyp As System.Integer Dim VarRadTyp As System.Boolean Dim OverflowType As System.Integer Dim NRadii As System.Integer Dim Radii As System.Object Dim UseHelpPoint As System.Boolean Dim UseTangentHoldLine As System.Boolean Dim value As System.Integer   value = instance.FeatureFillet3(R1, Propagate, Ftyp, VarRadTyp, OverflowType, NRadii, Radii, UseHelpPoint, UseTangentHoldLine) ``` | |

| C# |  |
| --- | --- |
| ``` System.int FeatureFillet3(     System.double R1,    System.bool Propagate,    System.int Ftyp,    System.bool VarRadTyp,    System.int OverflowType,    System.int NRadii,    System.object Radii,    System.bool UseHelpPoint,    System.bool UseTangentHoldLine ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int FeatureFillet3(  &   System.double R1, &   System.bool Propagate, &   System.int Ftyp, &   System.bool VarRadTyp, &   System.int OverflowType, &   System.int NRadii, &   System.Object^ Radii, &   System.bool UseHelpPoint, &   System.bool UseTangentHoldLine ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*R1*

*Propagate*

*Ftyp*

*VarRadTyp*

*OverflowType*

*NRadii*

*Radii*

*UseHelpPoint*

*UseTangentHoldLine*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::FeatureFillet3.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)