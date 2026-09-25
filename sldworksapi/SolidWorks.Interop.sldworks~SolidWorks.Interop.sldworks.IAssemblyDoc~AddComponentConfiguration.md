<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~AddComponentConfiguration.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddComponentConfiguration Method (IAssemblyDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html) : AddComponentConfiguration Method (IAssemblyDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Name*
:   Name of new configuration

*Comment*
:   Comment displayed in Configuration Properties

*AlternateName*
:   Alternate configuration name; used if swConfigOption\_UseAlternateName is set to true (see **Remarks**)

*Options*
:   Combination of one or more BOOLEAN configuration options as defined in swConfigurationOptions2\_e (see Remarks)

Adds a new configuration for the last selected assembly component.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddComponentConfiguration( _    ByVal Name As System.String, _    ByVal Comment As System.String, _    ByVal AlternateName As System.String, _    ByVal Options As System.Integer _ ) As Configuration ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAssemblyDoc Dim Name As System.String Dim Comment As System.String Dim AlternateName As System.String Dim Options As System.Integer Dim value As Configuration   value = instance.AddComponentConfiguration(Name, Comment, AlternateName, Options) ``` | |

| C# |  |
| --- | --- |
| ``` Configuration AddComponentConfiguration(     System.string Name,    System.string Comment,    System.string AlternateName,    System.int Options ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Configuration^ AddComponentConfiguration(  &   System.String^ Name, &   System.String^ Comment, &   System.String^ AlternateName, &   System.int Options ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Name*
:   Name of new configuration

*Comment*
:   Comment displayed in Configuration Properties

*AlternateName*
:   Alternate configuration name; used if swConfigOption\_UseAlternateName is set to true (see **Remarks**)

*Options*
:   Combination of one or more BOOLEAN configuration options as defined in swConfigurationOptions2\_e (see Remarks)

#### Return Value

[IConfiguration](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IConfiguration.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AssemblyDoc::AddComponentConfiguration.

# ![](dotnetimages/collapse.gif)Remarks

The Options argument can be a combination of any of the following values:

* swConfigOption\_SuppressByDefault True if you want to suppress newly added features and mates in this configuration, false if not

  * swConfigOption\_HideByDefault - True if you want newly added components to be hidden, false if not

    * swConfigOption\_MinFeatureManager True if you want newly added components to only display their component name in the FeatureManager design tree, false if you want newly added components to display their name and each of their features in the FeatureManager design tree

      * swConfigOption\_DontActivate - True if you do not want the new configuration activated, false if not

# ![](dotnetimages/collapse.gif)See Also

####

[IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html)

[IAssemblyDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2005 FCS, Revision Number 13