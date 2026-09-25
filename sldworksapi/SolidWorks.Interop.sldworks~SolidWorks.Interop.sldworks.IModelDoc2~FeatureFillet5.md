<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~FeatureFillet5.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| FeatureFillet5 Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : FeatureFillet5 Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Options*

*R1*

*Ftyp*

*OverflowType*

*Radii*

*SetBackDistances*

*PointRadiusArray*

Obsolete. Superseded by [IFeatureManager::FeatureFillet](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~FeatureFillet.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function FeatureFillet5( _    ByVal Options As System.Integer, _    ByVal R1 As System.Double, _    ByVal Ftyp As System.Integer, _    ByVal OverflowType As System.Integer, _    ByVal Radii As System.Object, _    ByVal SetBackDistances As System.Object, _    ByVal PointRadiusArray As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim Options As System.Integer Dim R1 As System.Double Dim Ftyp As System.Integer Dim OverflowType As System.Integer Dim Radii As System.Object Dim SetBackDistances As System.Object Dim PointRadiusArray As System.Object Dim value As System.Integer   value = instance.FeatureFillet5(Options, R1, Ftyp, OverflowType, Radii, SetBackDistances, PointRadiusArray) ``` | |

| C# |  |
| --- | --- |
| ``` System.int FeatureFillet5(     System.int Options,    System.double R1,    System.int Ftyp,    System.int OverflowType,    System.object Radii,    System.object SetBackDistances,    System.object PointRadiusArray ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int FeatureFillet5(  &   System.int Options, &   System.double R1, &   System.int Ftyp, &   System.int OverflowType, &   System.Object^ Radii, &   System.Object^ SetBackDistances, &   System.Object^ PointRadiusArray ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Options*

*R1*

*Ftyp*

*OverflowType*

*Radii*

*SetBackDistances*

*PointRadiusArray*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::FeatureFillet5.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)