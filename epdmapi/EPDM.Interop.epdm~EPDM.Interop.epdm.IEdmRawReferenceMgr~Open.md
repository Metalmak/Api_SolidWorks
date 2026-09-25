<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRawReferenceMgr~Open.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| Open Method (IEdmRawReferenceMgr) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmRawReferenceMgr Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRawReferenceMgr.html) : Open Method (IEdmRawReferenceMgr) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsPath*
:   Path to the file to open

Opens a file.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function Open( _    ByVal bsPath As System.String _ ) As System.Boolean ``` | |

| C# |  |
| --- | --- |
| ``` System.bool Open(     System.string bsPath ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool Open(  &   System.String^ bsPath ) ``` | |

#### Parameters

*bsPath*
:   Path to the file to open

#### Return Value

True if the file's format supports file references, false if not

# ![](dotnetimages/collapse.gif)Example

See the [IEdmRawReferenceMgr](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRawReferenceMgr.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

You must call this method before you call any of the other methods in this interface.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: The file's format does not support file references.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmRawReferenceMgr Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRawReferenceMgr.html)

[IEdmRawReferenceMgr Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRawReferenceMgr_members.html)

# ![](dotnetimages/collapse.gif)Availability

Version 6.4 of SOLIDWORKS PDM Professional