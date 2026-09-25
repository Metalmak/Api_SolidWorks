<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc~PrintOut.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| PrintOut Method (IModelDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html) : PrintOut Method (IModelDoc) |

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

Obsolete. Superseded by [IModelDoc2::PrintOut](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~PrintOut.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub PrintOut( _    ByVal FromPage As System.Integer, _    ByVal ToPage As System.Integer, _    ByVal NumCopies As System.Integer, _    ByVal Collate As System.Boolean, _    ByVal Printer As System.String, _    ByVal Scale As System.Double, _    ByVal PrintToFile As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc Dim FromPage As System.Integer Dim ToPage As System.Integer Dim NumCopies As System.Integer Dim Collate As System.Boolean Dim Printer As System.String Dim Scale As System.Double Dim PrintToFile As System.Boolean   instance.PrintOut(FromPage, ToPage, NumCopies, Collate, Printer, Scale, PrintToFile) ``` | |

| C# |  |
| --- | --- |
| ``` void PrintOut(     System.int FromPage,    System.int ToPage,    System.int NumCopies,    System.bool Collate,    System.string Printer,    System.double Scale,    System.bool PrintToFile ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void PrintOut(  &   System.int FromPage, &   System.int ToPage, &   System.int NumCopies, &   System.bool Collate, &   System.String^ Printer, &   System.double Scale, &   System.bool PrintToFile ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FromPage*

*ToPage*

*NumCopies*

*Collate*

*Printer*

*Scale*

*PrintToFile*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc::PrintOut.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html)

[IModelDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc_members.html)