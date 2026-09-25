<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertUntrimSurface.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertUntrimSurface Method (IFeatureManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertUntrimSurface Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FaceUntrimType*
:   Untrim face as defined in swFaceUntrimType\_e

*EdgeUntrimType*
:   Untrim edge as defined in swEdgeUntrimType\_e

*Distance*
:   Distance by which to untrim surface

*BMerge*
:   True to create a surface extension that merges with the original surface, false to create a new, separate surface body

Inserts an untrimmed surface to patch surface holes and external edges by extending an existing surface along its natural boundaries.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertUntrimSurface( _    ByVal FaceUntrimType As System.Integer, _    ByVal EdgeUntrimType As System.Integer, _    ByVal Distance As System.Double, _    ByVal BMerge As System.Boolean _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim FaceUntrimType As System.Integer Dim EdgeUntrimType As System.Integer Dim Distance As System.Double Dim BMerge As System.Boolean Dim value As Feature   value = instance.InsertUntrimSurface(FaceUntrimType, EdgeUntrimType, Distance, BMerge) ``` | |

| C# |  |
| --- | --- |
| ``` Feature InsertUntrimSurface(     System.int FaceUntrimType,    System.int EdgeUntrimType,    System.double Distance,    System.bool BMerge ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ InsertUntrimSurface(  &   System.int FaceUntrimType, &   System.int EdgeUntrimType, &   System.double Distance, &   System.bool BMerge ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FaceUntrimType*
:   Untrim face as defined in swFaceUntrimType\_e

*EdgeUntrimType*
:   Untrim edge as defined in swEdgeUntrimType\_e

*Distance*
:   Distance by which to untrim surface

*BMerge*
:   True to create a surface extension that merges with the original surface, false to create a new, separate surface body

#### Return Value

Pointer to the [IFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html) object

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertUntrimSurface.

# ![](dotnetimages/collapse.gif)Remarks

You must preselect the face or the edges you want to untrim.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[ISurfaceExtendFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurfaceExtendFeatureData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 SP5, Revision Number 12.5