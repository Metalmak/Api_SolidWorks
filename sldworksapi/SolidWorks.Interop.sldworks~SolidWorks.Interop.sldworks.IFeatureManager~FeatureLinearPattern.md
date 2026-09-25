<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~FeatureLinearPattern.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| FeatureLinearPattern Method (IFeatureManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : FeatureLinearPattern Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Num1*

*Spacing1*

*Num2*

*Spacing2*

*FlipDir1*

*FlipDir2*

*DName1*

*DName2*

Obsolete. Superseded by [IFeatureManager::FeatureLinearPattern2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~FeatureLinearPattern2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function FeatureLinearPattern( _    ByVal Num1 As System.Integer, _    ByVal Spacing1 As System.Double, _    ByVal Num2 As System.Integer, _    ByVal Spacing2 As System.Double, _    ByVal FlipDir1 As System.Boolean, _    ByVal FlipDir2 As System.Boolean, _    ByVal DName1 As System.String, _    ByVal DName2 As System.String _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Num1 As System.Integer Dim Spacing1 As System.Double Dim Num2 As System.Integer Dim Spacing2 As System.Double Dim FlipDir1 As System.Boolean Dim FlipDir2 As System.Boolean Dim DName1 As System.String Dim DName2 As System.String Dim value As Feature   value = instance.FeatureLinearPattern(Num1, Spacing1, Num2, Spacing2, FlipDir1, FlipDir2, DName1, DName2) ``` | |

| C# |  |
| --- | --- |
| ``` Feature FeatureLinearPattern(     System.int Num1,    System.double Spacing1,    System.int Num2,    System.double Spacing2,    System.bool FlipDir1,    System.bool FlipDir2,    System.string DName1,    System.string DName2 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ FeatureLinearPattern(  &   System.int Num1, &   System.double Spacing1, &   System.int Num2, &   System.double Spacing2, &   System.bool FlipDir1, &   System.bool FlipDir2, &   System.String^ DName1, &   System.String^ DName2 ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Num1*

*Spacing1*

*Num2*

*Spacing2*

*FlipDir1*

*FlipDir2*

*DName1*

*DName2*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::FeatureLinearPattern.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)