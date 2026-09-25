<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~SetComponentState.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetComponentState Method (IAssemblyDoc) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html) : SetComponentState Method (IAssemblyDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SuppressionState*
:   Component suppression state as defined in swComponentSuppressionState\_e (see **Remarks**)

*CompArr*
:   Array of [components](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2.html) to change

*ConfigOption*
:   Configuration option as defined in swInConfigurationOpts\_e

*WhichConfig*
:   Name of the configuration to change

*SaveClosedDocs*
:   True saves closed documents, false does not

Sets the suppression state for the specified components.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetComponentState( _    ByVal SuppressionState As System.Integer, _    ByVal CompArr As System.Object, _    ByVal ConfigOption As System.Integer, _    ByVal WhichConfig As System.String, _    ByVal SaveClosedDocs As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAssemblyDoc Dim SuppressionState As System.Integer Dim CompArr As System.Object Dim ConfigOption As System.Integer Dim WhichConfig As System.String Dim SaveClosedDocs As System.Boolean Dim value As System.Boolean   value = instance.SetComponentState(SuppressionState, CompArr, ConfigOption, WhichConfig, SaveClosedDocs) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetComponentState(     System.int SuppressionState,    System.object CompArr,    System.int ConfigOption,    System.string WhichConfig,    System.bool SaveClosedDocs ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetComponentState(  &   System.int SuppressionState, &   System.Object^ CompArr, &   System.int ConfigOption, &   System.String^ WhichConfig, &   System.bool SaveClosedDocs ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*SuppressionState*
:   Component suppression state as defined in swComponentSuppressionState\_e (see **Remarks**)

*CompArr*
:   Array of [components](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2.html) to change

*ConfigOption*
:   Configuration option as defined in swInConfigurationOpts\_e

*WhichConfig*
:   Name of the configuration to change

*SaveClosedDocs*
:   True saves closed documents, false does not

#### Return Value

True if the components were changed, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AssemblyDoc::SetComponentState.

# ![](dotnetimages/collapse.gif)Example

[Set Component State (VBA)](Set_Component_State_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

You cannot set a component to lightweight using this method. Instead, use [IComponent::SetSuppression2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2~SetSuppression2.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html)

[IAssemblyDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc_members.html)

[IAssemblyDoc::SetComponentState Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~SetComponentState.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2003 FCS, Revision Number 11.0