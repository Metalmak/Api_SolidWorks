<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFile2~mlLocalVersion.html -->

![](dotnetimages/collapse.gif)
![](dotnetimages/expand.gif)
![](dotnetimages/collapse.gif)
![](dotnetimages/expand.gif)
![](dotnetimages/drpdown.gif)
![](dotnetimages/drpdown_orange.gif)
![](dotnetimages/copycode.gif)
![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |

| mlLocalVersion Field | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [EdmListFile2 Structure](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFile2.html) : mlLocalVersion Field |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Version of the file in the local cache, based on the date of the file passed to the [IEdmBatchListing::AddFile](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing~AddFile.html) method.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public mlLocalVersion As System.Integer ``` | |

| C# |  |
| --- | --- |
| ``` public System.int mlLocalVersion ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public: System.int mlLocalVersion ``` | |

#### Field Value

Version of the file in the local cache or 0 if the date of the version of the file in local cache passed to IEdmBatchListing::AddFile doesn’t match any version of the file in the vault

# ![](dotnetimages/collapse.gif)See Also

####

[EdmListFile2 Structure](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFile2.html)

[EdmListFile2 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFile2_members.html)