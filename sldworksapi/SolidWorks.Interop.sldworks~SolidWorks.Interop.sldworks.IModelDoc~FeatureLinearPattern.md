<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc~FeatureLinearPattern.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| FeatureLinearPattern Method (IModelDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html) : FeatureLinearPattern Method (IModelDoc) |

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

Obsolete. Superseded by [IModelDoc2::FeatureLinearPattern](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~FeatureLinearPattern.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub FeatureLinearPattern( _    ByVal Num1 As System.Integer, _    ByVal Spacing1 As System.Double, _    ByVal Num2 As System.Integer, _    ByVal Spacing2 As System.Double, _    ByVal FlipDir1 As System.Boolean, _    ByVal FlipDir2 As System.Boolean, _    ByVal DName1 As System.String, _    ByVal DName2 As System.String _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc Dim Num1 As System.Integer Dim Spacing1 As System.Double Dim Num2 As System.Integer Dim Spacing2 As System.Double Dim FlipDir1 As System.Boolean Dim FlipDir2 As System.Boolean Dim DName1 As System.String Dim DName2 As System.String   instance.FeatureLinearPattern(Num1, Spacing1, Num2, Spacing2, FlipDir1, FlipDir2, DName1, DName2) ``` | |

| C# |  |
| --- | --- |
| ``` void FeatureLinearPattern(     System.int Num1,    System.double Spacing1,    System.int Num2,    System.double Spacing2,    System.bool FlipDir1,    System.bool FlipDir2,    System.string DName1,    System.string DName2 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void FeatureLinearPattern(  &   System.int Num1, &   System.double Spacing1, &   System.int Num2, &   System.double Spacing2, &   System.bool FlipDir1, &   System.bool FlipDir2, &   System.String^ DName1, &   System.String^ DName2 ) ``` | |

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

See ModelDoc::FeatureLinearPattern.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html)

[IModelDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc_members.html)