<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertTableDrivenPattern2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertTableDrivenPattern2 Method (IFeatureManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertTableDrivenPattern2 Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FileName*
:   Name of the file that has the coordinates for the table-driven pattern; can be an empty string (see **Remarks**)

*PointVar*
:   Array of x, y coordinates of the points for the table-driven pattern (see **Remarks**)

*UseCentroid*
:   True to use the centroid of the seed feature, face, or body; false to use a different point as the reference point (see **Remarks**)

*GeomPattern*
:   True to pattern the geometry, false to not

*PropVisProps*
:   True to propagate visual properties, false to not

Obsolete. See [IFeatureManager::CreateFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~CreateFeature.html) and the Remarks in [ITablePatternFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITablePatternFeatureData.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertTableDrivenPattern2( _    ByVal FileName As System.String, _    ByVal PointVar As System.Object, _    ByVal UseCentroid As System.Boolean, _    ByVal GeomPattern As System.Boolean, _    ByVal PropVisProps As System.Boolean _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim FileName As System.String Dim PointVar As System.Object Dim UseCentroid As System.Boolean Dim GeomPattern As System.Boolean Dim PropVisProps As System.Boolean Dim value As Feature   value = instance.InsertTableDrivenPattern2(FileName, PointVar, UseCentroid, GeomPattern, PropVisProps) ``` | |

| C# |  |
| --- | --- |
| ``` Feature InsertTableDrivenPattern2(     System.string FileName,    System.object PointVar,    System.bool UseCentroid,    System.bool GeomPattern,    System.bool PropVisProps ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ InsertTableDrivenPattern2(  &   System.String^ FileName, &   System.Object^ PointVar, &   System.bool UseCentroid, &   System.bool GeomPattern, &   System.bool PropVisProps ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FileName*
:   Name of the file that has the coordinates for the table-driven pattern; can be an empty string (see **Remarks**)

*PointVar*
:   Array of x, y coordinates of the points for the table-driven pattern (see **Remarks**)

*UseCentroid*
:   True to use the centroid of the seed feature, face, or body; false to use a different point as the reference point (see **Remarks**)

*GeomPattern*
:   True to pattern the geometry, false to not

*PropVisProps*
:   True to propagate visual properties, false to not

#### Return Value

[Feature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertTableDrivenPattern2.

# ![](dotnetimages/collapse.gif)Remarks

Specify:

* coordinates for the input points in system units in a **.sldptab** or **.txt** file for FileName.
  - or -* input points in system units in PointVar. Because each point has two coordinates (x, y), the size of PointVar is (2 x number\_of\_points).

This method requires selecting the input entities using these selection marks:

| Input entity | Mark |
| --- | --- |
| Seed feature | 4 |
| Coordinate system | 16 |
| Reference point | 32 |
| Seed face | 128 |
| Seed body | 256 |

If UseCentroid is false, then you must specify a reference point.

See the SOLIDWORKS Help for more information about table-driven patterns.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2017 FCS, Revision Number 25.0