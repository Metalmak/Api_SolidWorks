<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr2~GetRevisionNumberIDFromFile.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetRevisionNumberIDFromFile Method (IEdmRevisionMgr2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmRevisionMgr2 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr2.html) : GetRevisionNumberIDFromFile Method (IEdmRevisionMgr2) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lFileID*
:   ID of file for which to get a revision number (see **Remarks**)

*pbCanIncrement*
:   True if the next increment will succeed, false if not

Gets the active revision number of the specified file.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetRevisionNumberIDFromFile( _    ByVal lFileID As System.Integer, _    ByRef pbCanIncrement As System.Boolean _ ) As System.Integer ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetRevisionNumberIDFromFile(     System.int lFileID,    out System.bool pbCanIncrement ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetRevisionNumberIDFromFile(  &   System.int lFileID, &   [Out] System.bool pbCanIncrement ) ``` | |

#### Parameters

*lFileID*
:   ID of file for which to get a revision number (see **Remarks**)

*pbCanIncrement*
:   True if the next increment will succeed, false if not

#### Return Value

Revision number ID; 0 if no revision number is found for the file

# ![](dotnetimages/collapse.gif)Example

[Set Initial Revision (VB.NET)](Set_Initial_Revision_Example_VBNET.htm)

[Set Initial Revision (C#)](Set_Initial_Revision_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, set lFileID using [IEdmFile5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5.html).ID.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmRevisionMgr2 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr2.html)

[IEdmRevisionMgr2 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2007 SP03