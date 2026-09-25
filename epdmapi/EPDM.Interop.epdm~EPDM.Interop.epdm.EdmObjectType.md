<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmObjectType.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmObjectType Enumeration | |
| [See Also](#seealsobookmark)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmObjectType Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Types of objects returned by [IEdmObject5::ObjectType](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmObject5~ObjectType.html), [IEdmFile5::ObjectType](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~ObjectType.html), and [IEdmFolder5::ObjectType](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~ObjectType.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmObjectType     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmObjectType : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmObjectType : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **EdmObject\_Attribute** | 10 = The object is an attribute, used in variables, and it supports the [IEdmAttribute5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAttribute5.html) interface |
| **EdmObject\_BOM** | 15 = The object is a Bill of Materials; see [IEdmBom](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBom.html) |
| **EdmObject\_Card** | 5 = The object is a file/folder data card, and it supports the [IEdmCard5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCard5.html) interface |
| **EdmObject\_CardControl** | 6 = The object is a control in a file/folder data card, and it supports the [IEdmCardControl5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardControl5.html) interface |
| **EdmObject\_Category** | 14 = The object is a category; see [IEdmCategory6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCategory6.html) |
| **EdmObject\_Dictionary** | 12 = The object is a dictionary, and it supports the [IEdmDictionary5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmDictionary5.html) interface |
| **EdmObject\_File** | 1 = The object is a file, and it supports the [IEdmFile5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5.html) interface |
| **EdmObject\_Folder** | 2 = The object is a folder, and it supports the [IEdmFolder5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5.html) interface |
| **EdmObject\_Invalid** | 0 = This is not an object type; it is an error code |
| **EdmObject\_Item** | 16 = The object is an [item](Items.htm); see [IEdmItem](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmItem.html) |
| **EdmObject\_ItemFolder** | 17 = The object is a parent folder of an [item](Items.htm); see [IEdmFolder6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder6.html) |
| **EdmObject\_ItemRootFolder** | 18 = The object is the invisible root folder of all [item](Items.htm) folders; see [IEdmFolder6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder6.html) |
| **EdmObject\_Label** | 11 = The object is a label, and it supports the [IEdmLabel5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmLabel5.html) interface |
| **EdmObject\_State** | 3 = The object is a workflow state, and it supports the [IEdmState5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmState5.html) interface |
| **EdmObject\_Transition** | 4 = The object is a transition (i.e., a workflow state change), and it supports the [IEdmTransition5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTransition5.html) interface |
| **EdmObject\_User** | 7 = The object is a user, and it supports the [IEdmUser5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser5.html) interface |
| **EdmObject\_UserGroup** | 8 = The object is a user group, and it supports the [IEdmUserGroup5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserGroup5.html) interface |
| **EdmObject\_Variable** | 9 = The object is a variable (for file/folder data cards), and it supports the IEdmVariable5 interface |
| **EdmObject\_Workflow** | 13 = The object is a workflow; see [IEdmWorkflow5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmWorkflow5.html) and [IEdmWorkflow6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmWorkflow6.html) |

# ![](dotnetimages/collapse.gif)Example

[Get and Set Folder Permissions (VB.NET)](Get_and_Set_Folder_Permissions_Example_VBNET.htm)

[Get and Set Folder Permissions (C#)](Get_and_Set_Folder_Permissions_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

All interfaces that inherit from IEdmObject5 have a corresponding EdmObjectType value indicating the kind of object.

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

[IEdmVault5::GetObject Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~GetObject.html)