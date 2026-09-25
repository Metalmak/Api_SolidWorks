<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAttribute5.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| IEdmAttribute5 Interface | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAttribute5_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : IEdmAttribute5 Interface |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Allows access to a file attribute that is used when data is transferred between a file data card and a file.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Interface IEdmAttribute5     Inherits IEdmObject5  ``` | |

| C# |  |
| --- | --- |
| ``` public interface IEdmAttribute5 : IEdmObject5  ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IEdmAttribute5 : public IEdmObject5  ``` | |

# ![](dotnetimages/collapse.gif)Example

[Find Data Cards with Description Variable (VB.NET)](Find_Data_Cards_with_Description_Variable_Example_VBNET.htm)

[Find Data Cards with Description Variable (C#)](Find_Data_Cards_with_Description_Variable_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This interface inherits from [IEdmObject5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmObject5.html). Call [IEdmObject5::Name](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmObject5~Name.html) to get the name of this attribute.

A variable, [EdmVariable5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariable5.html), can be mapped to zero or more attributes (IEdmAttribute5).

# ![](dotnetimages/collapse.gif)Accessors

[IEdmVariable5::GetNextAttribute](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariable5~GetNextAttribute.html)

[IEdmVariableValue5::GetNextAttribute](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariableValue5~GetNextAttribute.html)

[IEdmVault5::GetObject](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~GetObject.html)

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmAttribute5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAttribute5_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)