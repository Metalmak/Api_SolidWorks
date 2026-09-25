<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetSpecificFeature2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetSpecificFeature2 Method (IFeature) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeature Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature.html) : GetSpecificFeature2 Method (IFeature) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the more specific interface to a selected feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetSpecificFeature2() As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeature Dim value As System.Object   value = instance.GetSpecificFeature2() ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetSpecificFeature2() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetSpecificFeature2(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

Specific interface (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Feature::GetSpecificFeature2.

# ![](dotnetimages/collapse.gif)Example

[Get Spline Points (C++)](Get_Spline_Points_Example_CPlusPlus_COM.htm)

[Determine if Sketch Suitable for Feature (VBA)](Determine_If_Sketch_Suitable_for_Feature_Example_VB.htm)

[Find Total Length of Sketch Segments in Sketch (VBA)](Find_Total_Length_of_Sketch_Segments_in_Sketch_Example_VB.htm)

[Get Parameters for Reference Axis (VBA)](Get_Parameters_for_Reference_Axis_Example_VB.htm)

[Get Sketch Constraints (VBA)](Get_Sketch_Constraints_Example_VB.htm)

[Insert and Position DXF File in Drawing (VBA)](Insert_and_Position_DXF_File_in_Drawing_Example_VB.htm)

[Insert DXF File and Add Dimension (VBA)](Insert_DXF_File_and_Add_Dimension_Example_VB.htm)

[Insert Reference Points (VBA)](Insert_Reference_Points_Example_VB.htm)

[Get Areas of MidSurface Faces (C#)](Get_Areas_of_MidSurface_Faces_Example_CSharp.htm)

[Get Areas of MidSurface Faces (VB.NET)](Get_Areas_of_MidSurface_FAces_Example_VBNET.htm)

[Get Areas of MidSurface Faces (VBA)](Get_Areas_of_MidSurface_Faces_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method gets these interfaces to a corresponding selected feature:

|  |  |
| --- | --- |
| * [IAttribute](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAttribute.html) * [IBodyFolder](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBodyFolder.html) * [IBomFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBomFeature.html) * [ICamera](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICamera.html) * [ICommentFolder](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICommentFolder.html) * [ICosmeticWeldBeadFolder](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICosmeticWeldBeadFolder.html) * [IDetailCircle](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDetailCircle.html) * [IDrSection](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDrSection.html) * [IFeatureFolder](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureFolder.html) * [IFlatPatternFolder](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFlatPatternFolder.html) * [ILight](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILight.html) * [IMate2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2.html) * [IMateInPlace](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMateInPlace.html) | * [IMateReference](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMateReference.html) * [IMidSurface3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMidSurface3.html) * [IProfileGroupFolder](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IProfileGroupFolder.html) * [IRefAxis](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IRefAxis.html) * [IReferenceCurve](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IReferenceCurve.html) * [IRefPlane](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IRefPlane.html) * [IRefPoint](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IRefPoint.html) * [ISelectionSetFolder](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISelectionSetFolder.html) * [ISensor](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISensor.html)  * [ISheetMetalFolder](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISheetMetalFolder.html) * [ISketch](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch.html) * [ISketchBlockDefinition](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchBlockDefinition.html) * [ISketchBlockInstance](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchBlockInstance.html) * [ISketchPicture](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchPicture.html) * [IStructureSystemFolder](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemFolder.html) * [IWeldmentCutListFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IWeldmentCutListFeature.html) |

| **If...** | **Then...** |
| --- | --- |
| You start with an IFeature object and want to get a more specific object | A call to IFeature::GetSpecificFeature2 is required. If you have the more specific object, then a call to QueryInterface in C++ or an assignment to a IFeature-typed variable allows an application to get back to the IFeature object. |
| You are writing a Dispatch application | You can use [IFeature::GetTypeName](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~GetTypeName.html) or [IFeature::GetTypeName2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetTypeName2.html) to identify the type of Dispatch object returned so that you can call the appropriate properties and methods for that object. |
| You are writing a COM application | You can use the return value with QueryInterface to determine the object returned. |
| No interface exists or there is no specific object for the type of feature | This method returns Nothing or null. |

For some feature types, this method returns Nothing or null because there is no specific object for that type of feature (e.g., features such as extrusions, lofts, fillets, chamfers, etc.). For these types of features, call [IFeature::GetDefinition](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetDefinition.html) to get their feature data objects.

For other entities selected in the FeatureManager design tree, you must know its interface in advance and cast the return value of [ISelectionMgr::GetSelectedObject6](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISelectionMgr~GetSelectedObject6.html) to the correct interface.

For all functions that return objects, always check whether the return value is Nothing or null before you try to use it.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeature Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature.html)

[IFeature Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12.0