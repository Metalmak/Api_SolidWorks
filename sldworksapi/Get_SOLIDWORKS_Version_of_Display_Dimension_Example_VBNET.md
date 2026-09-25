<!-- source: sldworksapi/Get_SOLIDWORKS_Version_of_Display_Dimension_Example_VBNET.htm -->

# SOLIDWORKS API Help

# Get SOLIDWORKS Version of Display Dimension (VB.NET)

This example shows how to find out if a display dimension in a drawing was
created in SOLIDWORKS 2011 or later.

'------------------------------------------------

' Preconditions:

' 1. Open a drawing document in which a display

'    dimension exists.

' 2. Open the Immediate window.

' 3. Select the display dimension.

'

' Postconditions: Examine the Immediate window

' to see if the selected display dimension

' was created in SOLIDWORKS 2011 or later.

'-------------------------------------------------

Imports

 SolidWorks.Interop.sldworks

Imports

 SolidWorks.Interop.swconst

Imports

 System

Imports

 System.Diagnostics

Partial

Class SolidWorksMacro
> Public
> Sub Main()
>
> > Dim
> > swModel As
> > ModelDoc2

Dim
swSelMgr As
SelectionMgrDim
swDispDim As
DisplayDimensionDim
swSelObj As
Object

Dim selCount
As
Long

Dim selType
As
Long

swModel = swApp.**ActiveDoc**

swSelMgr = swModel.**SelectionManager**

selCount = swSelMgr.**GetSelectedObjectCount2**(-1)

If selCount < 1
Then

    Debug.Print("Select
a display dimension and rerun the macro.")

Exit Sub

End
If

selType = swSelMgr.**GetSelectedObjectType3**(1, 0)

swSelObj = swSelMgr.**GetSelectedObject6**(1, 0)

Select
Case selType

> Case
> swSelectType\_e.swSelDIMENSIONS
>
> swDispDim = swSelObj
>
> Debug.Print("Was
> display dimension created in SOLIDWORKS 2011 or later? " &
> swDispDim.**GetSupportsGenericText**)

End
Select

End
Sub

> ''' <summary>
>
> ''' The SldWorks swApp
> variable is pre-assigned for you.
>
> ''' </summary>
>
> Public swApp
> As SldWorks

End

Class