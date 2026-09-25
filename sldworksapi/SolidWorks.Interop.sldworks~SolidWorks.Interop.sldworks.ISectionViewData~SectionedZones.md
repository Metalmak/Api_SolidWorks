<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISectionViewData~SectionedZones.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SectionedZones Property (ISectionViewData) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISectionViewData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISectionViewData.html) : SectionedZones Property (ISectionViewData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the intersection zones that define how to section this section view.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property SectionedZones As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISectionViewData Dim value As System.Integer   instance.SectionedZones = value   value = instance.SectionedZones ``` | |

| C# |  |
| --- | --- |
| ``` System.int SectionedZones {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int SectionedZones {    System.int get();    void set ( &   System.int value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

Intersection zones as defined in swZonalSectionViewZones\_e (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SectionViewData::SectionedZones.

# ![](dotnetimages/collapse.gif)Example

[Selectively and Transparently Section a Section View (C#)](Selectively_and_Transparently_Section_a_Section_View_Example_CSharp.htm)

[Selectively and Transparently Section a Section View (VB.NET)](Selectively_and_Transparently_Section_a_Section_View_Example_VBNET.htm)

[Selectively and Transparently Section a Section View (VBA)](Selectively_and_Transparently_Section_a_Section_View_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

In the SOLIDWORKS API, zones are defined by the intersections of the sectioning planes. This table describes the intersection zones and the enumerators to which they correspond.

| Number of sectioning planes | Zones | Intersection zones | swZonalSectionViewZones\_e enumerators |
| --- | --- | --- | --- |
| 1 | 1 | Front side of sectioning plane 1 | swZonalSectionViewZones\_swZonalSectionViewZone\_1 |
|  | 2 | Back side of sectioning plane 2 | swZonalSectionViewZones\_swZonalSectionViewZone\_2 |
| 2 | 1 | * Front side of sectioning plane 1* Front side of sectioning plane 2 | swZonalSectionViewZones\_swZonalSectionViewZone\_1 |
|  | 2 | * Back side of sectioning plane 1* Front side of sectioning plane 2 | swZonalSectionViewZones\_swZonalSectionViewZone\_2 |
|  | 3 | * Front side of sectioning plane 1* Back side of sectioning plane 2 | swZonalSectionViewZones\_swZonalSectionViewZone\_3 |
|  | 4 | * Back side of sectioning plane 1* Back side of sectioning plane 2 | swZonalSectionViewZones\_swZonalSectionViewZone\_4 |
| 3 | 1 | * Front side of sectioning plane 1* Front side of sectioning plane 2* Front side of sectioning plane 3 | swZonalSectionViewZones\_swZonalSectionViewZone\_1 |
|  | 2 | * Back side of sectioning plane 1* Front side of sectioning plane 2* Front side of sectioning plane 3 | swZonalSectionViewZones\_swZonalSectionViewZone\_2 |
|  | 3 | * Front side of sectioning plane 1* Back side of sectioning plane 2* Front side of sectioning plane 3 | swZonalSectionViewZones\_swZonalSectionViewZone\_3 |
|  | 4 | * Back side of sectioning plane 1* Back side of sectioning plane 2* Front side of sectioning plane 3 | swZonalSectionViewZones\_swZonalSectionViewZone\_4 |
|  | 5 | * Front side of sectioning plane 1* Front side of sectioning plane 2* Back side of sectioning plane 3 | swZonalSectionViewZones\_swZonalSectionViewZone\_5 |
|  | 6 | * Back side of sectioning plane 1* Front side of sectioning plane 2* Back side of sectioning plane 3 | swZonalSectionViewZones\_swZonalSectionViewZone\_6 |
|  | 7 | * Front side of sectioning plane 1* Back side of sectioning plane 2* Back side of sectioning plane 3 | swZonalSectionViewZones\_swZonalSectionViewZone\_7 |
|  | 8 | * Back side of sectioning plane 1* Back side of sectioning plane 2* Back side of sectioning plane 3 | swZonalSectionViewZones\_swZonalSectionViewZone\_8 |

This property is only available if [ISectionViewData::ZonalSection](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISectionViewData~ZonalSection.html) is true.

# ![](dotnetimages/collapse.gif)See Also

####

[ISectionViewData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISectionViewData.html)

[ISectionViewData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISectionViewData_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2017 FCS, Revision Number 25.0