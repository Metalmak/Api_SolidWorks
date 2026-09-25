<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartExplodeStep~GetExplodeDirection.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetExplodeDirection Method (IPartExplodeStep) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPartExplodeStep Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartExplodeStep.html) : GetExplodeDirection Method (IPartExplodeStep) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ExplDirIndex*
:   Explode direction manipulator index as defined in swExplodeDirectionIndex\_e

Gets the explode direction (manipulator index and entity) for this explode step.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetExplodeDirection( _    ByRef ExplDirIndex As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPartExplodeStep Dim ExplDirIndex As System.Integer Dim value As System.Object   value = instance.GetExplodeDirection(ExplDirIndex) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetExplodeDirection(     out System.int ExplDirIndex ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetExplodeDirection(  &   [Out] System.int ExplDirIndex ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ExplDirIndex*
:   Explode direction manipulator index as defined in swExplodeDirectionIndex\_e

#### Return Value

Explode direction entity (e.g., [IEdge](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge.html), [IFace2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2.html), [IRefAxis](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefAxis.html)); Nothing or null if an explode direction entity was not selected during creation of this explode step

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PartExplodeStep::GetExplodeDirection.

# ![](dotnetimages/collapse.gif)See Also

####

[IPartExplodeStep Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartExplodeStep.html)

[IPartExplodeStep Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartExplodeStep_members.html)

[IPartExplodeStep::SetExplodeDirection Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartExplodeStep~SetExplodeDirection.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2020 FCS, Revision Number 28.0