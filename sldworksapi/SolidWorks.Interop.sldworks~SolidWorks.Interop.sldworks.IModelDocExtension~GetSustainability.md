<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~GetSustainability.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetSustainability Method (IModelDocExtension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : GetSustainability Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the entry-point interface to the SOLIDWORKS Sustainability API.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetSustainability() As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim value As System.Object   value = instance.GetSustainability() ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetSustainability() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetSustainability(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

ISustainabilityApp

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::GetSustainability.

# ![](dotnetimages/collapse.gif)Example

[Calculate Environmental Impact of Part (VBA)](Calculate_Environmental_Impact_of_Part_Example_VB.htm)

[Calculate Environmental Impact of Part (VB.NET)](Calculate_Environmental_Impact_of_Part_Example_VBNET.htm)

[Calculate Environmental Impact of Part (C#)](Calculate_Environmental_Impact_of_Part_Example_CSharp.htm)

[Calculate Environmental Impact of Assembly (VBA)](Calculate_Environmental_Impact_of_Assembly_Example_VB.htm)

[Calculate Environmental Impact of Assembly (VB.NET)](Calculate_Environmental_Impact_of_Assembly_Example_VBNET.htm)

[Calculate Environmental Impact of Assembly (C#)](Calculate_Environmental_Impact_of_Assembly_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

SOLIDWORKS Sustainability and its API are only available in SOLIDWORKS Professional and SOLIDWORKS Premium.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2013 FCS, Revision Number 21.0