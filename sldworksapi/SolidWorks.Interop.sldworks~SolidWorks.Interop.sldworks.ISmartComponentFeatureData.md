<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISmartComponentFeatureData.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ISmartComponentFeatureData Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISmartComponentFeatureData_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : ISmartComponentFeatureData Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Allows access to a Smart Component.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface ISmartComponentFeatureData ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISmartComponentFeatureData ``` | |

| C# |  |
| --- | --- |
| ``` public interface ISmartComponentFeatureData ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class ISmartComponentFeatureData ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SmartComponentFeatureData.

# ![](dotnetimages/collapse.gif)Example

[Delete Smart Feature (VBA)](Delete_Smart_Feature_Example_VB.htm)

[Delete Smart Feature (VB.NET)](Delete_Smart_Feature_Example_VBNET.htm)

[Delete Smart Feature (C#)](Delete_Smart_Feature_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

A Smart Component is defined by:

* Components* Features* Feature references

A Smart Component is created in a training assembly. When the Smart Component is saved, it is saved with the training assembly in a SOLIDWORKS part.

When the Smart Component is inserted or edited in a target assembly, the training assembly opens in a small preview window, and the PropertyManager page of the Smart Component displays.

See the SOLIDWORKS Help for more information about Smart Components.

| Use... | To... |
| --- | --- |
| This interface | - Gain access to the training assembly of a Smart Component.- Gain access to the selection lists on the PropertyManager page of a Smart Component.- Insert features and components into a Smart Component.- Delete features and components from a Smart Component. |
| [IComponent2::GetSmartComponentData](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2~GetSmartComponentData.html) | Get the current features, components, and feature references of a Smart Component. |
| [IComponent2::SetSmartComponentData](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2~SetSmartComponentData.html) | Change which features and components to enable in a Smart Component and to insert Smart Features in a target assembly. |

# ![](dotnetimages/collapse.gif)Accessors

[IFeature::GetDefinition](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~GetDefinition.html) and [IFeature::IGetDefinition](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~IGetDefinition.html)

# ![](dotnetimages/collapse.gif)Access Diagram

[SmartComponentFeatureData](SWObjectModel.pdf#SmartComponentFeatureData)

# ![](dotnetimages/collapse.gif)See Also

####

[ISmartComponentFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISmartComponentFeatureData_members.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)

[IComponent2::IsSmartComponent Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IsSmartComponent.html)