<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc~FeatureByName.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| FeatureByName Method (IPartDoc) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPartDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc.html) : FeatureByName Method (IPartDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Name*
:   Name of feature

Gets the named feature in the part.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function FeatureByName( _    ByVal Name As System.String _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPartDoc Dim Name As System.String Dim value As System.Object   value = instance.FeatureByName(Name) ``` | |

| C# |  |
| --- | --- |
| ``` System.object FeatureByName(     System.string Name ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ FeatureByName(  &   System.String^ Name ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Name*
:   Name of feature

#### Return Value

[Feature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PartDoc::FeatureByName.

# ![](dotnetimages/collapse.gif)Example

[Autodimension All Sketches (VBA)](Autodimension_All_Sketches_Example_VB.htm)

[Get and Set Constraint for Dome Feature (VBA)](Get_and_Set_Constraint_for_Dome_Feature_Example_VB.htm)

[Move Copy Sketch Entities (C#)](Move_Copy_Sketch_Entities_Example_CSharp.htm)

[Move Copy Sketch Entities (VB.NET)](Move_Copy_Sketch_Entities_Example_VBNET.htm)

[Move Copy Sketch Entities (VBA)](Move_Copy_Sketch_Entities_Example_VB.htm)

[Roll Back Model (C#)](Roll_Back_Model_Example_CSharp.htm)

[Roll Back Model (VB.NET)](Roll_Back_Model_Example_VBNET.htm)

[Roll Back Model (VBA)](Roll_Back_Model_Example_VB.htm)

[Suppress Component Feature (C#)](Suppress_Component_Feature_Example_CSharp.htm)

[Suppress Component Feature (VB.NET)](Suppress_Component_Feature_Example_VBNET.htm)

[Suppress Component Feature (VBA)](Suppress_Component_Feature_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IPartDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc.html)

[IPartDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc_members.html)

[IPartDoc::IFeatureByName Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc~IFeatureByName.html)

[IPartDoc::IFeatureById Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc~IFeatureById.html)

[IPartDoc::FeatureById Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc~FeatureById.html)

[IAssemblyDoc::FeatureByName Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~FeatureByName.html)

[IAssemblyDoc::IFeatureByName Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~IFeatureByName.html)

[IComponent2::FeatureByName Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~FeatureByName.html)

[IDrawingDoc::FeatureByName Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~FeatureByName.html)

[IDrawingDoc::IFeatureByName Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~IFeatureByName.html)