<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetBatchUploadedFilesInfo.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetBatchUploadedFilesInfo Method (ISldWorks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : GetBatchUploadedFilesInfo Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ProcessedFileNames*
:   Array of processed file names

*NonProcessedFileNames*
:   Array of unprocessed file names

*FailedFileNames*
:   Array of file names that failed to upload

Gets the files uploaded to 3DEXPERIENCE during a batch process.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetBatchUploadedFilesInfo( _    ByRef ProcessedFileNames As System.Object, _    ByRef NonProcessedFileNames As System.Object, _    ByRef FailedFileNames As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim ProcessedFileNames As System.Object Dim NonProcessedFileNames As System.Object Dim FailedFileNames As System.Object Dim value As System.Boolean   value = instance.GetBatchUploadedFilesInfo(ProcessedFileNames, NonProcessedFileNames, FailedFileNames) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetBatchUploadedFilesInfo(     out System.object ProcessedFileNames,    out System.object NonProcessedFileNames,    out System.object FailedFileNames ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetBatchUploadedFilesInfo(  &   [Out] System.Object^ ProcessedFileNames, &   [Out] System.Object^ NonProcessedFileNames, &   [Out] System.Object^ FailedFileNames ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ProcessedFileNames*
:   Array of processed file names

*NonProcessedFileNames*
:   Array of unprocessed file names

*FailedFileNames*
:   Array of file names that failed to upload

#### Return Value

True if retrieval successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::GetBatchUploadedFilesInfo.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only for SOLIDWORKS Connected.

Before calling this method, call [ISldWorks::RunBatchSaveProcess](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~RunBatchSaveProcess.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2022 SP03, Revision Number 30.3