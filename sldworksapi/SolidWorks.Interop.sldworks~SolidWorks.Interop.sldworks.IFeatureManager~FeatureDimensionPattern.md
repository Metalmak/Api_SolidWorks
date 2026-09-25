<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~FeatureDimensionPattern.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| FeatureDimensionPattern Method (IFeatureManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : FeatureDimensionPattern Method (IFeatureManager) |

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

*DiagonalOnly*

*DName1*

*DName2*

*VaryInstance*

Not implemented.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function FeatureDimensionPattern( _    ByVal Num1 As System.Integer, _    ByVal Spacing1 As System.Double, _    ByVal Num2 As System.Integer, _    ByVal Spacing2 As System.Double, _    ByVal DiagonalOnly As System.Boolean, _    ByVal DName1 As System.String, _    ByVal DName2 As System.String, _    ByVal VaryInstance As System.Boolean _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Num1 As System.Integer Dim Spacing1 As System.Double Dim Num2 As System.Integer Dim Spacing2 As System.Double Dim DiagonalOnly As System.Boolean Dim DName1 As System.String Dim DName2 As System.String Dim VaryInstance As System.Boolean Dim value As Feature   value = instance.FeatureDimensionPattern(Num1, Spacing1, Num2, Spacing2, DiagonalOnly, DName1, DName2, VaryInstance) ``` | |

| C# |  |
| --- | --- |
| ``` Feature FeatureDimensionPattern(     System.int Num1,    System.double Spacing1,    System.int Num2,    System.double Spacing2,    System.bool DiagonalOnly,    System.string DName1,    System.string DName2,    System.bool VaryInstance ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ FeatureDimensionPattern(  &   System.int Num1, &   System.double Spacing1, &   System.int Num2, &   System.double Spacing2, &   System.bool DiagonalOnly, &   System.String^ DName1, &   System.String^ DName2, &   System.bool VaryInstance ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Num1*

*Spacing1*

*Num2*

*Spacing2*

*DiagonalOnly*

*DName1*

*DName2*

*VaryInstance*

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

Not implemented