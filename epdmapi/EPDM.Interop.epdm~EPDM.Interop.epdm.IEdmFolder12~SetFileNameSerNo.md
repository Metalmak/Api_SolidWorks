<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder12~SetFileNameSerNo.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| SetFileNameSerNo Method (IEdmFolder12) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFolder12 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder12.html) : SetFileNameSerNo Method (IEdmFolder12) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*oSerialNumberName*
:   * File name without extension or path

        - or -

    * ID of the file's serial number generator

For internal use only; do not use.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub SetFileNameSerNo( _    ByVal oSerialNumberName As System.Object _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void SetFileNameSerNo(     System.object oSerialNumberName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetFileNameSerNo(  &   System.Object^ oSerialNumberName ) ``` | |

#### Parameters

*oSerialNumberName*
:   * File name without extension or path

        - or -

    * ID of the file's serial number generator

# ![](dotnetimages/collapse.gif)Remarks

This method specifies that when a file is added to the vault, its data card is created with a name that is either the added file's serial number or its name.

By default when files are added to the vault, file data cards are created with serial number names. To direct that an added file's data card be created with a file name instead of a serial number name, call this method specifying oSerialNumberName with a file name before calling [IEdmFolder8::AddFile2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder8~AddFile2.html) or [IEdmFolder6::AddFiles](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder6~AddFiles.html).

If you don't call this method before calling IEdmFolder8::AddFile2 or IEdmFolder6::AddFiles, the added file and its data card are created with different serial number names. To synchronize the serial number names:

1. Use [IEdmSerNoGen7](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSerNoGen7.html) to generate/get the added file's serial number.- Call this method, specifying oSerialNumberName with the added file's serial number generator ID.- Repeat steps 1 and 2 for each added file.- Call IEdmFolder8::AddFile2 or IEdmFolder6::AddFiles to add the new file(s) to the vault.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFolder12 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder12.html)

[IEdmFolder12 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder12_members.html)

[IEdmBatchAdd::SetFileNameSerNo Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAdd~SetFileNameSerNo.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2019