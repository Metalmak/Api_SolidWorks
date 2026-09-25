<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IsHidden.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IsHidden Method (IComponent2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IComponent2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2.html) : IsHidden Method (IComponent2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ConsiderSuppressed*
:   Controls whether suppressed components are hidden

Gets whether this component is hidden or suppressed.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IsHidden( _    ByVal ConsiderSuppressed As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IComponent2 Dim ConsiderSuppressed As System.Boolean Dim value As System.Boolean   value = instance.IsHidden(ConsiderSuppressed) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool IsHidden(     System.bool ConsiderSuppressed ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool IsHidden(  &   System.bool ConsiderSuppressed ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ConsiderSuppressed*
:   Controls whether suppressed components are hidden

#### Return Value

True or false (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Component2::IsHidden.

# ![](dotnetimages/collapse.gif)Example

[Change Material Properties (VBA)](Change_Material_Properties_Example_VB.htm)

[Get Transforms of Assembly Components (VBA)](Get_Transforms_of_Assembly_Components_Example_VB.htm)

[Get Component State (C#)](Get_Component_State_Example_CSharp.htm)

[Get Component State (VB.NET](Get_Component_State_Example_VBNET.htm)

[Get Component State (VBA)](Get_Component_State_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

The state of this component can vary based on the active configuration.

|  |  |  |  |
| --- | --- | --- | --- |
| ConsiderSuppressed | Component | Component | IsHidden |
| True | Hidden | Unsuppressed | True |
| True | Hidden | Suppressed | True |
| True | Shown | Unsuppressed | False |
| True | Shown | Suppressed | True |
| False | Hidden | Unsuppressed | True |
| False | Hidden | Suppressed | True |
| False | Shown | Unsuppressed | False |
| False | Shown | Suppressed | False |

NOTE: For lightweight components, IsHidden returns True if ConsiderSuppressed is True.

# ![](dotnetimages/collapse.gif)See Also

####

[IComponent2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2.html)

[IComponent2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2_members.html)

[IComponent2::ISetVisibility Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~ISetVisibility.html)

[IComponent2::IsSuppressed Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IsSuppressed.html)

[IComponent2::SetSuppression2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~SetSuppression2.html)

[IComponent2::SetVisibility Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~SetVisibility.html)

[IComponent2::Visible Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~Visible.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0