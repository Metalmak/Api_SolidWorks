<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertTableDrivenPattern.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertTableDrivenPattern Method (IFeatureManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertTableDrivenPattern Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FileName*
:   Name of the file that has the coordinates information; can be an empty string (see **Remarks**)

*PointVar*
:   Array of x, y coordinates of the points (see **Remarks**)

*UseCentrod*
:   True to use the centroid of the seed feature, face, or body; false to use another point as the reference point (see **Remarks**)

*GeomPatt*
:   True to pattern the geometry, false to not

Obsolete. Superseded by [IFeatureManager::InsertTableDrivenPattern2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertTableDrivenPattern2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertTableDrivenPattern( _    ByVal FileName As System.String, _    ByVal PointVar As System.Object, _    ByVal UseCentrod As System.Boolean, _    ByVal GeomPatt As System.Boolean _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim FileName As System.String Dim PointVar As System.Object Dim UseCentrod As System.Boolean Dim GeomPatt As System.Boolean Dim value As Feature   value = instance.InsertTableDrivenPattern(FileName, PointVar, UseCentrod, GeomPatt) ``` | |

| C# |  |
| --- | --- |
| ``` Feature InsertTableDrivenPattern(     System.string FileName,    System.object PointVar,    System.bool UseCentrod,    System.bool GeomPatt ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ InsertTableDrivenPattern(  &   System.String^ FileName, &   System.Object^ PointVar, &   System.bool UseCentrod, &   System.bool GeomPatt ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FileName*
:   Name of the file that has the coordinates information; can be an empty string (see **Remarks**)

*PointVar*
:   Array of x, y coordinates of the points (see **Remarks**)

*UseCentrod*
:   True to use the centroid of the seed feature, face, or body; false to use another point as the reference point (see **Remarks**)

*GeomPatt*
:   True to pattern the geometry, false to not

#### Return Value

[Feature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertTableDrivenPattern.

# ![](dotnetimages/collapse.gif)Remarks

Specify:

* coordinates for the input points in system units in a **.sldptab** or **.txt** file for FileName.
  - or -* input points in system units in PointVar. Because each point has two coordinates (x, y), the size of PointVar is (2 x number\_of\_points).

This method requires selecting the input entities using these selection marks:

* 4 = Seed feature

  * 16 = Coordinate system

    * 32 = Reference point

      * 128 = Seed face

        * 256 = Seed body

If UseCentrod is false, then you must specify a reference point.

See the SOLIDWORKS Help for more information about table-driven patterns.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[ITablePatternFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITablePatternFeatureData.html)

[IFeatureManager::IInsertTableDrivenPattern Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~IInsertTableDrivenPattern.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2003 FCS, Revision Number 11.0