<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariable5~GetFirstAttributePosition.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetFirstAttributePosition Method (IEdmVariable5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVariable5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariable5.html) : GetFirstAttributePosition Method (IEdmVariable5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsFileExtension*
:   Extension of file for which to get attributes, e.g., "DWG" or "DOC"; "" to get all attributes for all file types

Starts an enumeration of the attributes to which this variable is mapped for the specified file type.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetFirstAttributePosition( _    ByVal bsFileExtension As System.String _ ) As IEdmPos5 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmPos5 GetFirstAttributePosition(     System.string bsFileExtension ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmPos5^ GetFirstAttributePosition(  &   System.String^ bsFileExtension ) ``` | |

#### Parameters

*bsFileExtension*
:   Extension of file for which to get attributes, e.g., "DWG" or "DOC"; "" to get all attributes for all file types

#### Return Value

[IEdmPos5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html); position of the first attribute in the enumeration

# ![](dotnetimages/collapse.gif)Example

[Find Data Cards with Description Variable (C#)](Find_Data_Cards_with_Description_Variable_Example_CSharp.htm)

[Find Data Cards with Description Variable (VB.NET)](Find_Data_Cards_with_Description_Variable_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

A variable in SOLIDWORKS PDM Professional can be mapped to zero or more block-attribute pairs. SOLIDWORKS PDM Professional uses the attributes when transferring data between the file data card and the file, itself. See the main SOLIDWORKS PDM Professional online help for more information.

After calling this method, pass the returned position of the first attribute to [IEdmVariable5::GetNextAttribute](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariable5~GetNextAttribute.html) to get the first attribute in this list. Then call IEdmVariable5::GetNextAttribute repeatedly to get the rest of the attributes.

C++ users not using smart-pointer wrapper functions must release the returned interface, IEdmPos5.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVariable5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariable5.html)

[IEdmVariable5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariable5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2