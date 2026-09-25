<!-- source: routingapi/SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.ICableProperty~GetCorePropertyCount.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Routing API Help | Send comments on this topic. |
| GetCorePropertyCount Method (ICableProperty) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.SWRoutingLib Namespace](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib_namespace.html) > [ICableProperty Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.ICableProperty.html) : GetCorePropertyCount Method (ICableProperty) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the number of core properties in the cable.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetCorePropertyCount() As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICableProperty Dim value As System.Integer   value = instance.GetCorePropertyCount() ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetCorePropertyCount() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetCorePropertyCount(); ``` | |

#### Return Value

Number of core properties

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CableProperty::GetCorePropertyCount.

# ![](dotnetimages/collapse.gif)Example

See the [ICableProperty](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.ICableProperty.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

Call this method before calling [ICableProperty::IGetCoreProperties](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.ICableProperty~IGetCoreProperties.html) to determine the size of the array for the cores for that method.

# ![](dotnetimages/collapse.gif)See Also

####

[ICableProperty Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.ICableProperty.html)

[ICableProperty Members](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.ICableProperty_members.html)

[ICableProperty::GetCoreProperties Method](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.ICableProperty~GetCoreProperties.html)

[ICable::GetCores Method](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.ICable~GetCores.html)

[ICable::GetCoresCount Method](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.ICable~GetCoresCount.html)

[ICable::IGetCores Method](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.ICable~IGetCores.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Routing 2006 FCS