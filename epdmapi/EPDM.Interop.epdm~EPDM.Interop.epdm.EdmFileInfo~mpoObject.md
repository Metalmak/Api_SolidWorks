<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFileInfo~mpoObject.html -->

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

| mpoObject Field | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [EdmFileInfo Structure](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFileInfo.html) : mpoObject Field |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Interface for the file or folder that was added to the batch using one of the [IEdmBatchAdd](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAdd.html)::AddXxxxx methods.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public mpoObject As IEdmObject5 ``` | |

| C# |  |
| --- | --- |
| ``` public IEdmObject5 mpoObject ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public: IEdmObject5^ mpoObject ``` | |

#### Field Value

[IEdmFile6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile6.html), if a file, or [IEdmFolder6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder6.html), if a folder

# ![](dotnetimages/collapse.gif)Remarks

This member is valid only if you specify [EdmBatchAddFolderFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBatchAddFolderFlag.html).Ebaff\_GetInterface or [EdmAddFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddFlag.html).EdmAdd\_GetInterface in the method that adds the file or folder to the batch.

# ![](dotnetimages/collapse.gif)See Also

####

[EdmFileInfo Structure](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFileInfo.html)

[EdmFileInfo Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFileInfo_members.html)