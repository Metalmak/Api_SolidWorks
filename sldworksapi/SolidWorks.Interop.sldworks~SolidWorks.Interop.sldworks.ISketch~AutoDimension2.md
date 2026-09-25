<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~AutoDimension2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AutoDimension2 Method (ISketch) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketch Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch.html) : AutoDimension2 Method (ISketch) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*EntitiesToDimension*
:   Entities to dimension as defined in swAutodimEntities\_e

*HorizontalScheme*
:   Horizontal dimensioning scheme as defined in swAutodimScheme\_e

*HorizontalPlacement*
:   Placement relative to the sketch as defined in swAutodimHorizontalPlacement\_e

*VerticalScheme*
:   Vertical dimensioning scheme as defined in swAutodimScheme\_e

*VerticalPlacement*
:   Placement relative to the sketch as defined in swAutodimVerticalPlacement\_e

Obsolete. Superseded by [ISketchManager::FullyDefineSketch](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchManager~FullyDefineSketch.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AutoDimension2( _    ByVal EntitiesToDimension As System.Integer, _    ByVal HorizontalScheme As System.Integer, _    ByVal HorizontalPlacement As System.Integer, _    ByVal VerticalScheme As System.Integer, _    ByVal VerticalPlacement As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketch Dim EntitiesToDimension As System.Integer Dim HorizontalScheme As System.Integer Dim HorizontalPlacement As System.Integer Dim VerticalScheme As System.Integer Dim VerticalPlacement As System.Integer Dim value As System.Integer   value = instance.AutoDimension2(EntitiesToDimension, HorizontalScheme, HorizontalPlacement, VerticalScheme, VerticalPlacement) ``` | |

| C# |  |
| --- | --- |
| ``` System.int AutoDimension2(     System.int EntitiesToDimension,    System.int HorizontalScheme,    System.int HorizontalPlacement,    System.int VerticalScheme,    System.int VerticalPlacement ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int AutoDimension2(  &   System.int EntitiesToDimension, &   System.int HorizontalScheme, &   System.int HorizontalPlacement, &   System.int VerticalScheme, &   System.int VerticalPlacement ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*EntitiesToDimension*
:   Entities to dimension as defined in swAutodimEntities\_e

*HorizontalScheme*
:   Horizontal dimensioning scheme as defined in swAutodimScheme\_e

*HorizontalPlacement*
:   Placement relative to the sketch as defined in swAutodimHorizontalPlacement\_e

*VerticalScheme*
:   Vertical dimensioning scheme as defined in swAutodimScheme\_e

*VerticalPlacement*
:   Placement relative to the sketch as defined in swAutodimVerticalPlacement\_e

#### Return Value

swAutodimStatusSuccess if the sketch is automatically dimensioned successfully; see swAutodimStatus\_e for values for reasons for possible failures

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Sketch::AutoDimension2.

# ![](dotnetimages/collapse.gif)Example

[Autodimension a Sketch (VBA)](Autodimension_a_Sketch_Example_VB.htm)

[Insert DXF File and Add Dimension (VBA)](Insert_DXF_File_and_Add_Dimension_Example_VB.htm)

[Autodimension All Sketches (C#)](Autodimension_All_Sketches_Example_CSharp.htm)

[Autodimension All Sketches (VB.NET)](Autodimension_All_Sketches_Example_VBNET.htm)

[Autodimension all Sketches (VBA)](Autodimension_All_Sketches_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

If the EntitiesToDimension argument takes the value swAutodimEntitiesSelected, then use [IModelDocExtension::SelectByID2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SelectByID2.html) with a mark value of swAutodimMarkEntities to select the sketch entities to dimension.

You can supply datums for horizontal and vertical dimensioning schemes. Select and mark a unique vertical edge, vertex, sketch point, or vertical sketch line as the datum for the horizontal dimensioning scheme, using swAutodimMarkHorizontalDatum as the mark value. Similarly, select a unique horizontal edge, vertex, sketch point, or horizontal sketch line as the datum for the vertical dimensioning scheme, using swAutodimMarkVerticalDatum as the mark value. It is an error to supply just one datum as indicated by the status value swAutodimStatus\_DatumNotSupplied.

# ![](dotnetimages/collapse.gif)See Also

####

[ISketch Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch.html)

[ISketch Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12.0