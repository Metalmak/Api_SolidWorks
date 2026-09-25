<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~FeatureManagerSplitterPosition.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| FeatureManagerSplitterPosition Property (IModelDoc2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : FeatureManagerSplitterPosition Property (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Splits the FeatureManager design tree and gets or sets the location of the split bar in the FeatureManager design tree panel.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property FeatureManagerSplitterPosition As System.Double ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim value As System.Double   instance.FeatureManagerSplitterPosition = value   value = instance.FeatureManagerSplitterPosition ``` | |

| C# |  |
| --- | --- |
| ``` System.double FeatureManagerSplitterPosition {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.double FeatureManagerSplitterPosition {    System.double get();    void set ( &   System.double value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

Percentage value between 0 and 1, which sets the location of the split bar in the FeatureManager design tree panel and the size of each split FeatureManager design tree (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::FeatureManagerSplitterPosition.

# ![](dotnetimages/collapse.gif)Example

[Add ActiveX Tabs to FeatureManager Design Tree (C#)](Add_ActiveX_Tabs_to_FeatureManager_Design_Tree_Example_CSharp.htm)

[Add ActiveX Tabs to FeatureManager Design Tree (VB.NET)](Add_ActiveX_Tabs_to_FeatureManager_Design_Tree_Example_VBNET.htm)

[Add ActiveX Tabs to FeatureManager Design Tree (VBA)](Add_ActiveX_Tabs_to_FeatureManager_Design_Tree_Example_VB.htm)

[Split FeatureManager Design Tree and Position Splitter (C#)](Split_FeatureManager_Design_Tree_and_Position_Splitter_Example_CSharp.htm)

[Split FeatureManager Design Tree and Position Splitter (VB.NET)](Split_FeatureManager_Design_Tree_and_Position_Splitter_Example_VBNET.htm)

[Split FeatureManager Design Tree and Position Splitter (VBA)](Split_FeatureManager_Design_Tree_and_Position_Splitter_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

|  |  |
| --- | --- |
| **Setting this property to...** | **Results in the split panel bar..**. |
| 0 | Remaining above the FeatureManager design tree. |
| 1 | Moving below the FeatureManager design tree. |
| >0 and <1 | Setting the size of the split FeatureManager design trees within the FeatureManager design tree panel.  For example, if you specify:   * 0.5, then each FeatureManager design tree takes up 50 percent of the panel, and the split bar is located between them.* 0.8, then the bottom FeatureManager design tree takes up 80 percent of the panel, the top FeatureManager design tree takes up 20 percent of the panel, and the split bar is located between them. |

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0