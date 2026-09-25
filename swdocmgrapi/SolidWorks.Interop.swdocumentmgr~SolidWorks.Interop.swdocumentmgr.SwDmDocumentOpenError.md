<!-- source: swdocmgrapi/SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.SwDmDocumentOpenError.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Document Manager API Help | Send comments on this topic. |
| SwDmDocumentOpenError Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdocumentmgr Namespace](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr_namespace.html) : SwDmDocumentOpenError Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Document open errors.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum SwDmDocumentOpenError     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As SwDmDocumentOpenError ``` | |

| C# |  |
| --- | --- |
| ``` public enum SwDmDocumentOpenError : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class SwDmDocumentOpenError : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swDmDocumentOpenErrorFail** | 1 = File failed to open; reasons could be related to permissions or the file is in use by some other application or the file does not exist |
| **swDmDocumentOpenErrorFileNotFound** | 3 = File not found |
| **swDmDocumentOpenErrorFileReadOnly** | 4 = File is read only |
| **swDmDocumentOpenErrorFutureVersion** | 6 = File was created in a version of SOLIDWORKS more recent than the SOLIDWORKS Document Manager version attempting to open the file; you need to install a later version of SOLIDWORKS Document Manager; see [ISwDMApplication::GetLatestSupportedFileVersion](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMApplication~GetLatestSupportedFileVersion.html) |
| **swDmDocumentOpenErrorNoLicense** | 5 = No valid SOLIDWORKS Document Manager API license; the file may have been saved in a later version of SOLIDWORKS to which your license key does not allow access; see **License Key** section of [Getting Started](GettingStarted-swdocmgrapi.html) |
| **swDmDocumentOpenErrorNone** | 0 = File successfully opened |
| **swDmDocumentOpenErrorNonSW** | 2 = Non-SOLIDWORKS file was opened |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swdocumentmgr Namespace](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr_namespace.html)