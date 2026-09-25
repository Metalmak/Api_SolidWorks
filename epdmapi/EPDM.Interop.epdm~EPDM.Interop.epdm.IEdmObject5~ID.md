<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmObject5~ID.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| ID Property (IEdmObject5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmObject5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmObject5.html) : ID Property (IEdmObject5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Gets the database ID of this object.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` ReadOnly Property ID As System.Integer ``` | |

| C# |  |
| --- | --- |
| ``` System.int ID {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int ID {    System.int get(); } ``` | |

#### Property Value

Database ID of this object

# ![](dotnetimages/collapse.gif)Example

[Get and Set Folder Permissions (VB.NET)](Get_and_Set_Folder_Permissions_Example_VBNET.htm)

[Get and Set Folder Permissions (C#)](Get_and_Set_Folder_Permissions_Example_CSharp.htm)

[Get File References for a File (C#)](Get_File_References_for_File_Example_CSharp.htm)

[Get File References for a File (VB.NET)](Get_File_References_for_File_Example_VBNET.htm)

[Create a Task that Finds Files in Workflow States (VB.NET)](Schedule_Task_to_Find_Files_in_State_Addin_Example_VBNET.htm)

[Create a Task that Finds Files in Workflow States (C#)](Schedule_Task_to_Find_Files_in_State_Addin_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Database IDs are unique for same-type objects. For example, two files can never have the same database ID; however, a file and a folder might have the same database ID.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmObject5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmObject5.html)

[IEdmObject5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmObject5_members.html)

# ![](dotnetimages/collapse.gif)Availability

Version 5.2 of SOLIDWORKS PDM Professional