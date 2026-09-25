<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertSlicing.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertSlicing Method (IFeatureManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertSlicing Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SlicingData*
:   [ISlicingData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISlicingData.html) (see **Remarks**)

*Errors*
:   Errors as defined in swInsertSlicingError\_e

Creates and inserts slicing into the FeatureManager design tree.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertSlicing( _    ByVal SlicingData As System.Object, _    ByRef Errors As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim SlicingData As System.Object Dim Errors As System.Integer Dim value As System.Object   value = instance.InsertSlicing(SlicingData, Errors) ``` | |

| C# |  |
| --- | --- |
| ``` System.object InsertSlicing(     System.object SlicingData,    out System.int Errors ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ InsertSlicing(  &   System.Object^ SlicingData, &   [Out] System.int Errors ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*SlicingData*
:   [ISlicingData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISlicingData.html) (see **Remarks**)

*Errors*
:   Errors as defined in swInsertSlicingError\_e

#### Return Value

Array of sketch and reference plane objects

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertSlicing.

# ![](dotnetimages/collapse.gif)Example

See the [ISlicingData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISlicingData.html) example.

# ![](dotnetimages/collapse.gif)Remarks

This method invokes the Slicing tool. For more information, refer to **SOLIDWORKS Help > Parts and Features > Controlling Parts > Slicing Tool**.

Before calling this method:

1. Pre-select in the graphics area a planar entity (to create a linear pattern of slices) or a combination of a linear entity and a point entity (to create an angular pattern of slices whose axis is the linear entity).- Use [IFeatureManager::GetSlicingData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~GetSlicingData.html) to get an ISlicingData object.- Set [ISlicingData::PlaneReferences](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISlicingData~PlaneReferences.html) if step 1 is not performed. Specify a planar entity or a combination of a linear entity and a point entity as specified in step 1.- Set other ISlicingData properties.- Populate SlicingData with the ISlicingData object.

After calling this method:

* Use the array of sketch and reference plane objects returned by this method to perform further work.* If [ISlicingData::AddSlicingPlanesAndSketchesToFolder](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISlicingData~AddSlicingPlanesAndSketchesToFolder.html) was set to true, then a **Slice1** folder in the FeatureManager design tree is created containing the slicing planes and sketches. You can edit the slicing planes and sketches individually as needed.* Delete the Slice1 folder and its contents to remove slicing from the model.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2020 FCS, Revision Number 28.0