<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~PrintOut2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| PrintOut2 Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : PrintOut2 Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FromPage*

*ToPage*

*NumCopies*

*Collate*

*Printer*

*Scale*

*PrintToFile*

*PtfName*

Obsolete. Superseded by [IModelDocExtension::PrintOut2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~PrintOut2.html) and [IModelDocExtension::IPrintOut2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~IPrintOut2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub PrintOut2( _    ByVal FromPage As System.Integer, _    ByVal ToPage As System.Integer, _    ByVal NumCopies As System.Integer, _    ByVal Collate As System.Boolean, _    ByVal Printer As System.String, _    ByVal Scale As System.Double, _    ByVal PrintToFile As System.Boolean, _    ByVal PtfName As System.String _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim FromPage As System.Integer Dim ToPage As System.Integer Dim NumCopies As System.Integer Dim Collate As System.Boolean Dim Printer As System.String Dim Scale As System.Double Dim PrintToFile As System.Boolean Dim PtfName As System.String   instance.PrintOut2(FromPage, ToPage, NumCopies, Collate, Printer, Scale, PrintToFile, PtfName) ``` | |

| C# |  |
| --- | --- |
| ``` void PrintOut2(     System.int FromPage,    System.int ToPage,    System.int NumCopies,    System.bool Collate,    System.string Printer,    System.double Scale,    System.bool PrintToFile,    System.string PtfName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void PrintOut2(  &   System.int FromPage, &   System.int ToPage, &   System.int NumCopies, &   System.bool Collate, &   System.String^ Printer, &   System.double Scale, &   System.bool PrintToFile, &   System.String^ PtfName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FromPage*

*ToPage*

*NumCopies*

*Collate*

*Printer*

*Scale*

*PrintToFile*

*PtfName*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::PrintOut2.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)