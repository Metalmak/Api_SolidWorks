<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~SetVisibilityInAsmDisplayStates.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetVisibilityInAsmDisplayStates Method (IComponent2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IComponent2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2.html) : SetVisibilityInAsmDisplayStates Method (IComponent2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*HideComponent*
:   Visibility as defined in swComponentVisibilityState\_e

*Option*
:   Display state option as defined in swDisplayStateOpts\_e

*AssemblyDisplayStateNames*
:   Array of assembly display state names; valid only if Option is set to swDisplayStateOpts\_e.swSpecifyDisplayState

Sets the visibility of this component in the specified assembly display state(s).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetVisibilityInAsmDisplayStates( _    ByVal HideComponent As System.Integer, _    ByVal Option As System.Integer, _    ByVal AssemblyDisplayStateNames As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IComponent2 Dim HideComponent As System.Integer Dim Option As System.Integer Dim AssemblyDisplayStateNames As System.Object Dim value As System.Boolean   value = instance.SetVisibilityInAsmDisplayStates(HideComponent, Option, AssemblyDisplayStateNames) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetVisibilityInAsmDisplayStates(     System.int HideComponent,    System.int Option,    System.object AssemblyDisplayStateNames ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetVisibilityInAsmDisplayStates(  &   System.int HideComponent, &   System.int Option, &   System.Object^ AssemblyDisplayStateNames ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*HideComponent*
:   Visibility as defined in swComponentVisibilityState\_e

*Option*
:   Display state option as defined in swDisplayStateOpts\_e

*AssemblyDisplayStateNames*
:   Array of assembly display state names; valid only if Option is set to swDisplayStateOpts\_e.swSpecifyDisplayState

#### Return Value

True if visibility successfully set, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Component2::SetVisibilityInAsmDisplayStates.

# ![](dotnetimages/collapse.gif)See Also

####

[IComponent2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2.html)

[IComponent2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2_members.html)

[IComponent2::SetReferencedDisplayStates Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~SetReferencedDisplayStates.html)

[IComponent2::GetVisibilityInAsmDisplayStates Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetVisibilityInAsmDisplayStates.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2018 FCS, Revision Number 26.0