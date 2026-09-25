<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| IEdmRevisionMgr Interface | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : IEdmRevisionMgr Interface |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Allows you to update revision numbers on many files all at once.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Interface IEdmRevisionMgr ``` | |

| C# |  |
| --- | --- |
| ``` public interface IEdmRevisionMgr ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IEdmRevisionMgr ``` | |

# ![](dotnetimages/collapse.gif)Remarks

This interface:

* inherits from IDispatch. See [IDispatch Interface (Automation)](http://msdn.microsoft.com/en-us/library/windows/desktop/ms221608%28v%3Dvs.85%29.aspx).* is extended by [IEdmRevisionMgr2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr2.html).* is more efficient than calling [IEdmFile5::IncrementRevision](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~IncrementRevision.html) for each file whose revision number you want to update.

Typical usage of this interface:

1. Access this interface by calling IEdmVault7::CreateUtility, setting eType to [EdmUtility](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUtility.html).EdmUtil\_RevisionMgr.- Call [IEdmRevisionMgr::SetRevisionCounters](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr~SetRevisionCounters.html) for each file  whose revision counters you want to set.- Call [IEdmRevisionMgr::IncrementRevision](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr~IncrementRevision.html) for each file whose revision you want to increment.- Call [IEdmRevisionMgr::Commit](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr~Commit.html) to commit all of the changes to the database.

# ![](dotnetimages/collapse.gif)Accessors

[IEdmVault7::CreateUtility](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault7~CreateUtility.html)

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmRevisionMgr Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)