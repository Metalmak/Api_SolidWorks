<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITextFormat~IsHeightSpecifiedInPts.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IsHeightSpecifiedInPts Method (ITextFormat) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ITextFormat Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITextFormat.html) : IsHeightSpecifiedInPts Method (ITextFormat) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets whether the character height is in points or system units.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IsHeightSpecifiedInPts() As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ITextFormat Dim value As System.Boolean   value = instance.IsHeightSpecifiedInPts() ``` | |

| C# |  |
| --- | --- |
| ``` System.bool IsHeightSpecifiedInPts() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool IsHeightSpecifiedInPts(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

True if the character height is in points, false if it is in system units

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See TextFormat::IsHeightSpecifiedInPts.

# ![](dotnetimages/collapse.gif)Example

[Get All Elements in Sketch (VBA)](Get_All_Elements_of_Sketch_Example_VB.htm)

[Get Note Text Formatting Properties (VBA)](Get_Note_Text_Formatting_Properties_Example_VB.htm)

[Get Arrow in Projected View (C#)](Get_Arrow_in_Projected_View_Example_CSharp.htm)

[Get Arrow in Projected View (VB.NET)](Get_Arrow_in_Projected_View_Example_VBNET.htm)

[Get Arrow in Projected View (VBA)](Get_Arrow_in_Projected_View_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

|  |  |
| --- | --- |
| **If the font height was set using...** | **Then this method returns...** |
| [ITextFormat::CharHeight](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ITextFormat~CharHeight.html) | False |
| [ITextFormat::CharHeightInPts](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ITextFormat~CharHeightInPts.html) | True |

# ![](dotnetimages/collapse.gif)See Also

####

[ITextFormat Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITextFormat.html)

[ITextFormat Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITextFormat_members.html)