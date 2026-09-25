<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~SetDontCutAllInstances.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetDontCutAllInstances Method (IDrSection) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDrSection Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection.html) : SetDontCutAllInstances Method (IDrSection) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*LpComp*
:   Pointer to the [IComponent2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2.html) object

*VbCut*
:   True if all instances of the selected component are left uncut, false if only the selected component is left uncut

Sets whether all instances of the specified component are uncut in this section view or only in the specified component.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetDontCutAllInstances( _    ByVal LpComp As Component, _    ByVal VbCut As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDrSection Dim LpComp As Component Dim VbCut As System.Boolean Dim value As System.Boolean   value = instance.SetDontCutAllInstances(LpComp, VbCut) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetDontCutAllInstances(     Component LpComp,    System.bool VbCut ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetDontCutAllInstances(  &   Component^ LpComp, &   System.bool VbCut ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*LpComp*
:   Pointer to the [IComponent2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2.html) object

*VbCut*
:   True if all instances of the selected component are left uncut, false if only the selected component is left uncut

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DrSection::SetDontCutAllInstances.

# ![](dotnetimages/collapse.gif)See Also

####

[IDrSection Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection.html)

[IDrSection Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection_members.html)

[IDrSection::GetDontCutAllInstances Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~GetDontCutAllInstances.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2005 FCS, Revision Number 13.0