<!-- source: sldworksapi/Add_Ordinate_Dimension_Example_VB.htm -->

# SOLIDWORKS API Help

# Add Ordinate Dimension Example (VBA)

This example shows how to add an ordinate dimension.

'------------------------------------------

' Preconditions:

'          1)
Drawing document is open.

'          2)
Two horizontal parallel edges are selected.

'

' Postconditions: Ordinate dimension added.

'-------------------------------------------

Option Explicit

Public Enum swAddOrdinateDims\_e

    swOrdinate
= 1

    swVerticalOrdinate
= 2

    swHorizontalOrdinate
= 3

End Enum

Public Enum swCreateOrdDimError\_e

    swCreateOrdDimErr\_Undefined
= -1            '
 If encountered,
report as SPR.

    swCreateOrdDimErr\_Success
= 0

    swCreateOrdDimErr\_GenFailure
= 1            '
 MSG\_SDIM\_BAD\_DIM

    swCreateOrdDimErr\_GenNoInternalDims
= 2     '
 MSG\_NO\_INTERNAL\_DIMS\_IN\_DSKETCH

    swCreateOrdDimErr\_GenBadSel
= 3             '
 MSG\_DIM\_REF\_NOCREATE

    swCreateOrdDimErr\_GenNeedModelLoaded
= 4    '
 MSG\_CANNOT\_DIM\_GHOST\_IN3D

    swCreateOrdDimErr\_GenSamePartOnly
= 5       '
 MSG\_DIM\_EDIT\_PART

    swCreateOrdDimErr\_GenExtraSelection
= 6     '
 MSG\_DIM\_TOO\_MANY\_SELECT

    swCreateOrdDimErr\_OrdFailure
= 7            '
 MSG\_BAD\_ORDINATE\_DIM0

    swCreateOrdDimErr\_OrdDupInGroup
= 8         '
 MSG\_BAD\_ORDINATE\_DIM1

    swCreateOrdDimErr\_OrdBadDir
= 9             '
 MSG\_BAD\_ORDINATE\_DIM2

End Enum

Sub main()

    Dim
swApp                   As
SldWorks.SldWorks

    Dim
swModel                 As
SldWorks.modelDoc

    Dim
swDraw                  As
SldWorks.DrawingDoc

    Dim
nRetval                 As
Long

    Set
swApp = Application.SldWorks

    Set
swModel = swApp.ActiveDoc

    Set
swDraw = swModel

    '
Horizontal ordinate ignores X placement

    nRetval
= swDraw.AddOrdinateDimension2(swHorizontalOrdinate,
-0.1, 0.02, 0#)

End Sub