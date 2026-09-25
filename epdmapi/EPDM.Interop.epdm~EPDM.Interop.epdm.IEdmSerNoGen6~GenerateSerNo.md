<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSerNoGen6~GenerateSerNo.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GenerateSerNo Method (IEdmSerNoGen6) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmSerNoGen6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSerNoGen6.html) : GenerateSerNo Method (IEdmSerNoGen6) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsSerNoName*
:   Name of the serial number generator to use to generate a new serial number (see **Remarks**)

*lParentWnd*
:   Parent window handle; passed to a serial number add-in, if it exists

*bsFilePath*
:   Path to the file for which to generate a serial number

*lFolderID*
:   ID of the file's parent folder

*lFileID*
:   ID of the file for which to generate a serial number

*lCardID*
:   ID of the data card in which the serial number is generated

*lCardControlID*
:   ID of the control for which to generate a serial number

Obsolete. Superseded by [IEdmSerNoGen7::AllocSerNoValue](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSerNoGen7~AllocSerNoValue.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GenerateSerNo( _    ByVal bsSerNoName As System.String, _    Optional ByVal lParentWnd As System.Integer, _    Optional ByVal bsFilePath As System.String, _    Optional ByVal lFolderID As System.Integer, _    Optional ByVal lFileID As System.Integer, _    Optional ByVal lCardID As System.Integer, _    Optional ByVal lCardControlID As System.Integer _ ) As System.String ``` | |

| C# |  |
| --- | --- |
| ``` System.string GenerateSerNo(     System.string bsSerNoName,    System.int lParentWnd,    System.string bsFilePath,    System.int lFolderID,    System.int lFileID,    System.int lCardID,    System.int lCardControlID ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.String^ GenerateSerNo(  &   System.String^ bsSerNoName, &   System.int lParentWnd, &   System.String^ bsFilePath, &   System.int lFolderID, &   System.int lFileID, &   System.int lCardID, &   System.int lCardControlID ) ``` | |

#### Parameters

*bsSerNoName*
:   Name of the serial number generator to use to generate a new serial number (see **Remarks**)

*lParentWnd*
:   Parent window handle; passed to a serial number add-in, if it exists

*bsFilePath*
:   Path to the file for which to generate a serial number

*lFolderID*
:   ID of the file's parent folder

*lFileID*
:   ID of the file for which to generate a serial number

*lCardID*
:   ID of the data card in which the serial number is generated

*lCardControlID*
:   ID of the control for which to generate a serial number

#### Return Value

Serial number value

# ![](dotnetimages/collapse.gif)Remarks

This method is superseded by [IEdmSerNoGen7:AllocSerNoValue](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSerNoGen7~AllocSerNoValue.html) which provides the ability to push back serial numbers that you don't need using [IEdmSerNoValue](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSerNoValue.html).

bsSerNoName is the name you specify in the SOLIDWORKS PDM Professional Administration tool when you create a serial number generator.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* E\_EDM\_INVALID\_SERIAL\_NUMBER\_NAME: The bsSerNoName argument is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmSerNoGen6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSerNoGen6.html)

[IEdmSerNoGen6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSerNoGen6_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.0