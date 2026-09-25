<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShell~SetFavMaterial2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetFavMaterial2 Method (ICWShell) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWShell Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShell.html) : SetFavMaterial2 Method (ICWShell) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NFav*
:   1 <= index of material in favorites list <= 100 (see **Remarks**)

Applies the specified material from the material favorites list.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetFavMaterial2( _    ByVal NFav As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWShell Dim NFav As System.Integer Dim value As System.Boolean   value = instance.SetFavMaterial2(NFav) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetFavMaterial2(     System.int NFav ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetFavMaterial2(  &   System.int NFav ) ``` | |

#### Parameters

*NFav*
:   1 <= index of material in favorites list <= 100 (see **Remarks**)

#### Return Value

-1 or true if material applied successfully, 0 or false if not

# ![](dotnetimages/collapse.gif)Remarks

The list of material favorites appears when you right-click a component in the Simulation study tree and click **Apply Favorite Material**.

This method is not valid if [ICWShell::Formulation](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShell~Formulation.html) is set to [swsShellFormulation\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsShellFormulation_e.html).swsShellFormulationComposite. To set the material of composite shell plies, you must:

1. Use [ICWShell::CompositeOptions](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShell~CompositeOptions.html) to get an instance of [ICWCompositeShellOptions](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCompositeShellOptions.html).- Call [ICWCompositeShellOptions::SetPlyParameters](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCompositeShellOptions~SetPlyParameters.html) to set a ply's material.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWShell Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShell.html)

[ICWShell Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShell_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2022 FCS, Revision Number 30