<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITriadManipulator~SetColorRefAtIndex.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetColorRefAtIndex Method (ITriadManipulator) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ITriadManipulator Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITriadManipulator.html) : SetColorRefAtIndex Method (ITriadManipulator) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Index*
:   Control whose color to set as defined in swTriadManipulatorControlPoints\_e

*ColorRef*
:   COLORREF value

Sets the colors of the controls of a triad manipulator.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetColorRefAtIndex( _    ByVal Index As System.Integer, _    ByVal ColorRef As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ITriadManipulator Dim Index As System.Integer Dim ColorRef As System.Integer   instance.SetColorRefAtIndex(Index, ColorRef) ``` | |

| C# |  |
| --- | --- |
| ``` void SetColorRefAtIndex(     System.int Index,    System.int ColorRef ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetColorRefAtIndex(  &   System.int Index, &   System.int ColorRef ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Index*
:   Control whose color to set as defined in swTriadManipulatorControlPoints\_e

*ColorRef*
:   COLORREF value

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See TriadManipulator::SetColorRefAtIndex.

# ![](dotnetimages/collapse.gif)See Also

####

[ITriadManipulator Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITriadManipulator.html)

[ITriadManipulator Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITriadManipulator_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0