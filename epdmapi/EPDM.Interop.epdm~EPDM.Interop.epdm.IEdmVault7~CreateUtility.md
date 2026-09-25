<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault7~CreateUtility.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| CreateUtility Method (IEdmVault7) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVault7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault7.html) : CreateUtility Method (IEdmVault7) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*eType*
:   Type of interface to create as defined in [EdmUtility](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUtility.html)

Creates a utility interface of the specified type.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function CreateUtility( _    ByVal eType As EdmUtility _ ) As System.Object ``` | |

| C# |  |
| --- | --- |
| ``` System.object CreateUtility(     EdmUtility eType ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ CreateUtility(  &   EdmUtility eType ) ``` | |

#### Parameters

*eType*
:   Type of interface to create as defined in [EdmUtility](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUtility.html)

#### Return Value

Interface

# ![](dotnetimages/collapse.gif)Example

[Find Revisions Using Component (C#)](Find_Revisions_Using_Component_Example_CSharp.htm)

[Find Revisions Using Component (VB.NET)](Find_Revisions_Using_Component_Example_VBNET.htm)

[Add Items (C#)](Add_Items_Example_CSharp.htm)

[Add Items (VB.NET)](Add_Items_Example_VBNET.htm)

[Get File References for a File (C#)](Get_File_References_for_File_Example_CSharp.htm)

[Get File References for a File (VB.NET)](Get_File_References_for_File_Example_VBNET.htm)

[Create a Task that Finds Files in Workflow States (VB.NET)](Schedule_Task_to_Find_Files_in_State_Addin_Example_VBNET.htm)

[Create a Task that Finds Files in Workflow States (C#)](Schedule_Task_to_Find_Files_in_State_Addin_Example_CSharp.htm)

[Add Custom File Reference (VB.NET)](Add_Custom_File_Reference_Example_VBNET.htm)

[Add Custom File Reference (C#)](Add_Custom_File_Reference_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVault7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault7.html)

[IEdmVault7 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault7_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.2