<!-- source: epdmapi/EPDM.Interop.EPDMResultCode~EPDM.Interop.EPDMResultCode.EdmResultSuccessCodes_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmResultSuccessCodes\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.EPDMResultCode Namespace](EPDM.Interop.EPDMResultCode~EPDM.Interop.EPDMResultCode_namespace.html) : EdmResultSuccessCodes\_e Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Success codes. See [EdmResultErrorCodes\_e](EPDM.Interop.EPDMResultCode~EPDM.Interop.EPDMResultCode.EdmResultErrorCodes_e.html) for error codes.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmResultSuccessCodes_e     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmResultSuccessCodes_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmResultSuccessCodes_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **S\_EDM\_32BIT\_ADDIN** | 0x4023D = Retrieved information successfully from the 32-bit add-in |
| **S\_EDM\_64BIT\_ADDIN** | 0x4023E = Retrieved information successfully from the 64-bit add-in |
| **S\_EDM\_FILES\_NOT\_UNIQUE\_GLOBALLY** | 0x4023F = The vault has the **Do not allow duplicate file names in the file vault** or **Do not allow duplicate file names with these extensions** option selected, and a file with the same name or filename extension exists in the vault |
| **S\_EDM\_INVALID\_FILE** | 0x4023C = The file was handled, but the file format is not recognized |
| **S\_EDM\_MENU\_ITEM\_NOT\_APPLICABLE** | 0x40219 = Menu item not valid in this context due to flags set |
| **S\_EDM\_REFRESH\_LIST** | 0x40201 = Success; refresh the entire list |
| **S\_EDM\_REFRESH\_MENU** | 0x40218 = Administrated plug-ins successfully; you should now recreate the plug-in menu |
| **S\_EDM\_REFRESH\_TREE** | 0x40202 = Success; refresh the tree |
| **S\_EDM\_TRY\_AGAIN** | 0x40203 = Try the operation again |

# ![](dotnetimages/collapse.gif)Example

Client code can only access these return codes by handling the exception. For example, in C#:

> try
> {
>     // Some SOLIDWORKS PDM Professional call that results in an exception
> }
> catch (System.Runtime.InteropServices.ComException comEx)
> {
>     switch (comEx.ErrorCode)
>     {
>         case S\_EDM\_*xxx*:
>             // respond to *xxx*
>             break;
>         case S\_EDM\_*yyy*:
>             // respond to *yyy*
>             break;
>         default:
>             // Unexpected or cannot be handled silently
>             // Use IEdmVault5::GetErrorString or IEdmVault11::GetErrorMessage to prepare a message for the user or log
>             break;
>     }
> }

# ![](dotnetimages/collapse.gif)Remarks

HRESULT return codes are supported by the SOLIDWORKS PDM Professional API. You can pass the HRESULT code to the method [IEdmVault11::GetErrorMessage](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11~GetErrorMessage.html) to get information about the code.

Client code can only access these success codes by handling the exception; i.e., via System.Runtime.InteropServices.ComException.

**NOTES:**

* Methods called from Visual Basic do not return the HRESULT code directly. Instead, the return codes are returned as an argument declared with the [retval] directive, if one exists. Visual Basic users can view the error codes returned by methods by implementing an error handler and checking the Number property of the Err object. The property is the HRESULT return code from the failing method.* The values shown in this topic are written in C++ style hexadecimal notation. In VB.NET, the value 0x80040200 is written as &H80040200.

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.EPDMResultCode Namespace](EPDM.Interop.EPDMResultCode~EPDM.Interop.EPDMResultCode_namespace.html)

[IEdmVault5::GetErrorString Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~GetErrorString.html)

[IEdmVault11::GetErrorName Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11~GetErrorName.html)

[Return Codes](ReturnCodes.htm)