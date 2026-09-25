<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~SetReferencedDisplayStates.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetReferencedDisplayStates Method (IComponent2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IComponent2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2.html) : SetReferencedDisplayStates Method (IComponent2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ComponentDisplayStateName*
:   Component display state name

*Option*
:   Display state option as defined in swDisplayStateOpts\_e

*AssemblyDisplayStateNames*
:   Array of assembly display state names; valid only if Option is set to swDisplayStateOpts\_e.swSpecifyDisplayState

Sets the specified display state of this component to be referenced by the specified assembly display state(s).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetReferencedDisplayStates( _    ByVal ComponentDisplayStateName As System.String, _    ByVal Option As System.Integer, _    ByVal AssemblyDisplayStateNames As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IComponent2 Dim ComponentDisplayStateName As System.String Dim Option As System.Integer Dim AssemblyDisplayStateNames As System.Object Dim value As System.Boolean   value = instance.SetReferencedDisplayStates(ComponentDisplayStateName, Option, AssemblyDisplayStateNames) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetReferencedDisplayStates(     System.string ComponentDisplayStateName,    System.int Option,    System.object AssemblyDisplayStateNames ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetReferencedDisplayStates(  &   System.String^ ComponentDisplayStateName, &   System.int Option, &   System.Object^ AssemblyDisplayStateNames ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ComponentDisplayStateName*
:   Component display state name

*Option*
:   Display state option as defined in swDisplayStateOpts\_e

*AssemblyDisplayStateNames*
:   Array of assembly display state names; valid only if Option is set to swDisplayStateOpts\_e.swSpecifyDisplayState

#### Return Value

True if component display state referenced successfully, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Component2::SetReferencedDisplayStates.

# ![](dotnetimages/collapse.gif)See Also

####

[IComponent2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2.html)

[IComponent2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2_members.html)

[IComponent2::GetReferencedDisplayStates Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetReferencedDisplayStates.html)

[IComponent2::SetVisibilityInAsmDisplayStates Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~SetVisibilityInAsmDisplayStates.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2018 FCS, Revision Number 26.0