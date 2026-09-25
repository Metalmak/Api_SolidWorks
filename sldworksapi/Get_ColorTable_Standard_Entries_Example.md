<!-- source: sldworksapi/Get_ColorTable_Standard_Entries_Example.htm -->

# SOLIDWORKS API Help

# Get ColorTable Standard Entries Example (VBA)

This example shows how to get the names of
all standard colors and the corresponding COLORREF values.

'---------------------------------------------

' Get the ColorTable Object

Set ColorTable = Part.GetColorTable()

' Iterate through standard colors

For Count = 0 To ColorTable.GetStandardCount()
- 1

    '
Get the entry name

    ColorName
= ColorTable.GetNameAtIndex(Count)

    '
Get the Entry COLORREF

    ColorRef
= ColorTable.GetColorRefAtIndex(Count)

Next Count