<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRackPinionMateFeatureData~EntitiesToMate.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| EntitiesToMate Property (IRackPinionMateFeatureData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IRackPinionMateFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRackPinionMateFeatureData.html) : EntitiesToMate Property (IRackPinionMateFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*EntityType*
:   Entity type to mate as defined in swRackPinionMateEntityType\_e

Gets or sets the entities to mate in this rack and pinion mate feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property EntitiesToMate( _    ByVal EntityType As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IRackPinionMateFeatureData Dim EntityType As System.Integer Dim value As System.Object   instance.EntitiesToMate(EntityType) = value   value = instance.EntitiesToMate(EntityType) ``` | |

| C# |  |
| --- | --- |
| ``` System.object EntitiesToMate(     System.int EntityType ) {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.Object^ EntitiesToMate {    System.Object^ get(System.int EntityType);    void set (System.int EntityType, System.Object^ value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*EntityType*
:   Entity type to mate as defined in swRackPinionMateEntityType\_e

#### Property Value

Array of entities to mate (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See RackPinionMateFeatureData::EntitiesToMate.

# ![](dotnetimages/collapse.gif)Remarks

If EntityType is set to swRackPinionMateEntityType\_e.:

* swRackPinionMateEntityType\_Pinion, then set the array with a a cylindrical [face](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2.html), circular [edge](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge.html) or [arc](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchArc.html), sketch circle, [axis](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefAxis.html), or revolved [surface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface.html).* swRackPinionMateEntityType\_Rack, then set the array with a linear edge, [sketch line](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchLine.html), [centerline](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICenterLine.html), axis, or cylindrical face.

Instead of specifying this property, you can use [IModelDocExtension::SelectByID2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~SelectByID2.html) to pre-select the entities to mate using Mark = 64 for the rack and Mark = 128 for the pinion. You can pre-select mate entities during mate creation, but not during mate editing.

# ![](dotnetimages/collapse.gif)See Also

####

[IRackPinionMateFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRackPinionMateFeatureData.html)

[IRackPinionMateFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRackPinionMateFeatureData_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2019 FCS, Revision Number 27.0