<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShellManager~CreateShell.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| CreateShell Method (ICWShellManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWShellManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShellManager.html) : CreateShell Method (ICWShellManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DispArray*
:   Array of entities (faces or reference surfaces) to use to create the shell

Obsolete. Not superseded.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateShell( _    ByVal DispArray As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWShellManager Dim DispArray As System.Object Dim value As System.Integer   value = instance.CreateShell(DispArray) ``` | |

| C# |  |
| --- | --- |
| ``` System.int CreateShell(     System.object DispArray ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int CreateShell(  &   System.Object^ DispArray ) ``` | |

#### Parameters

*DispArray*
:   Array of entities (faces or reference surfaces) to use to create the shell

#### Return Value

Error as defined in [swsShellManagerError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsShellManagerError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWShellManager::CreateShell.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWShellManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShellManager.html)

[ICWShellManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShellManager_members.html)

[ICWShellManager::DeleteShell Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWShellManager~DeleteShell.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2008 SP1.0