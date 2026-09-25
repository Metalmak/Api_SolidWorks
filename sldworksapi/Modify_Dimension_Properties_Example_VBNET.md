<!-- source: sldworksapi/Modify_Dimension_Properties_Example_VBNET.htm -->

# SOLIDWORKS API Help

# Modify Dimension Properties Example (VB.NET)

This example shows how to modify the properties of a selected display
dimension in a drawing.

'----------------------------------------------------------
' Preconditions:
' 1. Open a drawing document with one or more display
'    dimensions.
' 2. Select a display dimension.
'
' Postconditions:
' 1. The properties of the selected display dimension
'    are modified as specified.
' 2. Examine the display dimension to verify.
' ----------------------------------------------------------
Imports
SolidWorks.Interop.sldworks
Imports
SolidWorks.Interop.swconst
Imports
System.Runtime.InteropServices
Imports
System

Partial
Class
SolidWorksMacro

    Dim
swModel As
ModelDoc2
    Dim
swModelDoc Ext As
ModelDocExtension
    Dim
boolstatus As
Boolean

    Sub
main()

        swModel = swApp.**ActiveDoc**        swModelDocExt = swModel.**Extension**

        boolstatus = swModelDocExt.**EditDimensionProperties**(swTolType\_e.swTolBASIC,
0, 0, "",
"",
True, 9,
swDimensionArrowsSide\_e.swDimArrowsSmart, False,
swArrowStyle\_e.swSLASH\_ARROWHEAD, swArrowStyle\_e.swSLASH\_ARROWHEAD,
"",
"",
True,
"",
"",
"Example of lower text",
True,
swInConfigurationOpts\_e.swThisConfiguration,
""

)

        swModel.**ClearSelection2**(True)

    End
Sub

    Public
swApp As
SldWorks

End
Class