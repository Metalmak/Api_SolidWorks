<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep~SetExplodeDirection.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetExplodeDirection Method (IExplodeStep) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IExplodeStep Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep.html) : SetExplodeDirection Method (IExplodeStep) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ExplodeDirection*
:   Explode direction entity

*ExplDirIndex*
:   Explode direction manipulator index as defined in swExplodeDirectionIndex\_e; valid only for regular explode steps

Sets the explode direction (manipulator index and entity) for this explode step.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetExplodeDirection( _    ByVal ExplodeDirection As System.Object, _    ByVal ExplDirIndex As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IExplodeStep Dim ExplodeDirection As System.Object Dim ExplDirIndex As System.Integer   instance.SetExplodeDirection(ExplodeDirection, ExplDirIndex) ``` | |

| C# |  |
| --- | --- |
| ``` void SetExplodeDirection(     System.object ExplodeDirection,    System.int ExplDirIndex ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetExplodeDirection(  &   System.Object^ ExplodeDirection, &   System.int ExplDirIndex ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ExplodeDirection*
:   Explode direction entity

*ExplDirIndex*
:   Explode direction manipulator index as defined in swExplodeDirectionIndex\_e; valid only for regular explode steps

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ExplodeStep::SetExplodeDirection.

# ![](dotnetimages/collapse.gif)Example

See the [IExplodeStep](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[IExplodeStep Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep.html)

[IExplodeStep Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep_members.html)

[IExplodeStep::GetExplodeDirection Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExplodeStep~GetExplodeDirection.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2018 FCS, Revision Number 26.0