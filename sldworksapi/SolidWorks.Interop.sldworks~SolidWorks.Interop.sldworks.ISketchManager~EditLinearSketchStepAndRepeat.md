<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~EditLinearSketchStepAndRepeat.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| EditLinearSketchStepAndRepeat Method (ISketchManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html) : EditLinearSketchStepAndRepeat Method (ISketchManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NumX*
:   Total number of instances along the x axis, including the seed

*NumY*
:   Total number of instances along the y axis, including the seed

*SpacingX*
:   Spacing between instances along the x axis

*SpacingY*
:   Spacing between instances along the y axis

*AngleX*
:   Angle for direction 1 relative to the x axis

*AngleY*
:   Angle for direction 2 relative to the y axis

*DeleteInstances*
:   Number of instances to delete, passed as a string in the format: "(a) (b) (c) "

*XSpacingDim*
:   True to display the spacing between instances dimension along the x axis in the graphics area, false to not

*YSpacingDim*
:   True to display the spacing between instances dimension along the y axis in the graphics area, false to not

*AngleDim*
:   True to display the angle dimension between axes in the graphics area, false to not

*CreateNumOfInstancesDimInXDir*
:   True to display the number of instances in the x direction dimension in the graphics area, false to not

*CreateNumOfInstancesDimInYDir*
:   True to display the number of instances in the y direction dimension in the graphics area, false to not

*Seeds*
:   Array of the names of the entities, separated by the underscore character (\_), that comprise the seed pattern (e.g., Line1\_Line2\_Line3\_Line4 for a rectangular-shaped seed pattern)

Edits a linear sketch pattern.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function EditLinearSketchStepAndRepeat( _    ByVal NumX As System.Integer, _    ByVal NumY As System.Integer, _    ByVal SpacingX As System.Double, _    ByVal SpacingY As System.Double, _    ByVal AngleX As System.Double, _    ByVal AngleY As System.Double, _    ByVal DeleteInstances As System.String, _    ByVal XSpacingDim As System.Boolean, _    ByVal YSpacingDim As System.Boolean, _    ByVal AngleDim As System.Boolean, _    ByVal CreateNumOfInstancesDimInXDir As System.Boolean, _    ByVal CreateNumOfInstancesDimInYDir As System.Boolean, _    ByVal Seeds As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchManager Dim NumX As System.Integer Dim NumY As System.Integer Dim SpacingX As System.Double Dim SpacingY As System.Double Dim AngleX As System.Double Dim AngleY As System.Double Dim DeleteInstances As System.String Dim XSpacingDim As System.Boolean Dim YSpacingDim As System.Boolean Dim AngleDim As System.Boolean Dim CreateNumOfInstancesDimInXDir As System.Boolean Dim CreateNumOfInstancesDimInYDir As System.Boolean Dim Seeds As System.String Dim value As System.Boolean   value = instance.EditLinearSketchStepAndRepeat(NumX, NumY, SpacingX, SpacingY, AngleX, AngleY, DeleteInstances, XSpacingDim, YSpacingDim, AngleDim, CreateNumOfInstancesDimInXDir, CreateNumOfInstancesDimInYDir, Seeds) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool EditLinearSketchStepAndRepeat(     System.int NumX,    System.int NumY,    System.double SpacingX,    System.double SpacingY,    System.double AngleX,    System.double AngleY,    System.string DeleteInstances,    System.bool XSpacingDim,    System.bool YSpacingDim,    System.bool AngleDim,    System.bool CreateNumOfInstancesDimInXDir,    System.bool CreateNumOfInstancesDimInYDir,    System.string Seeds ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool EditLinearSketchStepAndRepeat(  &   System.int NumX, &   System.int NumY, &   System.double SpacingX, &   System.double SpacingY, &   System.double AngleX, &   System.double AngleY, &   System.String^ DeleteInstances, &   System.bool XSpacingDim, &   System.bool YSpacingDim, &   System.bool AngleDim, &   System.bool CreateNumOfInstancesDimInXDir, &   System.bool CreateNumOfInstancesDimInYDir, &   System.String^ Seeds ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*NumX*
:   Total number of instances along the x axis, including the seed

*NumY*
:   Total number of instances along the y axis, including the seed

*SpacingX*
:   Spacing between instances along the x axis

*SpacingY*
:   Spacing between instances along the y axis

*AngleX*
:   Angle for direction 1 relative to the x axis

*AngleY*
:   Angle for direction 2 relative to the y axis

*DeleteInstances*
:   Number of instances to delete, passed as a string in the format: "(a) (b) (c) "

*XSpacingDim*
:   True to display the spacing between instances dimension along the x axis in the graphics area, false to not

*YSpacingDim*
:   True to display the spacing between instances dimension along the y axis in the graphics area, false to not

*AngleDim*
:   True to display the angle dimension between axes in the graphics area, false to not

*CreateNumOfInstancesDimInXDir*
:   True to display the number of instances in the x direction dimension in the graphics area, false to not

*CreateNumOfInstancesDimInYDir*
:   True to display the number of instances in the y direction dimension in the graphics area, false to not

*Seeds*
:   Array of the names of the entities, separated by the underscore character (\_), that comprise the seed pattern (e.g., Line1\_Line2\_Line3\_Line4 for a rectangular-shaped seed pattern)

#### Return Value

True if the linear sketch pattern is edited, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SketchManager::EditLinearSketchStepAndRepeat.

# ![](dotnetimages/collapse.gif)Example

[Create and Edit Linear Sketch Pattern (VB.NET)](Create_and_Edit_Linear_Sketch_Pattern_Example_VBNET.htm)

[Create and Edit Linear Sketch Pattern (VBA)](Create_and_Edit_Linear_Sketch_Pattern_Example_VB.htm)

[Create and Edit Linear Sketch Pattern (C#)](Create_and_Edit_Linear_Sketch_Pattern_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

The spacing instances, angle, and number of instances dimensions displayed in the graphics area can be modified by interactive users

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html)

[ISketchManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager_members.html)

[ISketchManager::CreateLinearSketchStepAndRepeat Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreateLinearSketchStepAndRepeat.html)

[ISketchManager::CreateCircularSketchStepAndRepeat Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreateCircularSketchStepAndRepeat.html)

[ISketchManager::EditCircularSketchStepAndRepeat Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~EditCircularSketchStepAndRepeat.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0