<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension~GetJogParameters.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetJogParameters Method (IDisplayDimension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDisplayDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension.html) : GetJogParameters Method (IDisplayDimension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*WitnessIndex*
:   Index of linear dimension extension line whose jog to get

*Jogged*
:   True if the linear dimension extension line is jogged, false if not

*Offset1*
:   First line segment of the linear dimension extension line

*Offset2*
:   Second line segment of the linear dimension extension line; this is the line segment that is jogged

*Offset1to2*
:   Third line segment of the linear dimension extension line

Gets the jog in a linear dimension extension line.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetJogParameters( _    ByVal WitnessIndex As System.Short, _    ByRef Jogged As System.Boolean, _    ByRef Offset1 As System.Double, _    ByRef Offset2 As System.Double, _    ByRef Offset1to2 As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDisplayDimension Dim WitnessIndex As System.Short Dim Jogged As System.Boolean Dim Offset1 As System.Double Dim Offset2 As System.Double Dim Offset1to2 As System.Double Dim value As System.Boolean   value = instance.GetJogParameters(WitnessIndex, Jogged, Offset1, Offset2, Offset1to2) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetJogParameters(     System.short WitnessIndex,    out System.bool Jogged,    out System.double Offset1,    out System.double Offset2,    out System.double Offset1to2 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetJogParameters(  &   System.short WitnessIndex, &   [Out] System.bool Jogged, &   [Out] System.double Offset1, &   [Out] System.double Offset2, &   [Out] System.double Offset1to2 ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*WitnessIndex*
:   Index of linear dimension extension line whose jog to get

*Jogged*
:   True if the linear dimension extension line is jogged, false if not

*Offset1*
:   First line segment of the linear dimension extension line

*Offset2*
:   Second line segment of the linear dimension extension line; this is the line segment that is jogged

*Offset1to2*
:   Third line segment of the linear dimension extension line

#### Return Value

True if the operation succeeds, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DisplayDimension::GetJogParameters.

# ![](dotnetimages/collapse.gif)Example

[Add and Offset Dimension Extension Lines Jogs (VBA)](Add_and_Offset_Dimension_Extension_Lines_Jogs_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IDisplayDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension.html)

[IDisplayDimension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension_members.html)

[IDisplayDimension::SetJogParameters Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension~SetJogParameters.html)

[IModelDocExtension::JogDimension Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~JogDimension.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 FCS, Revision Number 17.0