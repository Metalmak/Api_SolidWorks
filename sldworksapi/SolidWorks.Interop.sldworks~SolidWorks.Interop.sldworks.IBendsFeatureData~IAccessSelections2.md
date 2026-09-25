<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBendsFeatureData~IAccessSelections2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IAccessSelections2 Method (IBendsFeatureData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBendsFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBendsFeatureData.html) : IAccessSelections2 Method (IBendsFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*TopDoc*
:   Top-level document

*Component*
:   Allows you to gain access to the selections that describe this Flatten-Bends/Process-Bends feature

Allows access to the selections that describe this Flatten-Bends/Process-Bends feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IAccessSelections2( _    ByVal TopDoc As ModelDoc2, _    ByVal Component As Component2 _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBendsFeatureData Dim TopDoc As ModelDoc2 Dim Component As Component2 Dim value As System.Boolean   value = instance.IAccessSelections2(TopDoc, Component) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool IAccessSelections2(     ModelDoc2 TopDoc,    Component2 Component ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool IAccessSelections2(  &   ModelDoc2^ TopDoc, &   Component2^ Component ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*TopDoc*
:   Top-level document

*Component*
:   Allows you to gain access to the selections that describe this Flatten-Bends/Process-Bends feature

#### Return Value

True if the selections were successfully accessed, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See BendsFeatureData::IAccessSelections2.

# ![](dotnetimages/collapse.gif)Remarks

|  |  |
| --- | --- |
| **To modify a feature in a...** | **Then...** |
| Part | * TopDoc argument is the [IModelDoc2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2.html) for the part * Component argument is NULL |
| Assembly | * TopDoc argument is the ModelDoc2 object for the assembly * Component argument is the [IComponent2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2.html) object in which the feature is to be modified |

This method puts the model into a rollback state to allow access to the selections that define this feature. You must use either of the following methods to restore the rollback state:

* [IFeature::IModifyDefinition2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~IModifyDefinition2.html) if you modified the feature

  * [IBendsFeatureData::ReleaseSelectionAccess](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBendsFeatureData~ReleaseSelectionAccess.html) if you did not

# ![](dotnetimages/collapse.gif)See Also

####

[IBendsFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBendsFeatureData.html)

[IBendsFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBendsFeatureData_members.html)

[IBendsFeatureData::AccessSelections Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBendsFeatureData~AccessSelections.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0