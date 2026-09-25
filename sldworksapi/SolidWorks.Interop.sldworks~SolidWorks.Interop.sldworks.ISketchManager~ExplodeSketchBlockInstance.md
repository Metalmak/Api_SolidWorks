<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~ExplodeSketchBlockInstance.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ExplodeSketchBlockInstance Method (ISketchManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html) : ExplodeSketchBlockInstance Method (ISketchManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*LpSketchBlockInstance*
:   [Block instance](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchBlockInstance.html) to explode

Explodes the specified block instance.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub ExplodeSketchBlockInstance( _    ByVal LpSketchBlockInstance As SketchBlockInstance _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchManager Dim LpSketchBlockInstance As SketchBlockInstance   instance.ExplodeSketchBlockInstance(LpSketchBlockInstance) ``` | |

| C# |  |
| --- | --- |
| ``` void ExplodeSketchBlockInstance(     SketchBlockInstance LpSketchBlockInstance ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void ExplodeSketchBlockInstance(  &   SketchBlockInstance^ LpSketchBlockInstance ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*LpSketchBlockInstance*
:   [Block instance](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchBlockInstance.html) to explode

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SketchManager::ExplodeSketchBlockInstance.

# ![](dotnetimages/collapse.gif)Remarks

If this is the only or last block instance, then:

* All sketch entities in the block instances are copied to the owning sketch of the block instance.

  * Source block definition is destroyed.

See Block Definitions and Block Instances for details.

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html)

[ISketchManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager_members.html)

[ISketchBlockInstance Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchBlockInstance.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0