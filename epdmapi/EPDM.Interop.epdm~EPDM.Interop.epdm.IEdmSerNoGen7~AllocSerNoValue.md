<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSerNoGen7~AllocSerNoValue.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| AllocSerNoValue Method (IEdmSerNoGen7) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmSerNoGen7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSerNoGen7.html) : AllocSerNoValue Method (IEdmSerNoGen7) |

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
:   ID of the data card for which to generate a serial number

*lCardControlID*
:   ID of the control for which to generate a serial number

Generates a new serial number for the specified file, data card, or card control using the specified serial number generator.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function AllocSerNoValue( _    ByVal bsSerNoName As System.String, _    Optional ByVal lParentWnd As System.Integer, _    Optional ByVal bsFilePath As System.String, _    Optional ByVal lFolderID As System.Integer, _    Optional ByVal lFileID As System.Integer, _    Optional ByVal lCardID As System.Integer, _    Optional ByVal lCardControlID As System.Integer _ ) As IEdmSerNoValue ``` | |

| C# |  |
| --- | --- |
| ``` IEdmSerNoValue AllocSerNoValue(     System.string bsSerNoName,    System.int lParentWnd,    System.string bsFilePath,    System.int lFolderID,    System.int lFileID,    System.int lCardID,    System.int lCardControlID ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmSerNoValue^ AllocSerNoValue(  &   System.String^ bsSerNoName, &   System.int lParentWnd, &   System.String^ bsFilePath, &   System.int lFolderID, &   System.int lFileID, &   System.int lCardID, &   System.int lCardControlID ) ``` | |

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
:   ID of the data card for which to generate a serial number

*lCardControlID*
:   ID of the control for which to generate a serial number

#### Return Value

[IEdmSerNoValue](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSerNoValue.html)

# ![](dotnetimages/collapse.gif)Example

[Set Part Number Using Default Serial Numbers (C#)](Set_Part_Number_Using_Default_Serial_Numbers_Example_CSharp.htm)

[Set Part Number Using Default Serial Numbers (VB.NET)](Set_Part_Number_Using_Default_Serial_Numbers_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

The difference between this method and the now obsolete [IEdmSerNoGen6::GenerateSerNo](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSerNoGen6~GenerateSerNo.html) method is that this method returns an [IEdmSerNoValue](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSerNoValue.html) interface instead of a string. [IEdmSerNoValue::Rollback](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSerNoValue~Rollback.html) allows you to return generated numbers that you can not use. This helps to avoid gaps between serial numbers.

bsSerNoName is the name you specify in the SOLIDWORKS PDM Professional Administration tool when you create a serial number generator.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* E\_EDM\_INVALID\_SERIAL\_NUMBER\_NAME: The bsSerNoName argument is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmSerNoGen7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSerNoGen7.html)

[IEdmSerNoGen7 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSerNoGen7_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.4