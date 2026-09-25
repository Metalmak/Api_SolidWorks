<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~AlternateName.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AlternateName Property (IConfiguration) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IConfiguration Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration.html) : AlternateName Property (IConfiguration) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the configuration's alternate name (i.e., user-specified name).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property AlternateName As System.String ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IConfiguration Dim value As System.String   instance.AlternateName = value   value = instance.AlternateName ``` | |

| C# |  |
| --- | --- |
| ``` System.string AlternateName {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.String^ AlternateName {    System.String^ get();    void set ( &   System.String^ value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

Alternate or user-specified name for the configuration

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Configuration::AlternateName.

# ![](dotnetimages/collapse.gif)Example

[Change Configuration Properties (VBA)](Change_Configuration_Properties_Example_VB.htm)

[Traverse Hierarchy of Configurations (VBA)](Traverse_Hierarchy_of_Configurations_Example_VB.htm)

[Get List of Configurations (C#)](Get_List_Of_Configurations_Example_CSharp.htm)

[Get List of Configurations (VB.NET)](Get_List_Of_Configurations_Example_VBNET.htm)

[Get List of Configurations (VBA)](Get_List_Of_Configurations_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

To display the configuration's alternate name as the part number in the bill of materials, use [IConfiguration::UseAlternateNameInBOM](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IConfiguration~UseAlternateNameInBOM.html).

Configuration names must not contain any special characters reserved by SOLIDWORKS.

If you specify [IConfiguration::BOMPartNoSource](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~BOMPartNoSource.html) with anything other than swBOMPartNumberSource\_e.swBOMPartNumber\_UserSpecified, then this property is set to an empty string.

# ![](dotnetimages/collapse.gif)See Also

####

[IConfiguration Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration.html)

[IConfiguration Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration_members.html)

[IConfiguration::Name Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~Name.html)