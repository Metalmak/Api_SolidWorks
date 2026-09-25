<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable8~CloseFile.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| CloseFile Method (IEdmEnumeratorVariable8) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmEnumeratorVariable8 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable8.html) : CloseFile Method (IEdmEnumeratorVariable8) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bFlush*
:   True to call [IEdmEnumeratorVariable5::Flush](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable5~Flush.html) before closing the file, false to not

Closes the file that is open for access by this interface.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub CloseFile( _    ByVal bFlush As System.Boolean _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void CloseFile(     System.bool bFlush ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void CloseFile(  &   System.bool bFlush ) ``` | |

#### Parameters

*bFlush*
:   True to call [IEdmEnumeratorVariable5::Flush](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable5~Flush.html) before closing the file, false to not

# ![](dotnetimages/collapse.gif)Example

[Set Part Number Using Default Serial Numbers (C#)](Set_Part_Number_Using_Default_Serial_Numbers_Example_CSharp.htm)

[Set Part Number Using Default Serial Numbers (VB.NET)](Set_Part_Number_Using_Default_Serial_Numbers_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

After closing the file using this method, none of the other methods in this interface work.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: An argument is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmEnumeratorVariable8 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable8.html)

[IEdmEnumeratorVariable8 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable8_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2008