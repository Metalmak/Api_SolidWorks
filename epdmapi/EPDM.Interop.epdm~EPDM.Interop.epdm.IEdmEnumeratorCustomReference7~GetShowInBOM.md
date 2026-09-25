<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorCustomReference7~GetShowInBOM.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetShowInBOM Method (IEdmEnumeratorCustomReference7) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmEnumeratorCustomReference7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorCustomReference7.html) : GetShowInBOM Method (IEdmEnumeratorCustomReference7) |

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

Gets whether the specified file's user-defined file references are shown in a BOM.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetShowInBOM( _    ByVal lFileID As System.Integer, _    ByVal lFolderID As System.Integer _ ) As System.Boolean ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetShowInBOM(     System.int lFileID,    System.int lFolderID ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetShowInBOM(  &   System.int lFileID, &   System.int lFolderID ) ``` | |

#### Parameters

*lFileID*
:   ID of referenced file

*lFolderID*
:   ID of parent folder of referenced file

#### Return Value

True if the specified file's user-defined file references are shown in a BOM, false if not

# ![](dotnetimages/collapse.gif)Example

[Access Custom File References (C#)](Access_Custom_File_References_Example_CSharp.htm)

[Access Custom File References (VB.NET)](Access_Custom_File_References_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmEnumeratorCustomReference7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorCustomReference7.html)

[IEdmEnumeratorCustomReference7 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorCustomReference7_members.html)

[IEdmEnumeratorCustomReference7::GetShowInBOM Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorCustomReference7~GetShowInBOM.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2017