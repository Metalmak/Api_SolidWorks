<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc~FeatureRevolve2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| FeatureRevolve2 Method (IPartDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPartDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc.html) : FeatureRevolve2 Method (IPartDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Angle*

*ReverseDir*

*Angle2*

*RevType*

*Merge*

Obsolete. Superseded by [IFeatureManager::FeatureRevolve](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~FeatureRevolve.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub FeatureRevolve2( _    ByVal Angle As System.Double, _    ByVal ReverseDir As System.Boolean, _    ByVal Angle2 As System.Double, _    ByVal RevType As System.Integer, _    ByVal Merge As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPartDoc Dim Angle As System.Double Dim ReverseDir As System.Boolean Dim Angle2 As System.Double Dim RevType As System.Integer Dim Merge As System.Boolean   instance.FeatureRevolve2(Angle, ReverseDir, Angle2, RevType, Merge) ``` | |

| C# |  |
| --- | --- |
| ``` void FeatureRevolve2(     System.double Angle,    System.bool ReverseDir,    System.double Angle2,    System.int RevType,    System.bool Merge ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void FeatureRevolve2(  &   System.double Angle, &   System.bool ReverseDir, &   System.double Angle2, &   System.int RevType, &   System.bool Merge ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Angle*

*ReverseDir*

*Angle2*

*RevType*

*Merge*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PartDoc::FeatureRevolve2.

# ![](dotnetimages/collapse.gif)See Also

####

[IPartDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc.html)

[IPartDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc_members.html)