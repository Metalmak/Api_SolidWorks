<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~PrintOut4.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| PrintOut4 Method (IModelDocExtension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : PrintOut4 Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Printer*
:   Name of the printer to which to print (see **Remarks**)

*PrintFileName*
:   Name of file to which to print (see **Remarks**)

*PrintSpecification*
:   [IPrintSpecification](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPrintSpecification.html) (see **Remarks**)

Prints this document without displaying any dialogs or message boxes.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub PrintOut4( _    ByVal Printer As System.String, _    ByVal PrintFileName As System.String, _    ByVal PrintSpecification As System.Object _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim Printer As System.String Dim PrintFileName As System.String Dim PrintSpecification As System.Object   instance.PrintOut4(Printer, PrintFileName, PrintSpecification) ``` | |

| C# |  |
| --- | --- |
| ``` void PrintOut4(     System.string Printer,    System.string PrintFileName,    System.object PrintSpecification ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void PrintOut4(  &   System.String^ Printer, &   System.String^ PrintFileName, &   System.Object^ PrintSpecification ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Printer*
:   Name of the printer to which to print (see **Remarks**)

*PrintFileName*
:   Name of file to which to print (see **Remarks**)

*PrintSpecification*
:   [IPrintSpecification](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPrintSpecification.html) (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::PrintOut4.

# ![](dotnetimages/collapse.gif)Example

[Print Drawing (VBA)](Print_Drawing_as_High_Quality_Example_VB.htm)

[Print Drawing (VB.NET)](Print_Drawing_as_High_Quality_Example_VBNET.htm)

[Print Drawing (C#)](Print_Drawing_as_High_Quality_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method supports printing parts, assemblies, and both single and multisheet drawings.

Before calling this method:

1. Call [IModelDocExtension::GetPrintSpecification](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~GetPrintSpecification.html) to get the IPrintSpecification object for this document.- Set [IPrintSpecification::PrintToFile](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrintSpecification~PrintToFile.html) to:
     * true to print to PrintFileName.* false to print to Printer.- Set other properties on the IPrintSpecification object.- Use the IPrintSpecification object to specify PrintSpecification.

If Printer, PrintFileName, and PrintSpecification are not specified, then this method prints to the default printer specified by [IModelDoc2::Printer](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~Printer.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

[IModelDoc2::PrintDirect Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~PrintDirect.html)

[IModelDoc2::PrintPreview Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~PrintPreview.html)

[IModelDoc2::ClosePrintPreview Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ClosePrintPreview.html)

[IModelDocExtension::SaveAs Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~SaveAs.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2015 FCS, Revision Number 23.0