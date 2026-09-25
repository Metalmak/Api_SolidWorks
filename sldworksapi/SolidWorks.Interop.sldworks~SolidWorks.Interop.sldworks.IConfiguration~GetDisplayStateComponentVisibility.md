<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~GetDisplayStateComponentVisibility.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetDisplayStateComponentVisibility Method (IConfiguration) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IConfiguration Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration.html) : GetDisplayStateComponentVisibility Method (IConfiguration) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DisplayStateName*
:   Name of the display state

*Onlyhidden*
:   True to only return visibilities for hidden components, false to return visibilities for all components

*ToplevelOnly*
:   True to get the top-level components only, false to get all components

*Components*
:   Array of [IComponent2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2.html)s

Gets the components and their visibilities in the specified display state.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetDisplayStateComponentVisibility( _    ByVal DisplayStateName As System.String, _    ByVal Onlyhidden As System.Boolean, _    ByVal ToplevelOnly As System.Boolean, _    ByRef Components As System.Object _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IConfiguration Dim DisplayStateName As System.String Dim Onlyhidden As System.Boolean Dim ToplevelOnly As System.Boolean Dim Components As System.Object Dim value As System.Object   value = instance.GetDisplayStateComponentVisibility(DisplayStateName, Onlyhidden, ToplevelOnly, Components) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetDisplayStateComponentVisibility(     System.string DisplayStateName,    System.bool Onlyhidden,    System.bool ToplevelOnly,    out System.object Components ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetDisplayStateComponentVisibility(  &   System.String^ DisplayStateName, &   System.bool Onlyhidden, &   System.bool ToplevelOnly, &   [Out] System.Object^ Components ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*DisplayStateName*
:   Name of the display state

*Onlyhidden*
:   True to only return visibilities for hidden components, false to return visibilities for all components

*ToplevelOnly*
:   True to get the top-level components only, false to get all components

*Components*
:   Array of [IComponent2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2.html)s

#### Return Value

Array of longs or integers indicating component visibilities; 1 if visible, 0 if hidden

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Configuration::GetDisplayStateComponentVisibility.

# ![](dotnetimages/collapse.gif)Example

[Get Display States and Visibilities of Components (C#)](Get_Display_State_Names_and_Visibilites_of_Components_Example_CSharp.htm)

[Get Display States and Visibilities of Components (VB.NET)](Get_Display_State_Names_and_Visibilites_of_Components_Example_VBNET.htm)

[Get Display States and Visibilities of Components (VBA)](Get_Display_State_Names_and_Visibilites_of_Components_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IConfiguration Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration.html)

[IConfiguration Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration_members.html)

[IConfiguration::GetDisplayStateBodyProperties Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~GetDisplayStateBodyProperties.html)

[IConfiguration::GetDisplayStateComponentProperties Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~GetDisplayStateComponentProperties.html)

[IConfiguration::GetDisplayStateFaceProperties Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~GetDisplayStateFaceProperties.html)

[IConfiguration::GetDisplayStateFeatureProperties Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~GetDisplayStateFeatureProperties.html)

[IConfiguration::GetDisplayStateProperties Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~GetDisplayStateProperties.html)

[IConfiguration::GetDisplayStates Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~GetDisplayStates.html)

[IConfiguration::GetDisplayStatesCount Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~GetDisplayStatesCount.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2015 FCS, Revision Number 23.0