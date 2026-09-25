<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr~SetRevisionCounters.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| SetRevisionCounters Method (IEdmRevisionMgr) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmRevisionMgr Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr.html) : SetRevisionCounters Method (IEdmRevisionMgr) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lFileID*
:   ID of file in which to set counters

*poCounters*
:   Array of [EdmRevCounter](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevCounter.html) structures; one structure for each revision component

Sets the revision number component counters to specified values.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub SetRevisionCounters( _    ByVal lFileID As System.Integer, _    ByVal poCounters() As EdmRevCounter _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void SetRevisionCounters(     System.int lFileID,    EdmRevCounter[] poCounters ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetRevisionCounters(  &   System.int lFileID, &   array<EdmRevCounter>^ poCounters ) ``` | |

#### Parameters

*lFileID*
:   ID of file in which to set counters

*poCounters*
:   Array of [EdmRevCounter](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevCounter.html) structures; one structure for each revision component

# ![](dotnetimages/collapse.gif)Example

[Set Initial Revision (VB.NET)](Set_Initial_Revision_Example_VBNET.htm)

[Set Initial Revision (C#)](Set_Initial_Revision_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method only adds the new counters to this batch. After calling this method, you must call [IEdmRevisionMgr::Commit](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr~Commit.html) to commit the changes to the database.

This method only sets the revision component counters. It does not generate new revision numbers using any of the revision number generators that may be using the components. To create a new revision number for the file, you must also call [IEdmRevisionMgr::IncrementRevision](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr~IncrementRevision.html).

The order of calls to this method and IEdmRevisionMgr::IncrementRevision does not matter. Calls to IRevisionMgr::IncrementRevision are always processed after calls to this method.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmRevisionMgr Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr.html)

[IEdmRevisionMgr Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2007