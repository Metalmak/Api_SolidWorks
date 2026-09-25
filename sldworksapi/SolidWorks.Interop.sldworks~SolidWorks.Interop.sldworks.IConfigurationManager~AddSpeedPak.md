<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager~AddSpeedPak.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddSpeedPak Method (IConfigurationManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IConfigurationManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager.html) : AddSpeedPak Method (IConfigurationManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Type*
:   * 1 = Geometry* 2 = Graphics

*PartThreshold*

*FaceThreshold*
:   See **Remarks**

Obsolete. Superseded by [IConfigurationManager::AddSpeedPak2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IConfigurationManager~AddSpeedPak2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddSpeedPak( _    ByVal Type As System.Integer, _    ByVal PartThreshold As System.Double, _    ByVal FaceThreshold As System.Double _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IConfigurationManager Dim Type As System.Integer Dim PartThreshold As System.Double Dim FaceThreshold As System.Double Dim value As System.Object   value = instance.AddSpeedPak(Type, PartThreshold, FaceThreshold) ``` | |

| C# |  |
| --- | --- |
| ``` System.object AddSpeedPak(     System.int Type,    System.double PartThreshold,    System.double FaceThreshold ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ AddSpeedPak(  &   System.int Type, &   System.double PartThreshold, &   System.double FaceThreshold ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Type*
:   * 1 = Geometry* 2 = Graphics

*PartThreshold*

*FaceThreshold*
:   See **Remarks**

#### Return Value

SpeedPak [configuration](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IConfiguration.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ConfigurationManager::AddSpeedPak.

# ![](dotnetimages/collapse.gif)Remarks

The SOLIDWORKS user-interface control corresponding to the FaceThreshhold parameter was removed from SOLIDWORKS 2013 and later. Regardless of the value that you specify for the FaceThreshhold parameter, the value 0 is passed, which results in no faces being included for SpeedPak by a call to this method.

This method was revised as described so that existing applications that call this method will not fail.

# ![](dotnetimages/collapse.gif)See Also

####

[IConfigurationManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager.html)

[IConfigurationManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager_members.html)

[IConfiguration::IsSpeedPak Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~IsSpeedPak.html)

[IConfiguration::UpdateSpeedPak Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~UpdateSpeedPak.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 FCS, Revision Number 17.0