<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorCustomReference7~SetShowInBOM.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| SetShowInBOM Method (IEdmEnumeratorCustomReference7) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmEnumeratorCustomReference7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorCustomReference7.html) : SetShowInBOM Method (IEdmEnumeratorCustomReference7) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lFileID*
:   ID of referenced file

*lFolderID*
:   ID of parent folder of referenced file

*bShowInBOM*
:   True to show the specified file's user-defined file references in a BOM, false to not

Sets whether to show the specified file's user-defined file references in a BOM.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub SetShowInBOM( _    ByVal lFileID As System.Integer, _    ByVal lFolderID As System.Integer, _    ByVal bShowInBOM As System.Boolean _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void SetShowInBOM(     System.int lFileID,    System.int lFolderID,    System.bool bShowInBOM ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetShowInBOM(  &   System.int lFileID, &   System.int lFolderID, &   System.bool bShowInBOM ) ``` | |

#### Parameters

*lFileID*
:   ID of referenced file

*lFolderID*
:   ID of parent folder of referenced file

*bShowInBOM*
:   True to show the specified file's user-defined file references in a BOM, false to not

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmEnumeratorCustomReference7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorCustomReference7.html)

[IEdmEnumeratorCustomReference7 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorCustomReference7_members.html)

[IEdmEnumeratorCustomReference7::GetShowInBOM Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorCustomReference7~GetShowInBOM.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2017