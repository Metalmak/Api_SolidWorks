<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~InsertScale.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertScale Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : InsertScale Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ScaleFactor\_x*

*ScaleFactor\_y*

*ScaleFactor\_z*

*IsUniform*

*ScaleType*

Obsolete. Superseded by [IFeatureManager::InsertScale](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~InsertScale.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub InsertScale( _    ByVal ScaleFactor_x As System.Double, _    ByVal ScaleFactor_y As System.Double, _    ByVal ScaleFactor_z As System.Double, _    ByVal IsUniform As System.Boolean, _    ByVal ScaleType As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim ScaleFactor_x As System.Double Dim ScaleFactor_y As System.Double Dim ScaleFactor_z As System.Double Dim IsUniform As System.Boolean Dim ScaleType As System.Integer   instance.InsertScale(ScaleFactor_x, ScaleFactor_y, ScaleFactor_z, IsUniform, ScaleType) ``` | |

| C# |  |
| --- | --- |
| ``` void InsertScale(     System.double ScaleFactor_x,    System.double ScaleFactor_y,    System.double ScaleFactor_z,    System.bool IsUniform,    System.int ScaleType ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void InsertScale(  &   System.double ScaleFactor_x, &   System.double ScaleFactor_y, &   System.double ScaleFactor_z, &   System.bool IsUniform, &   System.int ScaleType ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ScaleFactor\_x*

*ScaleFactor\_y*

*ScaleFactor\_z*

*IsUniform*

*ScaleType*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::InsertScale.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)