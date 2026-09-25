<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAdd~SetFileNameSerNo.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| SetFileNameSerNo Method (IEdmBatchAdd) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchAdd Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAdd.html) : SetFileNameSerNo Method (IEdmBatchAdd) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*oSerialNumberName*
:   File name or the ID of the serial number generator

*lFlags*
:   Must be 0

For internal use only; do not use.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub SetFileNameSerNo( _    ByVal oSerialNumberName As System.Object, _    Optional ByVal lFlags As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void SetFileNameSerNo(     System.object oSerialNumberName,    System.int lFlags ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetFileNameSerNo(  &   System.Object^ oSerialNumberName, &   System.int lFlags ) ``` | |

#### Parameters

*oSerialNumberName*
:   File name or the ID of the serial number generator

*lFlags*
:   Must be 0

# ![](dotnetimages/collapse.gif)Remarks

This method specifies that when a file is batch added to the vault, its data card is created with a name that is either the added file's serial number or its name.

By default when new files are added to the vault, file data cards are created with serial number names. Use this method to specify that when batch adding a file to the vault ([IEdmBatchAdd](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAdd.html)::Add\* methods), the file's data card name is the file name instead of the file's serial number.

If you don't call this method before calling the IEdmBatchAdd::Add\* methods, they will create one serial number for the file and another serial number for the file data card. To synchronize the serial numbers:

1. Generate the added file's serial number using [IEdmSerNoGen7](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSerNoGen7.html).- Call this method, specifying oSerialNumberName with the added file's serial number generator ID.- Repeat steps 1 and 2 for each new file.- Call one of the IEdmBatchAdd::Add\* methods to add the new files to the batch.- Call  [IEdmBatchAdd::CommitAdd](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAdd~CommitAdd.html).

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchAdd Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAdd.html)

[IEdmBatchAdd Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAdd_members.html)

[IEdmFolder12::SetFileNameSerNo Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder12~SetFileNameSerNo.html)

# ![](dotnetimages/collapse.gif)Availability

Version 6.4 of SOLIDWORKS PDM Professional