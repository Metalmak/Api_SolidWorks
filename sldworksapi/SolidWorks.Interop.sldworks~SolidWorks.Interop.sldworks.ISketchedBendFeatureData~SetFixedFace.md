<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchedBendFeatureData~SetFixedFace.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetFixedFace Method (ISketchedBendFeatureData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchedBendFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchedBendFeatureData.html) : SetFixedFace Method (ISketchedBendFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*X*
:   X location

*Y*
:   Y location

*Z*
:   Z location

*EdgeArray*
:   Array of edges

Sets the fixed face of this sketched bend feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetFixedFace( _    ByVal X As System.Double, _    ByVal Y As System.Double, _    ByVal Z As System.Double, _    ByVal EdgeArray As System.Object _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchedBendFeatureData Dim X As System.Double Dim Y As System.Double Dim Z As System.Double Dim EdgeArray As System.Object   instance.SetFixedFace(X, Y, Z, EdgeArray) ``` | |

| C# |  |
| --- | --- |
| ``` void SetFixedFace(     System.double X,    System.double Y,    System.double Z,    System.object EdgeArray ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetFixedFace(  &   System.double X, &   System.double Y, &   System.double Z, &   System.Object^ EdgeArray ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*X*
:   X location

*Y*
:   Y location

*Z*
:   Z location

*EdgeArray*
:   Array of edges

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SketchedBendFeatureData::SetFixedFace.

# ![](dotnetimages/collapse.gif)Remarks

See Accessing Selections that Define Features for additional details.

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchedBendFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchedBendFeatureData.html)

[ISketchedBendFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchedBendFeatureData_members.html)

[ISketchedBendFeatureData::GetFixedFace Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchedBendFeatureData~GetFixedFace.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001 SP2, Revision Number 9.2