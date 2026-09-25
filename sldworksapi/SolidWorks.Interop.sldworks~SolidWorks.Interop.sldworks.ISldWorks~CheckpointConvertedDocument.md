<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~CheckpointConvertedDocument.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CheckpointConvertedDocument Method (ISldWorks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : CheckpointConvertedDocument Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DocName*
:   Full pathname of the file to save

Saves the specified open document if its version is older than the version of the SOLIDWORKS product being used.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CheckpointConvertedDocument( _    ByVal DocName As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim DocName As System.String Dim value As System.Integer   value = instance.CheckpointConvertedDocument(DocName) ``` | |

| C# |  |
| --- | --- |
| ``` System.int CheckpointConvertedDocument(     System.string DocName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int CheckpointConvertedDocument(  &   System.String^ DocName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*DocName*
:   Full pathname of the file to save

#### Return Value

0 for no error or a bitwise OR of the errors encountered as defined in swFileSaveError\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::CheckpointConvertedDocument.

# ![](dotnetimages/collapse.gif)Remarks

This saves the document even if the document is read-only.

This method requires that the document is currently open in your SOLIDWORKS session. It specifically checks if the document has been upgraded to the current version of the SOLIDWORKS product in this session. If it has not, then this method has no effect.

Be careful when using this method because this method attempts to change the file permissions to read-write if the file is read-only, and if successful , it overwrites the file and restores the permission to read-only. Although it may appear the file is safe because it is read-only before and after the operation, it might have been overwritten by this method.

This method was designed to be used with the ISldWorks event [DocumentConversionNotify](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.DSldWorksEvents_DocumentConversionNotifyEventHandler.html). It does not require that the notification be used, but it should work in response to that notification.

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 99 SP1, datecode 1999229