<!-- source: sldworksapiprogguide/GettingStarted/Option_Explicit_Statement.htm -->

# SOLIDWORKS API Help

# Option Explicit Statement

Including the Option Explicit
statement at the beginning of a Visual Basic for Applications (VBA) program
forces you to declare variables before they are used and assists in detecting
errors in your code.

## Example

'------------------------------------------------------------------------------
' In the following example, the Option
Explicit statement forces you to declare
' swApp
and retVal. Additionally, [early binding](Early_and_Late_Binding.htm) is used when declaring swApp.
'------------------------------------------------------------------------------

Option Explicit

Dim swApp As SldWorks.SldWorks

Dim retVal As Long

Sub main()

    Set swApp = Application.SldWorks

    retVal = swApp.CopyDocument("d:\samples\hotrod.sldprt",
"c:\temp\hotrod.sldprt", "", "", swMoveCopyOptionsOverwriteExistingDocs)

    Debug.Print retVal

End Sub