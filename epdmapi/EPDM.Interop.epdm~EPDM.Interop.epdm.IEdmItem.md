<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmItem.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| IEdmItem Interface | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmItem_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : IEdmItem Interface |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Allows you to access an item.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Interface IEdmItem     Inherits IEdmObject5  ``` | |

| C# |  |
| --- | --- |
| ``` public interface IEdmItem : IEdmObject5  ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IEdmItem : public IEdmObject5  ``` | |

# ![](dotnetimages/collapse.gif)Example

[Get and Set Item References (VB.NET)](Get_and_Set_Item_References_Example_VBNET.htm)

[Get and Set Item References (C#)](Get_and_Set_Item_References_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This interface inherits from [IEdmObject5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmObject5.html).

To access this interface, you can:

* Cast [IEdmFile*X*](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5.html) objects to an IEdmItem pointer.* Call IEdmVault5::GetObject, setting eType to [EdmObjectType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmObjectType.html).EdmObject\_Item.

See the [Programming Items](Items.htm) topic for more information.

# ![](dotnetimages/collapse.gif)Accessors

[IEdmVault5::GetObject](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~GetObject.html)

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmItem Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmItem_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)