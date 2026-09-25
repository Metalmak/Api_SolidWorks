<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IWizardHoleFeatureData2~ChangeStandard.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ChangeStandard Method (IWizardHoleFeatureData2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IWizardHoleFeatureData2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IWizardHoleFeatureData2.html) : ChangeStandard Method (IWizardHoleFeatureData2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Standard*
:   Standard as defined in swWzdHoleStandards\_e

*FastenerType*
:   Fastener type as defined in swWzdHoleStandardFastenerTypes\_e

*SSize*
:   Fastener size

Sets the standard for all of the parameters of the Hole Wizard feature that are driven by the database.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ChangeStandard( _    ByVal Standard As System.Integer, _    ByVal FastenerType As System.Integer, _    ByVal SSize As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IWizardHoleFeatureData2 Dim Standard As System.Integer Dim FastenerType As System.Integer Dim SSize As System.String Dim value As System.Boolean   value = instance.ChangeStandard(Standard, FastenerType, SSize) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ChangeStandard(     System.int Standard,    System.int FastenerType,    System.string SSize ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ChangeStandard(  &   System.int Standard, &   System.int FastenerType, &   System.String^ SSize ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Standard*
:   Standard as defined in swWzdHoleStandards\_e

*FastenerType*
:   Fastener type as defined in swWzdHoleStandardFastenerTypes\_e

*SSize*
:   Fastener size

#### Return Value

True if the standard is changed, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See WizardHoleFeatureData2::ChangeStandard.

# ![](dotnetimages/collapse.gif)Remarks

Use this method to change [fastener size](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IWizardHoleFeatureData2~FastenerSize.html), [fastener type](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IWizardHoleFeatureData2~FastenerType2.html), and [design standard](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IWizardHoleFeatureData2~Standard2.html) of a Hole Wizard feature.

If changing the standard requires you to change the type, then you must call [IWizardHoleFeatureData2::Type](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IWizardHoleFeatureData2~Type.html) before calling IWizardHoleFeatureData2::ChangeStandard.

# ![](dotnetimages/collapse.gif)See Also

####

[IWizardHoleFeatureData2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IWizardHoleFeatureData2.html)

[IWizardHoleFeatureData2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IWizardHoleFeatureData2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2005 SP3, Revision Number 13.3