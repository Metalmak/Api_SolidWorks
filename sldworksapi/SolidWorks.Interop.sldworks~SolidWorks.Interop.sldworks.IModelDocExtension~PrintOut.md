<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~PrintOut.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| PrintOut Method (IModelDocExtension) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : PrintOut Method (IModelDocExtension) |

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

*Copies*

*Collate*

*Printer*

*PrintFileName*

Obsolete. Superseded by [IModelDocExtension::PrintOut2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~PrintOut2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub PrintOut( _    ByVal FromPage As System.Integer, _    ByVal ToPage As System.Integer, _    ByVal Copies As System.Integer, _    ByVal Collate As System.Boolean, _    ByVal Printer As System.String, _    ByVal PrintFileName As System.String _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim FromPage As System.Integer Dim ToPage As System.Integer Dim Copies As System.Integer Dim Collate As System.Boolean Dim Printer As System.String Dim PrintFileName As System.String   instance.PrintOut(FromPage, ToPage, Copies, Collate, Printer, PrintFileName) ``` | |

| C# |  |
| --- | --- |
| ``` void PrintOut(     System.int FromPage,    System.int ToPage,    System.int Copies,    System.bool Collate,    System.string Printer,    System.string PrintFileName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void PrintOut(  &   System.int FromPage, &   System.int ToPage, &   System.int Copies, &   System.bool Collate, &   System.String^ Printer, &   System.String^ PrintFileName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FromPage*

*ToPage*

*Copies*

*Collate*

*Printer*

*PrintFileName*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::PrintOut.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)