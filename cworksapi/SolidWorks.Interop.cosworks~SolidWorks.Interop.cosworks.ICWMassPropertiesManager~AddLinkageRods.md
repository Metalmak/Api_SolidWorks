<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMassPropertiesManager~AddLinkageRods.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| AddLinkageRods Method (ICWMassPropertiesManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWMassPropertiesManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMassPropertiesManager.html) : AddLinkageRods Method (ICWMassPropertiesManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NamesArray*
:   Array of the names of linkage rod connectors to add to the mass properties calculation

Adds the specified linkage rod connectors to the calculation of mass properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddLinkageRods( _    ByVal NamesArray As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWMassPropertiesManager Dim NamesArray As System.Object Dim value As System.Integer   value = instance.AddLinkageRods(NamesArray) ``` | |

| C# |  |
| --- | --- |
| ``` System.int AddLinkageRods(     System.object NamesArray ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int AddLinkageRods(  &   System.Object^ NamesArray ) ``` | |

#### Parameters

*NamesArray*
:   Array of the names of linkage rod connectors to add to the mass properties calculation

#### Return Value

Error code as defined by [swsSimMassPropertiesError\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsSimMassPropertiesError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWMassPropertiesManager::AddLinkageRods.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWMassPropertiesManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMassPropertiesManager.html)

[ICWMassPropertiesManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMassPropertiesManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2022 SP0