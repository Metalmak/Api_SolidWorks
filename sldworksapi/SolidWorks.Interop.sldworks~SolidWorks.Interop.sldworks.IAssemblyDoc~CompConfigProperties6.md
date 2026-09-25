<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~CompConfigProperties6.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CompConfigProperties6 Method (IAssemblyDoc) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html) : CompConfigProperties6 Method (IAssemblyDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Suppression*
:   Suppression state of the selected component as defined in swComponentSuppressionState\_e

*Solving*
:   Solving state of the selected component as defined in swComponentSolvingOption\_e

*Visibility*
:   True if you want to show the selected component in the graphics area, false if not

*UseNamedRefConfig*
:   Not used

*RefConfigName*
:   * If a non-empty string is specified, then the referenced configuration of the selected component is changed to this named configuration* If an empty string is specified, then the default referenced configuration is used

*ExcludeFromBOM*
:   True to exclude the configuration from the BOM, false to not

*IsEnvelope*
:   True if the selected component is an envelope, false if not

*SaveAssemblyAsPartOption*
:   Option for the selected component when saving this assembly as a part as defined in swASMSLDPRTCompPref\_e

Sets the properties for the selected [component](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2.html) in the specified [configuration](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CompConfigProperties6( _    ByVal Suppression As System.Integer, _    ByVal Solving As System.Integer, _    ByVal Visibility As System.Boolean, _    ByVal UseNamedRefConfig As System.Boolean, _    ByVal RefConfigName As System.String, _    ByVal ExcludeFromBOM As System.Boolean, _    ByVal IsEnvelope As System.Boolean, _    ByVal SaveAssemblyAsPartOption As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAssemblyDoc Dim Suppression As System.Integer Dim Solving As System.Integer Dim Visibility As System.Boolean Dim UseNamedRefConfig As System.Boolean Dim RefConfigName As System.String Dim ExcludeFromBOM As System.Boolean Dim IsEnvelope As System.Boolean Dim SaveAssemblyAsPartOption As System.Integer Dim value As System.Boolean   value = instance.CompConfigProperties6(Suppression, Solving, Visibility, UseNamedRefConfig, RefConfigName, ExcludeFromBOM, IsEnvelope, SaveAssemblyAsPartOption) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool CompConfigProperties6(     System.int Suppression,    System.int Solving,    System.bool Visibility,    System.bool UseNamedRefConfig,    System.string RefConfigName,    System.bool ExcludeFromBOM,    System.bool IsEnvelope,    System.int SaveAssemblyAsPartOption ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool CompConfigProperties6(  &   System.int Suppression, &   System.int Solving, &   System.bool Visibility, &   System.bool UseNamedRefConfig, &   System.String^ RefConfigName, &   System.bool ExcludeFromBOM, &   System.bool IsEnvelope, &   System.int SaveAssemblyAsPartOption ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Suppression*
:   Suppression state of the selected component as defined in swComponentSuppressionState\_e

*Solving*
:   Solving state of the selected component as defined in swComponentSolvingOption\_e

*Visibility*
:   True if you want to show the selected component in the graphics area, false if not

*UseNamedRefConfig*
:   Not used

*RefConfigName*
:   * If a non-empty string is specified, then the referenced configuration of the selected component is changed to this named configuration* If an empty string is specified, then the default referenced configuration is used

*ExcludeFromBOM*
:   True to exclude the configuration from the BOM, false to not

*IsEnvelope*
:   True if the selected component is an envelope, false if not

*SaveAssemblyAsPartOption*
:   Option for the selected component when saving this assembly as a part as defined in swASMSLDPRTCompPref\_e

#### Return Value

True if setting the properties of the selected component in the specified configuration is successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AssemblyDoc::CompConfigProperties6.

# ![](dotnetimages/collapse.gif)Example

[Change Component to Envelope (VBA)](Change_Component_to_Envelope_Example_VB.htm)

[Change Component to Envelope (VB.NET)](Change_Component_to_Envelope_Example_VBNET.htm)

[Change Component to Envelope (C#)](Change_Component_to_Envelope_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

You can use configurations to save certain display characteristics with each of the assembly components and retrieve that configuration in the future. SOLIDWORKS applies the settings that you specify with this method to the active configuration.

You cannot set the selected component to lightweight using this method.

Known reasons for failure of this method include:

* Invalid suppression state specified in Suppression.* Not pre-selecting the component.

# ![](dotnetimages/collapse.gif)See Also

####

[IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html)

[IAssemblyDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc_members.html)

[IComponent2::ExcludeFromBOM Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~ExcludeFromBOM.html)

[IComponent2::Solving Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~Solving.html)

[IComponent2::Visible Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~Visible.html)

[IComponent2::ReferencedConfiguration Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~ReferencedConfiguration.html)

[IComponent2::IsEnvelope Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IsEnvelope.html)

[IComponent2::SetSuppression2 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~SetSuppression2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2019 FCS, Revision Number 27.0