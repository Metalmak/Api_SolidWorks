<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchRefVars.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| IEdmBatchRefVars Interface | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchRefVars_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : IEdmBatchRefVars Interface |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Allows you to access several file reference variables all at once.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Interface IEdmBatchRefVars ``` | |

| C# |  |
| --- | --- |
| ``` public interface IEdmBatchRefVars ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IEdmBatchRefVars ``` | |

# ![](dotnetimages/collapse.gif)Example

[Batch Get and Set Reference Variables (VB.NET)](Batch_Get_and_Set_Reference_Variables_Example_VBNET.htm)

[Batch Get and Set Reference Variables (C#)](Batch_Get_and_Set_Reference_Variables_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This interface inherits from IDispatch. See [IDispatch Interface (Automation)](http://msdn.microsoft.com/en-us/library/windows/desktop/ms221608%28v%3Dvs.85%29.aspx).

Reference variables are used in Bill of Materials columns that are configured to look for reference-specific values. To create a reference variable:

1. Open the SOLIDWORKS PDM Professional Administration tool.- Log into a vault.- Double-click **Bill of Materials > BOM**.- Click a column in the **Columns** list.- Select **Look for variable in reference specific values**.- Click **OK**.- In a vault view, check out an assembly.- Click the **Bill of Materials** tab.- In the column configured to use reference-specific values, type text.- Click **Save** in the Bill of Materials toolbar.

Each component of the assembly is in a separate reference relationship with the assembly. The BOM column configured to **Look for variable in reference specific values** contains reference variable values. Use this interface to get and set these reference variable values.

# ![](dotnetimages/collapse.gif)Accessors

[IEdmVault7::CreateUtility](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault7~CreateUtility.html)

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchRefVars Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchRefVars_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)