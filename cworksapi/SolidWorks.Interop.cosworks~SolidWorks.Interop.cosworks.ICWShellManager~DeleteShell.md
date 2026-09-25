<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShellManager~DeleteShell.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| DeleteShell Method (ICWShellManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWShellManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShellManager.html) : DeleteShell Method (ICWShellManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SName*
:   Name of the shell to delete

Deletes a shell from the study.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub DeleteShell( _    ByVal SName As System.String _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWShellManager Dim SName As System.String   instance.DeleteShell(SName) ``` | |

| C# |  |
| --- | --- |
| ``` void DeleteShell(     System.string SName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void DeleteShell(  &   System.String^ SName ) ``` | |

#### Parameters

*SName*
:   Name of the shell to delete

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWShellManager::DeleteShell.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWShellManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShellManager.html)

[ICWShellManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShellManager_members.html)

[ICWShell::Name Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShell~Name.html)

[ICWShellManager::CreateShell Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShellManager~CreateShell.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2008 SP1.0