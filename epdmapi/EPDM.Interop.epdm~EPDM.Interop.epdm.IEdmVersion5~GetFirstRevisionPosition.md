<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVersion5~GetFirstRevisionPosition.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetFirstRevisionPosition Method (IEdmVersion5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVersion5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVersion5.html) : GetFirstRevisionPosition Method (IEdmVersion5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Starts an enumeration of the revisions of this version.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetFirstRevisionPosition() As IEdmPos5 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmPos5 GetFirstRevisionPosition() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmPos5^ GetFirstRevisionPosition(); ``` | |

#### Return Value

[IEdmPos5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html); position of the first revision in the enumeration

# ![](dotnetimages/collapse.gif)Example

[Get Revision Names for Local Version of File (C#)](Get_Revision_Names_for_Local_Version_of_File_Example_CSharp.htm)

[Get Revision Names for Local Version of File (VB.NET)](Get_Revision_Names_for_Local_Version_of_File_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

After calling this method, pass the returned position of the first revision to [IEdmVersion5::GetNextRevision](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVersion5~GetNextRevision.html) to get the first revision in this list. Then call IEdmVersion5::GetNextRevision repeatedly to get the rest of the revisions.

C++ users not using smart-pointer wrapper functions must release the returned interface, IEdmPos5.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVersion5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVersion5.html)

[IEdmVersion5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVersion5_members.html)

[IEdmRevision5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevision5.html)

[IEdmEnumeratorVersion5::GetFirstRevisionPosition Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVersion5~GetFirstRevisionPosition.html)

[IEdmVersion5::HasRevision Property ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVersion5~HasRevision.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2