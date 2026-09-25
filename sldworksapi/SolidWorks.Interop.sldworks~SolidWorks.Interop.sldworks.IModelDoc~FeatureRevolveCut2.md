<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc~FeatureRevolveCut2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| FeatureRevolveCut2 Method (IModelDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html) : FeatureRevolveCut2 Method (IModelDoc) |

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

*Options*

Obsolete. Superseded by [IModelDoc2::FetureRevolveCut2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~FeatureRevolveCut2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function FeatureRevolveCut2( _    ByVal Angle As System.Double, _    ByVal ReverseDir As System.Boolean, _    ByVal Angle2 As System.Double, _    ByVal RevType As System.Integer, _    ByVal Options As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc Dim Angle As System.Double Dim ReverseDir As System.Boolean Dim Angle2 As System.Double Dim RevType As System.Integer Dim Options As System.Integer Dim value As System.Integer   value = instance.FeatureRevolveCut2(Angle, ReverseDir, Angle2, RevType, Options) ``` | |

| C# |  |
| --- | --- |
| ``` System.int FeatureRevolveCut2(     System.double Angle,    System.bool ReverseDir,    System.double Angle2,    System.int RevType,    System.int Options ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int FeatureRevolveCut2(  &   System.double Angle, &   System.bool ReverseDir, &   System.double Angle2, &   System.int RevType, &   System.int Options ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Angle*

*ReverseDir*

*Angle2*

*RevType*

*Options*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc::FeatureRevolveCut2.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html)

[IModelDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc_members.html)