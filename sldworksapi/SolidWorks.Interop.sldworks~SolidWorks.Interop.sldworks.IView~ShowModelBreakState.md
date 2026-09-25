<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~ShowModelBreakState.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ShowModelBreakState Method (IView) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html) : ShowModelBreakState Method (IView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ShowIt*
:   True to display the Model Break View specified in BreakName, false to not

*BreakName*
:   Name of Model Break View to display

Sets whether to display the specified Model Break View.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ShowModelBreakState( _    ByVal ShowIt As System.Boolean, _    ByVal BreakName As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IView Dim ShowIt As System.Boolean Dim BreakName As System.String Dim value As System.Boolean   value = instance.ShowModelBreakState(ShowIt, BreakName) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ShowModelBreakState(     System.bool ShowIt,    System.string BreakName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ShowModelBreakState(  &   System.bool ShowIt, &   System.String^ BreakName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ShowIt*
:   True to display the Model Break View specified in BreakName, false to not

*BreakName*
:   Name of Model Break View to display

#### Return Value

True if successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See View::ShowModelBreakState.

# ![](dotnetimages/collapse.gif)Example

[Get and Set Model Break View Display (VBA)](Get_and_Set_Model_Break_View_Display_Example_VB.htm)

[Get and Set Model Break View Display (VB.NET)](Get_and_Set_Model_Break_View_Display_Example_VBNET.htm)

[Get and Set Model Break View Display (C#)](Get_and_Set_Model_Break_View_Display_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html)

[IView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView_members.html)

[IView::IsModelBreakState Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~IsModelBreakState.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2015 FCS, Release Number 23.0