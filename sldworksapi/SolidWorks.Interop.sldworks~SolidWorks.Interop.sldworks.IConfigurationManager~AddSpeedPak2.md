<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager~AddSpeedPak2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddSpeedPak2 Method (IConfigurationManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IConfigurationManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager.html) : AddSpeedPak2 Method (IConfigurationManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Type*
:   Selection type:

    * 1 = Geometry* 2 = Graphics

*PartThreshold*
:   1.0 >= Double value for part or body selection threshold >= 0.0; 1.0 selects nothing, and 0.0 selects all (see **Remarks**)

Creates a SpeedPak configuration that includes all faces and the specified threshold of parts or bodies for the active assembly configuration.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddSpeedPak2( _    ByVal Type As System.Integer, _    ByVal PartThreshold As System.Double _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IConfigurationManager Dim Type As System.Integer Dim PartThreshold As System.Double Dim value As System.Object   value = instance.AddSpeedPak2(Type, PartThreshold) ``` | |

| C# |  |
| --- | --- |
| ``` System.object AddSpeedPak2(     System.int Type,    System.double PartThreshold ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ AddSpeedPak2(  &   System.int Type, &   System.double PartThreshold ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Type*
:   Selection type:

    * 1 = Geometry* 2 = Graphics

*PartThreshold*
:   1.0 >= Double value for part or body selection threshold >= 0.0; 1.0 selects nothing, and 0.0 selects all (see **Remarks**)

#### Return Value

SpeedPak [configuration](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IConfiguration.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ConfigurationManager::AddSpeedPak2.

# ![](dotnetimages/collapse.gif)Example

[Create a SpeedPak Configuration (VBA)](Create_SpeedPak_Example_VB.htm)

[Create a Speedpak Configuration (VB.NET)](Create_SpeedPak_Example_VBNET.htm)

[Create a Speedpak Configuration (C#)](Create_Speedpak_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

PartThreshold corresponds to the value of the **Bodies to Include** slider on the SpeedPak PropertyManager page.

This method includes all faces in the SpeedPak configuration.

# ![](dotnetimages/collapse.gif)See Also

####

[IConfigurationManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager.html)

[IConfigurationManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager_members.html)

[IConfiguration::IsSpeedPak Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~IsSpeedPak.html)

[IConfiguration::UpdateSpeedPak Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~UpdateSpeedPak.html)

[IAssemblyDoc::CreateSpeedPak Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~CreateSpeedPak.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2013 FCS, Revision Number 21.0