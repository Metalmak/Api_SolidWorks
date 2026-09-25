<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmDictionary5.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| IEdmDictionary5 Interface | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmDictionary5_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : IEdmDictionary5 Interface |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Allows you to access key-value pairs of data in the SOLIDWORKS PDM Professional database.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Interface IEdmDictionary5     Inherits IEdmObject5  ``` | |

| C# |  |
| --- | --- |
| ``` public interface IEdmDictionary5 : IEdmObject5  ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IEdmDictionary5 : public IEdmObject5  ``` | |

# ![](dotnetimages/collapse.gif)Example

[Change Card Variables Add-in (VB.NET)](Change_Card_Variables_Addin_Example_VBNET.htm)

[Change Card Variables Add-in (C#)](Change_Card_Variables_Addin_Example_CSharp.htm)

[Create and Delete Dictionaries (C#)](Create_and_Delete_Dictionaries_Example_CSharp.htm)

[Create and Delete Dictionaries (VB.NET)](Create_and_Delete_Dictionaries_Example_VBNET.htm)

[Get and Set Dictionary Key-Value Pairs (VB.NET)](Get_and_Set_Key_Value_Pairs_Example_VBNET.htm)

[Get and Set Dictionary Key-Value Pairs (C#)](Get_and_Set_Key_Value_Pairs_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This interface inherits from [IEdmObject5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmObject5.html). Call [IEdmObject5::Name](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmObject5~Name.html) to get the name of the dictionary.

To access this interface, call [IEdmVault5::GetObject](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~GetObject.html), setting eType to [EdmObjectType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmObjectType.html).EdmObject\_Dictionary.

A dictionary in SOLIDWORKS PDM Professional stores data as key-value pairs. Each key is mapped to exactly one value. Both keys and values can be searched using this interface.

**Note:** Instead of using dictionaries, you can also use [IEdmEnumeratorVariable5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable5.html) to store data in card variables that are connected to files and folders. One advantage of this is that if the data is logically linked to files or folders, the data is deleted and copied whenever the files or folders are deleted or copied.

# ![](dotnetimages/collapse.gif)Accessors

[IEdmVault5::GetDictionary](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~GetDictionary.html)

[IEdmVault5::GetObject](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~GetObject.html)

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmDictionary5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmDictionary5_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)