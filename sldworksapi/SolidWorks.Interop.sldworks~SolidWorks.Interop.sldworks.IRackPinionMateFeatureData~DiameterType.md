<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRackPinionMateFeatureData~DiameterType.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DiameterType Property (IRackPinionMateFeatureData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IRackPinionMateFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRackPinionMateFeatureData.html) : DiameterType Property (IRackPinionMateFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the type of diameter to set.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property DiameterType As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IRackPinionMateFeatureData Dim value As System.Integer   instance.DiameterType = value   value = instance.DiameterType ``` | |

| C# |  |
| --- | --- |
| ``` System.int DiameterType {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int DiameterType {    System.int get();    void set ( &   System.int value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

Type of diameter to set as defined in swRackPinionMateDistanceOptions\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See RackPinionMateFeatureData::DiameterType.

# ![](dotnetimages/collapse.gif)Example

See the [IRackPinionMateFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRackPinionMateFeatureData.html) example.

# ![](dotnetimages/collapse.gif)Remarks

For each full rotation of the pinion, the rack translates a distance = (pi \* pinion pitch diameter). Use this property to set either the pinion pitch diameter or the rack translation distance per pinion revolution.

If this property is set to swRackPinionMateDistanceOptions\_e:

* swPinionPitchDiameter, then set [IRackPinionMateFeatureData::DiameterVal](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRackPinionMateFeatureData~DiameterVal.html) with the pinion pitch diameter.* swRackTravelPerRevolution, then set IRackPinionMateFeatureData::DiameterVal with the rack translation distance per revolution of the pinion.

# ![](dotnetimages/collapse.gif)See Also

####

[IRackPinionMateFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRackPinionMateFeatureData.html)

[IRackPinionMateFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRackPinionMateFeatureData_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2019 FCS, Revision Number 27.0