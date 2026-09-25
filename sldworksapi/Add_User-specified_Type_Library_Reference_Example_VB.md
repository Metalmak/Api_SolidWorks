<!-- source: sldworksapi/Add_User-specified_Type_Library_Reference_Example_VB.htm -->

# SOLIDWORKS API Help

# Add User-specified Type Library Reference Example (VBA)

This example shows how to add a user-specified type library reference.

'----------------------------------------

' Preconditions:  User-specified
type library exists.

'

' Postconditions: User-specified type library is added.
It is

'                 visible
on VBA Available References
list

'                 only
after recording a macro.

'-----------------------------------------

Option Explicit

Dim swApp As SldWorks.SldWorks

Dim v1 As Variant

Dim s(0) As String

Sub main()

> Set swApp = Application.SldWorks
>
> s(0) = "c:\Program Files\MyAddin\myaddin.tlb"
>
> v1 = s
>
> swApp.UserTypeLibReferences
> = v1
>
> Debug.Print v1(0)

End Sub