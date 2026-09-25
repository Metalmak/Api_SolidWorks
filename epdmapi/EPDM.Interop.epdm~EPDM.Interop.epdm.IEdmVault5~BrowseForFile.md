<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~BrowseForFile.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| BrowseForFile Method (IEdmVault5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVault5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5.html) : BrowseForFile Method (IEdmVault5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*hParentWnd*
:   Parent window handle

*lEdmBrowseFlags*
:   Optional combination of [EdmBrowseFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBrowseFlag.html) bits

*bsFilter*
:   Optional filter string that limits the types of files displayed in the dialog box (see **Remarks**)

*bsDefaultExtension*
:   Optional default file extension to append if the user does not specify an extension

*bsDefaultFileName*
:   Optional default file name to display in the file name field of the dialog box

*bsDefaultFolder*
:   Optional path to the folder on which the dialog box should initially open

*bsCaption*
:   Optional caption for the dialog box

Displays an Open or Save As dialog box in which the user can click one or more files.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function BrowseForFile( _    ByVal hParentWnd As System.Integer, _    Optional ByVal lEdmBrowseFlags As System.Integer, _    Optional ByVal bsFilter As System.String, _    Optional ByVal bsDefaultExtension As System.String, _    Optional ByVal bsDefaultFileName As System.String, _    Optional ByVal bsDefaultFolder As System.String, _    Optional ByVal bsCaption As System.String _ ) As EdmStrLst5 ``` | |

| C# |  |
| --- | --- |
| ``` EdmStrLst5 BrowseForFile(     System.int hParentWnd,    System.int lEdmBrowseFlags,    System.string bsFilter,    System.string bsDefaultExtension,    System.string bsDefaultFileName,    System.string bsDefaultFolder,    System.string bsCaption ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` EdmStrLst5^ BrowseForFile(  &   System.int hParentWnd, &   System.int lEdmBrowseFlags, &   System.String^ bsFilter, &   System.String^ bsDefaultExtension, &   System.String^ bsDefaultFileName, &   System.String^ bsDefaultFolder, &   System.String^ bsCaption ) ``` | |

#### Parameters

*hParentWnd*
:   Parent window handle

*lEdmBrowseFlags*
:   Optional combination of [EdmBrowseFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBrowseFlag.html) bits

*bsFilter*
:   Optional filter string that limits the types of files displayed in the dialog box (see **Remarks**)

*bsDefaultExtension*
:   Optional default file extension to append if the user does not specify an extension

*bsDefaultFileName*
:   Optional default file name to display in the file name field of the dialog box

*bsDefaultFolder*
:   Optional path to the folder on which the dialog box should initially open

*bsCaption*
:   Optional caption for the dialog box

#### Return Value

[IEdmStrLst5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmStrLst5.html); list of paths to multi-selected files; Null if the user clicks **Cancel** (see **Remarks**)

# ![](dotnetimages/collapse.gif)Example

[Set Initial Revision (VB.NET)](Set_Initial_Revision_Example_VBNET.htm)

[Set Initial Revision (C#)](Set_Initial_Revision_Example_CSharp.htm)

[Access Check-in Flags in Check out Dialog (VB.NET)](Access_Check-in_Flags_in_Check_in_Dialog_Example_VBNET.htm)

[Access Check-in Flags in Check out Dialog (C#)](Access_Check-in_Flags_in_Check_in_Dialog_Example_CSharp.htm)

[Prevent Admin from Checking In File (C#)](Prevent_Admin_from_Checking_In_File_Example_CSharp.htm)

[Prevent Admin from Checking In File (VB.NET)](Prevent_Admin_from_Checking_In_File_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

If bsFilter is not empty, it contains the options for the **Files of type** combobox dropdown in the dialog box. Each option consists of a pair of substrings, where the first substring is the description that appears in the combobox dropdown:

> All Image Files (\*.JPG,\*.BMP)

and the second substring consists of one or more extension filters delimited by semicolons:

> \*.JPG;\*.BMP

The substrings are separated by a vertical bar, |, and the entire string is terminated with double vertical bars, ||.

For example, to give the combobox dropdown four options, including JPG and BMP file filters, specify bsFilter with the following string (without quotes):

"All Image Files (\*.JPG,\*.BMP)|\*.JPG;\*.BMP|JPEG-Files (\*.JPG)|\*.JPG|BMP-Files (\*.BMP)|\*.BMP|All Files (\*.\*)|\*.\*||"

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVault5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5.html)

[IEdmVault5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5_members.html)

[IEdmVault5::BrowseForFolder Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~BrowseForFolder.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2