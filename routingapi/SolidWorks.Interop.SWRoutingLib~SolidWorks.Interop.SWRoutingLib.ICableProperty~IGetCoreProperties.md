<!-- source: routingapi/SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.ICableProperty~IGetCoreProperties.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Routing API Help | Send comments on this topic. |
| IGetCoreProperties Method (ICableProperty) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.SWRoutingLib Namespace](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib_namespace.html) > [ICableProperty Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.ICableProperty.html) : IGetCoreProperties Method (ICableProperty) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Count*
:   Number of core properties

Gets the core properties in the cable.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetCoreProperties( _    ByRef Count As System.Integer _ ) As System.IntPtr ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICableProperty Dim Count As System.Integer Dim value As System.IntPtr   value = instance.IGetCoreProperties(Count) ``` | |

| C# |  |
| --- | --- |
| ``` System.IntPtr IGetCoreProperties(     out System.int Count ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.IntPtr IGetCoreProperties(  &   [Out] System.int Count ) ``` | |

#### Parameters

*Count*
:   Number of core properties

#### Return Value

* in-process, unmanaged C++: Pointer to an array of [core properties](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.IWireProperty.html)* VBA, VB.NET, C#, and C++/CLI: Not supported

See In-process Methods for details about this type of method.

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