<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrintSpecification~AddPrintRange.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddPrintRange Method (IPrintSpecification) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPrintSpecification Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrintSpecification.html) : AddPrintRange Method (IPrintSpecification) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FirstPage*
:   First page of print range

*LastPage*
:   Last page of print range

Adds a range of pages to print.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub AddPrintRange( _    ByVal FirstPage As System.Integer, _    ByVal LastPage As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPrintSpecification Dim FirstPage As System.Integer Dim LastPage As System.Integer   instance.AddPrintRange(FirstPage, LastPage) ``` | |

| C# |  |
| --- | --- |
| ``` void AddPrintRange(     System.int FirstPage,    System.int LastPage ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void AddPrintRange(  &   System.int FirstPage, &   System.int LastPage ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FirstPage*
:   First page of print range

*LastPage*
:   Last page of print range

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PrintSpecification::AddPrintRange.

# ![](dotnetimages/collapse.gif)Example

See the [IPrintSpecification](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPrintSpecification.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

Call this method multiple times to specify multiple ranges of pages to print.

# ![](dotnetimages/collapse.gif)See Also

####

[IPrintSpecification Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrintSpecification.html)

[IPrintSpecification Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrintSpecification_members.html)

[IPrintSpecification::ResetPrintRange Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrintSpecification~ResetPrintRange.html)

[IPrintSpecification::PrintRange Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrintSpecification~PrintRange.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2015 FCS, Revision Number 23.0