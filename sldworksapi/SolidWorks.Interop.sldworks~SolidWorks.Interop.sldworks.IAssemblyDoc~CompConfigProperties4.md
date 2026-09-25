<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~CompConfigProperties4.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CompConfigProperties4 Method (IAssemblyDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html) : CompConfigProperties4 Method (IAssemblyDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Suppression*
:   Suppression state of this component as defined in swComponentSuppressionState\_e

*Solving*
:   Solving state of this component as defined in swComponentSolvingOption\_e

*Visibility*
:   True if you want to show the selected component in the graphics display area, false if not

*UseNamedRefConfig*
:   Not used

*RefConfigName*
:   * If a non-empty string is specified, then the referenced configuration of the selected component is changed to this named configuration* If an empty string is specified, then the default referenced configuration is used

*ExcludeFromBOM*
:   True to exclude the configuration from the BOM, false to not

Obsolete. Superseded by [IAssemblyDoc::CompConfigProperties5](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~CompConfigProperties5.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CompConfigProperties4( _    ByVal Suppression As System.Integer, _    ByVal Solving As System.Integer, _    ByVal Visibility As System.Boolean, _    ByVal UseNamedRefConfig As System.Boolean, _    ByVal RefConfigName As System.String, _    ByVal ExcludeFromBOM As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAssemblyDoc Dim Suppression As System.Integer Dim Solving As System.Integer Dim Visibility As System.Boolean Dim UseNamedRefConfig As System.Boolean Dim RefConfigName As System.String Dim ExcludeFromBOM As System.Boolean Dim value As System.Boolean   value = instance.CompConfigProperties4(Suppression, Solving, Visibility, UseNamedRefConfig, RefConfigName, ExcludeFromBOM) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool CompConfigProperties4(     System.int Suppression,    System.int Solving,    System.bool Visibility,    System.bool UseNamedRefConfig,    System.string RefConfigName,    System.bool ExcludeFromBOM ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool CompConfigProperties4(  &   System.int Suppression, &   System.int Solving, &   System.bool Visibility, &   System.bool UseNamedRefConfig, &   System.String^ RefConfigName, &   System.bool ExcludeFromBOM ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Suppression*
:   Suppression state of this component as defined in swComponentSuppressionState\_e

*Solving*
:   Solving state of this component as defined in swComponentSolvingOption\_e

*Visibility*
:   True if you want to show the selected component in the graphics display area, false if not

*UseNamedRefConfig*
:   Not used

*RefConfigName*
:   * If a non-empty string is specified, then the referenced configuration of the selected component is changed to this named configuration* If an empty string is specified, then the default referenced configuration is used

*ExcludeFromBOM*
:   True to exclude the configuration from the BOM, false to not

#### Return Value

True if setting the properties of the selected component in the specified configuration is successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AssemblyDoc::CompConfigProperties4.

# ![](dotnetimages/collapse.gif)Remarks

You can use configurations to save certain display characteristics with each of the assembly components and retrieve that configuration in the future. SOLIDWORKS applies the settings that you specify with this method to the active configuration.

You cannot set a component to lightweight.

Known reasons for failure of this method include:

* Invalid suppression state specified.* Not preselecting a component.

# ![](dotnetimages/collapse.gif)See Also

####

[IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html)

[IAssemblyDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2005 FCS, Revision Number 13