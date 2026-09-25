<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~AutoDimension.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AutoDimension Method (IDrawingDoc) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html) : AutoDimension Method (IDrawingDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*EntitiesToDimension*
:   Entities to dimension as defined in swAutodimEntities\_e

*HorizontalScheme*
:   Horizontal dimensioning scheme as defined in swAutodimScheme\_e

*HorizontalPlacement*
:   Placement relative to the drawing view as defined in swAutodimHorizontalPlacement\_e

*VerticalScheme*
:   Vertical dimensioning scheme as defined in swAutodimScheme\_e

*VerticalPlacement*
:   Placement relative to the drawing view as defined in swAutodimVerticalPlacement\_e

Automatically dimensions the selected drawing view.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AutoDimension( _    ByVal EntitiesToDimension As System.Integer, _    ByVal HorizontalScheme As System.Integer, _    ByVal HorizontalPlacement As System.Integer, _    ByVal VerticalScheme As System.Integer, _    ByVal VerticalPlacement As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDrawingDoc Dim EntitiesToDimension As System.Integer Dim HorizontalScheme As System.Integer Dim HorizontalPlacement As System.Integer Dim VerticalScheme As System.Integer Dim VerticalPlacement As System.Integer Dim value As System.Integer   value = instance.AutoDimension(EntitiesToDimension, HorizontalScheme, HorizontalPlacement, VerticalScheme, VerticalPlacement) ``` | |

| C# |  |
| --- | --- |
| ``` System.int AutoDimension(     System.int EntitiesToDimension,    System.int HorizontalScheme,    System.int HorizontalPlacement,    System.int VerticalScheme,    System.int VerticalPlacement ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int AutoDimension(  &   System.int EntitiesToDimension, &   System.int HorizontalScheme, &   System.int HorizontalPlacement, &   System.int VerticalScheme, &   System.int VerticalPlacement ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*EntitiesToDimension*
:   Entities to dimension as defined in swAutodimEntities\_e

*HorizontalScheme*
:   Horizontal dimensioning scheme as defined in swAutodimScheme\_e

*HorizontalPlacement*
:   Placement relative to the drawing view as defined in swAutodimHorizontalPlacement\_e

*VerticalScheme*
:   Vertical dimensioning scheme as defined in swAutodimScheme\_e

*VerticalPlacement*
:   Placement relative to the drawing view as defined in swAutodimVerticalPlacement\_e

#### Return Value

swAutodimStatusSuccess if the view is automatically dimensioned; see swAutodimStatus\_e for reasons for possible failures

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DrawingDoc::AutoDimension.

# ![](dotnetimages/collapse.gif)Example

[Autodimension Selected Drawing View (C#)](Autodimension_Selected_Drawing_View_Example_CSharp.htm)

[Autodimension Selected Drawing View (VB.NET)](Autodimension_Selected_Drawing_View_Example_VBNET.htm)

[Autodimension Selected Drawing View (VBA)](Autodimension_Selected_Drawing_View_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method requires information about the:

* drawing view to autodimension. This information can be supplied by selecting the drawing view to use. No mark is necessary.

  If a drawing view is not selected, then this method attempts to determine the drawing view information from the other entities that are selected. If no other selections exist, then this method defaults to using the first drawing view, which is consistent with how the SOLIDWORKS user interface works.

  * datums to use for the dimensioning baseline. These can be supplied by selecting a vertical edge, vertical sketch line, vertex, or sketch point as the datum for the horizontal dimensioning scheme. Mark the selection with swAutodimMarkHorizontalDatum from swAutodimMark\_e. Similarly a horizontal edge, horizontal sketch line, vertex, or sketch point should be selected and marked with swAutodimMark\_e.swAutodimMarkVerticalDatum for defining the datum for the vertical dimensioning scheme. If only one of these datums is supplied, only the appropriate dimensions are created for that datum.

    Instead of selecting the horizontal and vertical datum separately, you can select a vertex or sketch point to use to define both datums. Mark the selected vertex or sketch point selection with swAutodimMark\_e.swAutodimMarkOriginDatum. If no datums are selected, then this method automatically uses the left- and bottom-most entities in the view to determine default datums, which is consistent with how the SOLIDWORKS user interface works.

    * entities to autodimension. This information is supplied by the entitiesToDimension argument and the selected entities marked with swAutodimMark\_e.swAutodimMarkEntities. The entitiesToDimension argument takes a value from the swAutodimEntities\_e enumeration:

      + swAutodimEntitiesSelected indicates that only selected entities marked with a value of swAutodimMarkEntities are considered for autodimensioning.

        + swAutodimEntitiesAll indicates that all entities in the drawing view are autodimensioned.

          + swAutodimEntitiesBasedOnPreselect indicates that SOLIDWORKS figures out what to do based on the selected entities marked with swAutodimMarkEntities. If any exist, then autodimension them, just like swAutodimEntitiesSelected. If none exist, then autodimension all entities, just like swAutodimEntitiesAll.

            Supported entities for dimensioning are lines, points, vertices, faces, and sketch entities.

# ![](dotnetimages/collapse.gif)See Also

####

[IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html)

[IDrawingDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc_members.html)

[IDrawingDoc:AddChamferDim Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~AddChamferDim.html)

[IDrawingDoc:CreateAngDim4 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~CreateAngDim4.html)

[IDrawingDoc:CreateDiamDim4 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~CreateDiamDim4.html)

[IDrawingDoc:CreateLinearDim4 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~CreateLinearDim4.html)

[IDrawingDoc:CreateOrdinateDim4 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~CreateOrdinateDim4.html)

[IDrawingDoc:Dimensions Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~Dimensions.html)

[IDrawingDoc:DragModelDimension Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~DragModelDimension.html)

[IDrawingDoc:HideShowDimensions Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~HideShowDimensions.html)

[IDrawingDoc:IAddChamferDim Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~IAddChamferDim.html)

[IDrawingDoc:ICreateAngDim4 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~ICreateAngDim4.html)

[IDrawingDoc:ICreateDiamDim4 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~ICreateDiamDim4.html)

[IDrawingDoc:ICreateLinearDim4 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~ICreateLinearDim4.html)

[IDrawingDoc:ICreateOrdinateDim4 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~ICreateOrdinateDim4.html)

[IDrawingDoc:InsertBaseDim Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~InsertBaseDim.html)

[IDrawingDoc:InsertHorizontalOrdinate Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~InsertHorizontalOrdinate.html)

[IDrawingDoc:InsertModelAnnotations3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~InsertModelAnnotations3.html)

[IDrawingDoc:InsertModelDimensions Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~InsertModelDimensions.html)

[IDrawingDoc:InsertOrdinate Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~InsertOrdinate.html)

[IDrawingDoc:InsertRefDim Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~InsertRefDim.html)

[IDrawingDoc:InsertVerticalOrdinate Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~InsertVerticalOrdinate.html)

[IDrawingDoc::SketchDim Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~SketchDim.html)

[IDisplayDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2005 FCS, Revision Number 13.0