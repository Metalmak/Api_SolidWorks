<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~Set3DExperienceType.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Set3DExperienceType Method (IConfiguration) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IConfiguration Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration.html) : Set3DExperienceType Method (IConfiguration) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*IsPhysicalProduct*
:   True to convert this configuration to a parent configuration (Physical Product/Family), false to convert it to a derived configuration (Representation)

*RepresentationParentName*
:   Parent Physical Product/Family name of derived configuration (Representation); valid only if IsPhysicalProduct is false

Converts this configuration in SOLIDWORKS Connected.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function Set3DExperienceType( _    ByVal IsPhysicalProduct As System.Boolean, _    ByVal RepresentationParentName As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IConfiguration Dim IsPhysicalProduct As System.Boolean Dim RepresentationParentName As System.String Dim value As System.Boolean   value = instance.Set3DExperienceType(IsPhysicalProduct, RepresentationParentName) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool Set3DExperienceType(     System.bool IsPhysicalProduct,    System.string RepresentationParentName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool Set3DExperienceType(  &   System.bool IsPhysicalProduct, &   System.String^ RepresentationParentName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*IsPhysicalProduct*
:   True to convert this configuration to a parent configuration (Physical Product/Family), false to convert it to a derived configuration (Representation)

*RepresentationParentName*
:   Parent Physical Product/Family name of derived configuration (Representation); valid only if IsPhysicalProduct is false

#### Return Value

True if configuration successfully converted, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Configuration::Set3DExperienceType.

# ![](dotnetimages/collapse.gif)See Also

####

[IConfiguration Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration.html)

[IConfiguration Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration_members.html)

[IConfiguration::Get3DExperienceType Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~Get3DExperienceType.html)

[IConfiguration::AddCADFamilyConfiguration Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager~AddCADFamilyConfiguration.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2022 FCS, Revision Number 30