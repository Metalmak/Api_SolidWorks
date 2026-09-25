<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICoreFeatureData~DraftAngle.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DraftAngle Property (ICoreFeatureData) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICoreFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICoreFeatureData.html) : DraftAngle Property (ICoreFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the angle of the draft for this core feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property DraftAngle As System.Double ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICoreFeatureData Dim value As System.Double   instance.DraftAngle = value   value = instance.DraftAngle ``` | |

| C# |  |
| --- | --- |
| ``` System.double DraftAngle {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.double DraftAngle {    System.double get();    void set ( &   System.double value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

Angle of draft

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CoreFeatureData::DraftAngle.

# ![](dotnetimages/collapse.gif)Example

[Get Core Feature Data (C#)](Get_Core_Feature_Example_CSharp.htm)

[Get Core Feature Data (VB.NET)](Get_Core_Feature_Example_VBNET.htm)

[Get Core Feature Data (VBA)](Get_Core_Feature_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

To set this property, [ICoreFeatureData::UseDraft](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICoreFeatureData~UseDraft.html) must be true.

# ![](dotnetimages/collapse.gif)See Also

####

[ICoreFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICoreFeatureData.html)

[ICoreFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICoreFeatureData_members.html)

[ICoreFeatureData::DraftOutward Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICoreFeatureData~DraftOutward.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 FCS, Revision Number 14.0