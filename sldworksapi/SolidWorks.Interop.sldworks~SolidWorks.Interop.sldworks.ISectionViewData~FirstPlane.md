<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISectionViewData~FirstPlane.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| FirstPlane Property (ISectionViewData) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISectionViewData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISectionViewData.html) : FirstPlane Property (ISectionViewData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the section plane for the first section of the section view for the part or assembly.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property FirstPlane As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISectionViewData Dim value As System.Object   instance.FirstPlane = value   value = instance.FirstPlane ``` | |

| C# |  |
| --- | --- |
| ``` System.object FirstPlane {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.Object^ FirstPlane {    System.Object^ get();    void set ( &   System.Object^ value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

[Plane](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html) or [planar face](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SectionViewData::FirstPlane.

# ![](dotnetimages/collapse.gif)Example

[Create Section View in Model (C#)](Create_Section_View_in_Model_Example_CSharp.htm)

[Create Section View in Model (VB.NET)](Create_Section_View_in_Model_Example_VBNET.htm)

[Create Section View in Model (VBA)](Create_Section_View_in_Model_Example_VB.htm)

[Get Section View Data (C#)](Get_Section_View_Data_Example_CSharp.htm)

[Get Section View Data (VB.NET)](Get_Section_View_Data_Example_VBNET.htm)

[Get Section View Data (VBA)](Get_Section_View_Data_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

To select the section plane for the first section, specify 1 for Mark for [IModelDocExtension::SelectByID2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~SelectByID2.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ISectionViewData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISectionViewData.html)

[ISectionViewData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISectionViewData_members.html)

[ISectionViewData::GetFirstPlaneParameters Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISectionViewData~GetFirstPlaneParameters.html)

[ISectionViewData::GetSecondPlaneParameters Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISectionViewData~GetSecondPlaneParameters.html)

[ISectionViewData::GetThirdPlaneParameters Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISectionViewData~GetThirdPlaneParameters.html)

[ISectionViewData::SecondPlane Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISectionViewData~SecondPlane.html)

[ISectionViewData::ThirdPlane Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISectionViewData~ThirdPlane.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0