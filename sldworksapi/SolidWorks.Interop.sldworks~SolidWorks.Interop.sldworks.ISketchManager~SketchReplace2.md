<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~SketchReplace2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SketchReplace2 Method (ISketchManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html) : SketchReplace2 Method (ISketchManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*MakeConstruction*
:   True to convert the replaced sketch entity to construction geometry, false to delete it

*MakeContour*
:   True to make the replacement sketch entity a contour, false to not

Replaces a sketch entity in a model with another sketch entity, preserving all references.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SketchReplace2( _    ByVal MakeConstruction As System.Boolean, _    ByVal MakeContour As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchManager Dim MakeConstruction As System.Boolean Dim MakeContour As System.Boolean Dim value As System.Boolean   value = instance.SketchReplace2(MakeConstruction, MakeContour) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SketchReplace2(     System.bool MakeConstruction,    System.bool MakeContour ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SketchReplace2(  &   System.bool MakeConstruction, &   System.bool MakeContour ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*MakeConstruction*
:   True to convert the replaced sketch entity to construction geometry, false to delete it

*MakeContour*
:   True to make the replacement sketch entity a contour, false to not

#### Return Value

True if the the sketch entity is successfully replaced, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SketchManager::SketchReplace2.

# ![](dotnetimages/collapse.gif)Example

[Replace Sketch Entity (VBA)](Replace_Sketch_Example_VB.htm)

[Replace Sketch Entity (VB.NET)](Replace_Sketch_Example_VBNET.htm)

[Replace Sketch Entity (C#)](Replace_Sketch_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, call [IModelDocExtension::SelectByID2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SelectByID2.html) with Append set to true to select each of the following entities:

1. Sketch entity to be replaced.- Replacement sketch entity that does not reference downstream geometry or have references outside of the sketch.

After calling this method, call [ISketchManager::InsertSketch](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchManager~InsertSketch.html) to rebuild the model with the replacement sketch.

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html)

[ISketchManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2022 FCS, Revision Number 30