<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~GetControlPointConicRhoOrRadiusAtIndex.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetControlPointConicRhoOrRadiusAtIndex Method (IVariableFilletFeatureData2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IVariableFilletFeatureData2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2.html) : GetControlPointConicRhoOrRadiusAtIndex Method (IVariableFilletFeatureData2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Index*
:   Zero-based index of the control point  (see **Remarks**)

Gets the conic rho or radius at the specified control point.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetControlPointConicRhoOrRadiusAtIndex( _    ByVal Index As System.Integer _ ) As System.Double ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IVariableFilletFeatureData2 Dim Index As System.Integer Dim value As System.Double   value = instance.GetControlPointConicRhoOrRadiusAtIndex(Index) ``` | |

| C# |  |
| --- | --- |
| ``` System.double GetControlPointConicRhoOrRadiusAtIndex(     System.int Index ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.double GetControlPointConicRhoOrRadiusAtIndex(  &   System.int Index ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Index*
:   Zero-based index of the control point  (see **Remarks**)

#### Return Value

Conic rho or radius

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See VariableFilletFeatureData2::GetControlPointConicRhoOrRadiusAtIndex.

# ![](dotnetimages/collapse.gif)Remarks

Call [IVariableFilletFeatureData2::GetControlPointsCount](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IVariableFilletFeatureData2~GetControlPointsCount.html) before calling this method to determine a value for Index.

If [IVariableFilletFeatureData2::ConicTypeForCrossSectionProfile](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~ConicTypeForCrossSectionProfile.html) is set to swFeatureFilletProfileType\_e.:

* swFeatureFilletConicRadius (symmetric fillet only), then this method returns a radius.* swFeatureFilletConicRho (symmetric or asymmetric fillet), then this method returns a conic rho value in the range [0.05, 0.95].

See Accessing Selections that Define Features for additional details.

# ![](dotnetimages/collapse.gif)See Also

####

[IVariableFilletFeatureData2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2.html)

[IVariableFilletFeatureData2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2_members.html)

[IVariableFilletFeatureData2::SetControlPointConicRhoOrRadiusAtIndex Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~SetControlPointConicRhoOrRadiusAtIndex.html)

[IVariableFilletFeatureData2::GetControlPointRadiusAtIndex Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~GetControlPointRadiusAtIndex.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2014 FCS, Revision Number 22.0