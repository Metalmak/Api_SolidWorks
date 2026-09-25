<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGeneralTableFeature.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGeneralTableFeature Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGeneralTableFeature_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IGeneralTableFeature Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Allows access to the general table feature.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface IGeneralTableFeature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IGeneralTableFeature ``` | |

| C# |  |
| --- | --- |
| ``` public interface IGeneralTableFeature ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IGeneralTableFeature ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See GeneralTableFeature.

# ![](dotnetimages/collapse.gif)Example

[Hide and Show Row (VBA)](Hide_and_Show_Row_Example_VB.htm)

[Get General Table Feature (C#)](Get_General_Table_Feature_Example_CSharp.htm)

[Get General Table Feature (VB.NET)](Get_General_Table_Feature_Example_VBNET.htm)

[Get General Table Feature (VBA)](Get_General_Table_Feature_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

You can get this object using:

* [ISelectionMgr::GetSelectedObject6](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISelectionMgr~GetSelectedObject6.html) when a general table feature is selected in the FeatureManager design tree of the drawing.

  * [ITableAnnotation::GeneralTableFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ITableAnnotation~GeneralTableFeature.html).

    * [IGeneralTableAnnotation::GeneralTable](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IGeneralTableAnnotation~GeneralTable.html).

The filename extension for a general table is .sldtbt. Table templates are not supplied for general tables.

# ![](dotnetimages/collapse.gif)Accessors

See **Remarks**.

# ![](dotnetimages/collapse.gif)Access Diagram

[GeneralTableFeature](SWObjectModel.pdf#GeneralTableFeature)

# ![](dotnetimages/collapse.gif)See Also

####

[IGeneralTableFeature Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGeneralTableFeature_members.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)

[IGeneralToleranceTableFeature Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGeneralToleranceTableFeature.html)