<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~SetSmartComponentData.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetSmartComponentData Method (IComponent2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IComponent2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2.html) : SetSmartComponentData Method (IComponent2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FeaturesSelected*
:   Array of boolean values indicating which features to enable in the Smart Component (see **Remarks**)

*ComponentsSelected*
:   Array of boolean values indicating which components to enable in the Smart Component (see **Remarks**)

*References*
:   Array of feature reference entities in the target assembly that are used to activate the features specified by FeaturesSelected (see **Remarks**)

Sets the features, components, and feature references of a Smart Component.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetSmartComponentData( _    ByVal FeaturesSelected As System.Object, _    ByVal ComponentsSelected As System.Object, _    ByVal References As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IComponent2 Dim FeaturesSelected As System.Object Dim ComponentsSelected As System.Object Dim References As System.Object Dim value As System.Boolean   value = instance.SetSmartComponentData(FeaturesSelected, ComponentsSelected, References) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetSmartComponentData(     System.object FeaturesSelected,    System.object ComponentsSelected,    System.object References ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetSmartComponentData(  &   System.Object^ FeaturesSelected, &   System.Object^ ComponentsSelected, &   System.Object^ References ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FeaturesSelected*
:   Array of boolean values indicating which features to enable in the Smart Component (see **Remarks**)

*ComponentsSelected*
:   Array of boolean values indicating which components to enable in the Smart Component (see **Remarks**)

*References*
:   Array of feature reference entities in the target assembly that are used to activate the features specified by FeaturesSelected (see **Remarks**)

#### Return Value

True if successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Component2::SetSmartComponentData.

# ![](dotnetimages/collapse.gif)Example

[Activate Smart Features in an Assembly (VBA)](Activate_Smart_Features_in_an_Assembly_Example_VB.htm)

[Activate Smart Features in an Assembly (VB.NET)](Activate_Smart_Features_in_an_Assembly_Example_VBNET.htm)

[Activate Smart Features in an Assembly (C#)](Activate_Smart_Features_in_an_Assembly_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

A Smart Component is defined by its:

* Components* Features* Feature references

See the SOLIDWORKS Help for more information about Smart Components.

Use this method to:

* Change which features and components to enable in a Smart Component.* Activate the Smart Features.

Before calling this method:

1. Open an assembly that contains a Smart Component whose Smart Features have not yet been activated.- Find the Smart Component in the assembly using [IComponent2::IsSmartComponent](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2~IsSmartComponent.html).- Call [IComponent2::GetSmartComponentData](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2~GetSmartComponentData.html) to obtain the current feature and component arrays for the Smart Component.- Create two boolean arrays whose elements map one-to-one with the elements in the feature and component arrays.- For each element in each boolean array, specify true if the corresponding feature or component is enabled in the Smart Component. Specify false if it is not.- Set FeaturesSelected and ComponentsSelected with the corresponding boolean arrays.- Create an array of reference entities (e.g., faces, edges, points) selected from the target assembly that map to the feature reference entities that were defined for the Smart Component.- Set References to the array of reference entities.

Use [ISmartComponentFeatureData](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISmartComponentFeatureData.html) to:

* Insert new features and components into a Smart Component.* Delete features and components from a Smart Component.

# ![](dotnetimages/collapse.gif)See Also

####

[IComponent2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2.html)

[IComponent2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2_members.html)

[IAssemblyDoc::AddSmartComponent Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~AddSmartComponent.html)

[IAssemblyDoc::CreateSmartComponent Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~CreateSmartComponent.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2012 FCS, Revision Number 20.0