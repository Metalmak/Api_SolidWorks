<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~Toolbars.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Toolbars Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : Toolbars Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*M*
:   True for main toolbar on, false for off

*Vw*
:   True for view manipulation toolbar on, false for off

*SkMain*
:   RUE for main sketch toolbar on, false for off

*Sk*
:   True for sketch entity toolbar on, false for off

*Feat*
:   True for feature toolbar on, false for off

*Constr*
:   True for relationships toolbar on, false for off

*Macro*
:   True for macro toolbar on, false for off

Turns the specified SOLIDWORKS toolbars on and off.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub Toolbars( _    ByVal M As System.Boolean, _    ByVal Vw As System.Boolean, _    ByVal SkMain As System.Boolean, _    ByVal Sk As System.Boolean, _    ByVal Feat As System.Boolean, _    ByVal Constr As System.Boolean, _    ByVal Macro As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim M As System.Boolean Dim Vw As System.Boolean Dim SkMain As System.Boolean Dim Sk As System.Boolean Dim Feat As System.Boolean Dim Constr As System.Boolean Dim Macro As System.Boolean   instance.Toolbars(M, Vw, SkMain, Sk, Feat, Constr, Macro) ``` | |

| C# |  |
| --- | --- |
| ``` void Toolbars(     System.bool M,    System.bool Vw,    System.bool SkMain,    System.bool Sk,    System.bool Feat,    System.bool Constr,    System.bool Macro ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void Toolbars(  &   System.bool M, &   System.bool Vw, &   System.bool SkMain, &   System.bool Sk, &   System.bool Feat, &   System.bool Constr, &   System.bool Macro ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*M*
:   True for main toolbar on, false for off

*Vw*
:   True for view manipulation toolbar on, false for off

*SkMain*
:   RUE for main sketch toolbar on, false for off

*Sk*
:   True for sketch entity toolbar on, false for off

*Feat*
:   True for feature toolbar on, false for off

*Constr*
:   True for relationships toolbar on, false for off

*Macro*
:   True for macro toolbar on, false for off

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::Toolbars.

# ![](dotnetimages/collapse.gif)Remarks

See [IModelDoc2::SetToolbarVisibility](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~SetToolbarVisibility.html) for control of all SOLIDWORKS toolbars.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

[IModelDoc2::GetToolbarVisibility Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~GetToolbarVisibility.html)

[ISldWorks::HideToolbar2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~HideToolbar2.html)

[ISldWorks::GetToolbarState2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetToolbarState2.html)

[ISldWorks::ShowToolbar2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~ShowToolbar2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0