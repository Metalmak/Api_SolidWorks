<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~IsBackgroundProcessingCompleted.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IsBackgroundProcessingCompleted Method (ISldWorks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : IsBackgroundProcessingCompleted Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FilePath*
:   Fully qualified path and filename of the drawing document that was opened in a background process

Gets whether SOLIDWORKS has finished background processing a drawing document that requires a lot of CPU time to open.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IsBackgroundProcessingCompleted( _    ByVal FilePath As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim FilePath As System.String Dim value As System.Boolean   value = instance.IsBackgroundProcessingCompleted(FilePath) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool IsBackgroundProcessingCompleted(     System.string FilePath ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool IsBackgroundProcessingCompleted(  &   System.String^ FilePath ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FilePath*
:   Fully qualified path and filename of the drawing document that was opened in a background process

#### Return Value

True if background processing is finished, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::IsBackgroundProcessingCompleted.

# ![](dotnetimages/collapse.gif)Remarks

SOLIDWORKS recommends that you only use this method with [ISldWorks::EnableBackgroundProcessing](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~EnableBackgroundProcessing.html) and [IDrawingDoc::BackgroundProcessingOption](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDrawingDoc~BackgroundProcessingOption.html) when you can quickly open a drawing document via the user interface, but that same drawing takes significantly more time to open programmatically.

To more efficiently and programmatically open a drawing document that requires a lot of CPU time and no user input:

1. Set ISldWorks::EnableBackgroundProcessing to true.

   - Use [ISldWorks Event BackgroundProcessingStartNotify](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.DSldWorksEvents_BackgroundProcessingStartNotifyEventHandler.html) to handle the background processing start event.- Open the drawing document by calling either [ISldWorks::OpenDoc6](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~OpenDoc6.html) or [ISldWorks::OpenDoc7](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~OpenDoc7.html).- Set IDrawingDoc::BackgroundProcessingOption to swBackgroundProcessOption\_e.swBackgroundProcessing\_DeferToApplication.- Call ISldWorks::IsBackgroundProcessingCompleted repeatedly, which polls the status of the open operation, to know when background processing ends.- Use [ISldWorks Event BackgroundProcessingEndNotify](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.DSldWorksEvents_BackgroundProcessingEndNotifyEventHandler.html) to handle the background processing end event.- When the open operation is finished, set ISldWorks::EnableBackgroundProcessing to false.

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0