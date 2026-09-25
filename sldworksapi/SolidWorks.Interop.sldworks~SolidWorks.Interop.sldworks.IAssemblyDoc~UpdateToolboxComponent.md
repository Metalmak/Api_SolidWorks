<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~UpdateToolboxComponent.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| UpdateToolboxComponent Method (IAssemblyDoc) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html) : UpdateToolboxComponent Method (IAssemblyDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*AssemblyLevelToUpdate*
:   Level in which to update SOLIDWORKS Toolbox components as defined in swAssemblyLevelToUpdate\_e

Updates SOLIDWORKS Toolbox components in the specified assembly level using the current information in Toolbox settings.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function UpdateToolboxComponent( _    ByVal AssemblyLevelToUpdate As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAssemblyDoc Dim AssemblyLevelToUpdate As System.Integer Dim value As System.Integer   value = instance.UpdateToolboxComponent(AssemblyLevelToUpdate) ``` | |

| C# |  |
| --- | --- |
| ``` System.int UpdateToolboxComponent(     System.int AssemblyLevelToUpdate ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int UpdateToolboxComponent(  &   System.int AssemblyLevelToUpdate ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*AssemblyLevelToUpdate*
:   Level in which to update SOLIDWORKS Toolbox components as defined in swAssemblyLevelToUpdate\_e

#### Return Value

Status of updating the SOLIDWORKS Toolbox components as defined in swAssemblyUpdateToolboxComponentStatus\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AssemblyDoc::UpdateToolboxComponent.

# ![](dotnetimages/collapse.gif)Example

[Update All Toolbox Components (C#)](Update_All_Toolbox_Components_Example_CSharp.htm)

[Update All Toolbox Components (VB.NET)](Update_All_Toolbox_Components_Example_VBNET.htm)

[Update All Toolbox Components (VBA)](Update_All_Toolbox_Components_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html)

[IAssemblyDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2017 FCS, Revision Number 25.0