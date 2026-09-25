<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUpdate.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| IEdmBatchUpdate Interface | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUpdate_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : IEdmBatchUpdate Interface |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Allows you to set the values of several file and folder card variables all at once.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Interface IEdmBatchUpdate ``` | |

| C# |  |
| --- | --- |
| ``` public interface IEdmBatchUpdate ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IEdmBatchUpdate ``` | |

# ![](dotnetimages/collapse.gif)Remarks

This interface:

* inherits from IDispatch. See [IDispatch Interface (Automation)](http://msdn.microsoft.com/en-us/library/windows/desktop/ms221608%28v%3Dvs.85%29.aspx).* is superseded by [IEdmBatchUpdate2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUpdate2.html), which can also update folder variables.

To set the values of file card variables:

1. Access this interface by calling [IEdmVault7::CreateUtility](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault7~CreateUtility.html), passing in [EdmUtility](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUtility.html).EdmUtil\_BatchUpdate.- Call [IEdmBatchUpdate::SetVar](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUpdate~SetVar.html) once for each variable you want to update.- Call [IEdmBatchUpdate::Commit](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUpdate~Commit.html) to commit all variable changes.

Before SOLIDWORKS PDM Professional 6.2, the only way to set the values of variables used in file data cards was to use the [IEdmEnumeratorVariable](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable9.html) interface which processed the variables one file and one variable at a time. This still works, but when setting the values of many variables, it is more efficient to use the IEdmBatchUpdate interface which accumulates all variables to set and then commits them all in a single operation.

# ![](dotnetimages/collapse.gif)Accessors

[IEdmVault7::CreateUtility](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault7~CreateUtility.html)

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchUpdate Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUpdate_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)