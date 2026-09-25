<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile7~NeedsRegeneration.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| NeedsRegeneration Method (IEdmFile7) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFile7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile7.html) : NeedsRegeneration Method (IEdmFile7) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lVersion*
:   File version; 0 to check the version in the local cache

*oFolderPathOrID*
:   Path or ID of the file's parent folder; valid only if lVersion is not 0

Gets whether the file with the specified version and location needs to be rebuilt in its associated CAD program.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function NeedsRegeneration( _    ByVal lVersion As System.Integer, _    Optional ByVal oFolderPathOrID As System.Object _ ) As System.Boolean ``` | |

| C# |  |
| --- | --- |
| ``` System.bool NeedsRegeneration(     System.int lVersion,    System.object oFolderPathOrID ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool NeedsRegeneration(  &   System.int lVersion, &   System.Object^ oFolderPathOrID ) ``` | |

#### Parameters

*lVersion*
:   File version; 0 to check the version in the local cache

*oFolderPathOrID*
:   Path or ID of the file's parent folder; valid only if lVersion is not 0

#### Return Value

True if the file needs to be rebuilt in its associated CAD program, false if not

# ![](dotnetimages/collapse.gif)Remarks

If you have a drawing that references a part, and you make a model change on the part and don't rebuild the drawing in the CAD program, then the drawing shows the earlier version of the part. Use this method to check whether the drawing needs to be rebuilt with the newer version of the part in the associated CAD program.

Support for rebuild checks is only available for files saved with SOLIDWORKS 2009 or later.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: An argument is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFile7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile7.html)

[IEdmFile7 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile7_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2009