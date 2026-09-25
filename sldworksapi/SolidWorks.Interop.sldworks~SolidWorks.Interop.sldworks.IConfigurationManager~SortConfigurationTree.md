<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager~SortConfigurationTree.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SortConfigurationTree Method (IConfigurationManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IConfigurationManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager.html) : SortConfigurationTree Method (IConfigurationManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*InSelType*
:   Order in which to list configurations in the ConfigurationManager as defined in swConfigTreeSortType\_e

Specifies the order in which to list configurations in the ConfigurationManager.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SortConfigurationTree( _    ByVal InSelType As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IConfigurationManager Dim InSelType As System.Integer   instance.SortConfigurationTree(InSelType) ``` | |

| C# |  |
| --- | --- |
| ``` void SortConfigurationTree(     System.int InSelType ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SortConfigurationTree(  &   System.int InSelType ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*InSelType*
:   Order in which to list configurations in the ConfigurationManager as defined in swConfigTreeSortType\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ConfigurationManager::SortConfigurationTree.

# ![](dotnetimages/collapse.gif)Example

[Specify Order of Configurations (C#)](Specify_Order_of_Configurations_Example_CSharp.htm)

[Specify Order of Configurations (VB.NET)](Specify_Order_of_Configurations_Example_VBNET.htm)

[Specify Order of Configurations (VBA)](Specify_Order_of_Configurations_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IConfigurationManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager.html)

[IConfigurationManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2017 FCS, Revision Number 25.0