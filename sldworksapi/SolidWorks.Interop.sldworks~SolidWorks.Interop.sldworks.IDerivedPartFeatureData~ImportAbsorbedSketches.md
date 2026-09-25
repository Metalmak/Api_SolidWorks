<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDerivedPartFeatureData~ImportAbsorbedSketches.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ImportAbsorbedSketches Property (IDerivedPartFeatureData) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDerivedPartFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDerivedPartFeatureData.html) : ImportAbsorbedSketches Property (IDerivedPartFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets whether to import absorbed sketches with the derived part feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property ImportAbsorbedSketches As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDerivedPartFeatureData Dim value As System.Boolean   instance.ImportAbsorbedSketches = value   value = instance.ImportAbsorbedSketches ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ImportAbsorbedSketches {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool ImportAbsorbedSketches {    System.bool get();    void set ( &   System.bool value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

True to its import absorbed sketches, false to not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DerivedPartFeatureData::ImportAbsorbedSketches.

# ![](dotnetimages/collapse.gif)Example

[Modify Derived Part (C#)](Modify_Derived_Part_Example_CSharp.htm)

[Modify Derived Part (VB.NET)](Modify_Derived_Part_Example_VBNET.htm)

[Modify Derived Part (VBA)](Modify_Derived_Part_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IDerivedPartFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDerivedPartFeatureData.html)

[IDerivedPartFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDerivedPartFeatureData_members.html)

[IDerivedPartFeatureData::ImportUnAbsorbedSketches Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDerivedPartFeatureData~ImportUnAbsorbedSketches.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0