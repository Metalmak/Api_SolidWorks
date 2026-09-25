<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent~GetBox.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetBox Method (IComponent) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IComponent Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent.html) : GetBox Method (IComponent) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*IncludeRefPlanes*

*IncludeSketches*

Obsolete. Superseded by [IComponent2::GetBox](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2~GetBox.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetBox( _    ByVal IncludeRefPlanes As System.Boolean, _    ByVal IncludeSketches As System.Boolean _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IComponent Dim IncludeRefPlanes As System.Boolean Dim IncludeSketches As System.Boolean Dim value As System.Object   value = instance.GetBox(IncludeRefPlanes, IncludeSketches) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetBox(     System.bool IncludeRefPlanes,    System.bool IncludeSketches ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetBox(  &   System.bool IncludeRefPlanes, &   System.bool IncludeSketches ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*IncludeRefPlanes*

*IncludeSketches*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Component::GetBox.

# ![](dotnetimages/collapse.gif)See Also

####

[IComponent Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent.html)

[IComponent Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent_members.html)