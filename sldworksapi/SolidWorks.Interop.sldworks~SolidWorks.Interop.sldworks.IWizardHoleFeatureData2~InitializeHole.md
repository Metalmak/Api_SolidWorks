<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IWizardHoleFeatureData2~InitializeHole.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InitializeHole Method (IWizardHoleFeatureData2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IWizardHoleFeatureData2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IWizardHoleFeatureData2.html) : InitializeHole Method (IWizardHoleFeatureData2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*GenericHoleType*
:   Hole type as defined in swWzdGeneralHoleTypes\_e

*StdIndex*
:   Standard as defined in swWzdHoleStandards\_e

*FastnerType*
:   Screw type as defined in swWzdHoleStandardFastenerTypes\_e

*SSize*
:   Size of the hole

*EndType*
:   End type as defined in swEndConditions\_e

Initializes a newly created Hole Wizard feature data object.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub InitializeHole( _    ByVal GenericHoleType As System.Integer, _    ByVal StdIndex As System.Integer, _    ByVal FastnerType As System.Integer, _    ByVal SSize As System.String, _    ByVal EndType As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IWizardHoleFeatureData2 Dim GenericHoleType As System.Integer Dim StdIndex As System.Integer Dim FastnerType As System.Integer Dim SSize As System.String Dim EndType As System.Integer   instance.InitializeHole(GenericHoleType, StdIndex, FastnerType, SSize, EndType) ``` | |

| C# |  |
| --- | --- |
| ``` void InitializeHole(     System.int GenericHoleType,    System.int StdIndex,    System.int FastnerType,    System.string SSize,    System.int EndType ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void InitializeHole(  &   System.int GenericHoleType, &   System.int StdIndex, &   System.int FastnerType, &   System.String^ SSize, &   System.int EndType ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*GenericHoleType*
:   Hole type as defined in swWzdGeneralHoleTypes\_e

*StdIndex*
:   Standard as defined in swWzdHoleStandards\_e

*FastnerType*
:   Screw type as defined in swWzdHoleStandardFastenerTypes\_e

*SSize*
:   Size of the hole

*EndType*
:   End type as defined in swEndConditions\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See WizardHoleFeatureData2::InitializeHole.

# ![](dotnetimages/collapse.gif)Remarks

# ![](dotnetimages/collapse.gif)See Also

####

[IWizardHoleFeatureData2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IWizardHoleFeatureData2.html)

[IWizardHoleFeatureData2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IWizardHoleFeatureData2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 FCS, Revision Number 14.0