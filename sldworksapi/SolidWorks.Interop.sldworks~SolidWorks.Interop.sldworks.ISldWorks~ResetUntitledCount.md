<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~ResetUntitledCount.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ResetUntitledCount Method (ISldWorks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : ResetUntitledCount Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*PartValue*
:   Starting index for part documents

*AssemValue*
:   Starting index for assembly documents

*DrawingValue*
:   Starting index for drawing documents

Resets the index of untitled documents.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ResetUntitledCount( _    ByVal PartValue As System.Integer, _    ByVal AssemValue As System.Integer, _    ByVal DrawingValue As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim PartValue As System.Integer Dim AssemValue As System.Integer Dim DrawingValue As System.Integer Dim value As System.Integer   value = instance.ResetUntitledCount(PartValue, AssemValue, DrawingValue) ``` | |

| C# |  |
| --- | --- |
| ``` System.int ResetUntitledCount(     System.int PartValue,    System.int AssemValue,    System.int DrawingValue ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int ResetUntitledCount(  &   System.int PartValue, &   System.int AssemValue, &   System.int DrawingValue ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*PartValue*
:   Starting index for part documents

*AssemValue*
:   Starting index for assembly documents

*DrawingValue*
:   Starting index for drawing documents

#### Return Value

Total number of successful resets

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::ResetUntitledCount

# ![](dotnetimages/collapse.gif)Example

[Reset Untitled Document Count (VBA)](Reset_Untitled_Document_Count_Example_VB.htm)

[Reset Untitled Document Count (VB.NET)](Reset_Untitled_Document_Count_Example_VBNET.htm)

[Reset Untitled Document Count (C#)](Reset_Untitled_Document_Count_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Use this method to reset untitled document indexes so that playbacks of the macro recorder increment untitled documents in a reproducible fashion.

For example, if the first playback of a macro creates Part1 and Part2, then the second playback may fail because it creates Part3 and Part4 instead of Part1 and Part2.

To ensure reproducible results, call ISldWorks::ResetUntitledCount at the beginning or end of a macro program.

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 SP1, Revision Number 17.1