<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~IgnoreClearanceForSurfaceContact.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| IgnoreClearanceForSurfaceContact Property (ICWStaticStudyOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWStaticStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions.html) : IgnoreClearanceForSurfaceContact Property (ICWStaticStudyOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Obsolete. Superseded by [ICWStaticStudyOptions::IgnoreClearanceForSurfaceContact2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~IgnoreClearanceForSurfaceContact2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property IgnoreClearanceForSurfaceContact As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWStaticStudyOptions Dim value As System.Integer   instance.IgnoreClearanceForSurfaceContact = value   value = instance.IgnoreClearanceForSurfaceContact ``` | |

| C# |  |
| --- | --- |
| ``` System.int IgnoreClearanceForSurfaceContact {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int IgnoreClearanceForSurfaceContact {    System.int get();    void set ( &   System.int value); } ``` | |

#### Property Value

* 1 = Ignore clearance for surface contact* 0 = Do not ignore clearance for surface contact

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWStaticStudyOptions::IgnoreClearanceForSurfaceContact.

# ![](dotnetimages/collapse.gif)Example

See the [ICWStaticStudyOptions](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

You can override this setting when defining [contact sets](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWContactSet.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ICWStaticStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions.html)

[ICWStaticStudyOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions_members.html)

[ICWStaticStudyOptions::ClearanceUnit Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactSet~ClearanceUnit.html)

[ICWStaticStudyOptions::ClearanceValue Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactSet~ClearanceValue.html)

[ICWStaticStudyOptions::IncludeGlobalFriction Property ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~IncludeGlobalFriction.html)

[ICWStaticStudyOptions::NoPenetration Property ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~NoPenetration.html)

[ICWStaticStudyOptions::FrictionCoefficient Property ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStaticStudyOptions~FrictionCoefficient.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2008 SP1.0