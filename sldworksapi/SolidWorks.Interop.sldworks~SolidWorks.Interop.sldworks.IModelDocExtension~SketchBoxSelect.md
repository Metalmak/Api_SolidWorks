<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~SketchBoxSelect.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SketchBoxSelect Method (IModelDocExtension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : SketchBoxSelect Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FirstPtX*
:   x coordinate of the first corner of the box

*FirstPtY*
:   y coordinate of the first corner of the box

*FirstPtZ*
:   z coordinate of the first corner of the box

*SecondPtX*
:   x coordinate of the opposite diagonal corner of the box

*SecondPtY*
:   y coordinate of the opposite diagonal corner of the box

*SecondPtZ*
:   z coordinate of the opposite diagonal corner of the box

Box selects all of the entities in a sketch within the specified coordinates of the selection box.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SketchBoxSelect( _    ByVal FirstPtX As System.Double, _    ByVal FirstPtY As System.Double, _    ByVal FirstPtZ As System.Double, _    ByVal SecondPtX As System.Double, _    ByVal SecondPtY As System.Double, _    ByVal SecondPtZ As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim FirstPtX As System.Double Dim FirstPtY As System.Double Dim FirstPtZ As System.Double Dim SecondPtX As System.Double Dim SecondPtY As System.Double Dim SecondPtZ As System.Double Dim value As System.Boolean   value = instance.SketchBoxSelect(FirstPtX, FirstPtY, FirstPtZ, SecondPtX, SecondPtY, SecondPtZ) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SketchBoxSelect(     System.double FirstPtX,    System.double FirstPtY,    System.double FirstPtZ,    System.double SecondPtX,    System.double SecondPtY,    System.double SecondPtZ ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SketchBoxSelect(  &   System.double FirstPtX, &   System.double FirstPtY, &   System.double FirstPtZ, &   System.double SecondPtX, &   System.double SecondPtY, &   System.double SecondPtZ ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FirstPtX*
:   x coordinate of the first corner of the box

*FirstPtY*
:   y coordinate of the first corner of the box

*FirstPtZ*
:   z coordinate of the first corner of the box

*SecondPtX*
:   x coordinate of the opposite diagonal corner of the box

*SecondPtY*
:   y coordinate of the opposite diagonal corner of the box

*SecondPtZ*
:   z coordinate of the opposite diagonal corner of the box

#### Return Value

True if the sketch entities lying in the specified coordinates are box-selected, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::SketchBoxSelect.

# ![](dotnetimages/collapse.gif)Example

[Box Select a Sketch (VB.NET)](Box_Select_a_Sketch_Example_VBNET.htm)

[Box Select a Sketch (VBA)](Box_Select_a_Sketch_Example_VB.htm)

[Box Select a Sketch (C#)](Box_Select_a_Sketch_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0