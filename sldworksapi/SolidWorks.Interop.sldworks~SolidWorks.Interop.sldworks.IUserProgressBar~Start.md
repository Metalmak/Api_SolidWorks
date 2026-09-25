<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IUserProgressBar~Start.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Start Method (IUserProgressBar) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IUserProgressBar Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IUserProgressBar.html) : Start Method (IUserProgressBar) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*LowerBound*
:   Lower bound of range

*UpperBound*
:   Upper bound of range

*ProgressBarTitle*
:   Title of progress indicator to show in status bar

Sets the range of the progress indicator display and shows it on the SOLIDWORKS status bar.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function Start( _    ByVal LowerBound As System.Integer, _    ByVal UpperBound As System.Integer, _    ByVal ProgressBarTitle As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IUserProgressBar Dim LowerBound As System.Integer Dim UpperBound As System.Integer Dim ProgressBarTitle As System.String Dim value As System.Boolean   value = instance.Start(LowerBound, UpperBound, ProgressBarTitle) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool Start(     System.int LowerBound,    System.int UpperBound,    System.string ProgressBarTitle ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool Start(  &   System.int LowerBound, &   System.int UpperBound, &   System.String^ ProgressBarTitle ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*LowerBound*
:   Lower bound of range

*UpperBound*
:   Upper bound of range

*ProgressBarTitle*
:   Title of progress indicator to show in status bar

#### Return Value

True if progress indicator successfully started, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See UserProgressBar::Start.

# ![](dotnetimages/collapse.gif)Example

See the [IUserProgressBar](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IUserProgressBar.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[IUserProgressBar Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IUserProgressBar.html)

[IUserProgressBar Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IUserProgressBar_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0