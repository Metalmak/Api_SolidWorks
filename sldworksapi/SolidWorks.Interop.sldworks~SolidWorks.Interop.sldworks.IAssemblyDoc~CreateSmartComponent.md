<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~CreateSmartComponent.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateSmartComponent Method (IAssemblyDoc) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html) : CreateSmartComponent Method (IAssemblyDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ComponentIn*
:   [IComponent2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2.html) to make smart

*RelatedComponents*
:   Array of the components to associate with the Smart Component

*RelatedFeatures*
:   Array of the [features](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html) contained in the components to associate with the Smart Component

*AutoSizeDiameter*
:   True to auto-size a cylindrical Smart Component that has multiple configurations, false to not

*LpMateReference*
:   Concentric mate reference between a cylindrical face or axis and a feature

*BoundingValues*
:   Array of doubles specifying minimum and maximum diameter values with which each configuration is compatible

Creates a Smart Component.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateSmartComponent( _    ByVal ComponentIn As Component2, _    ByVal RelatedComponents As System.Object, _    ByVal RelatedFeatures As System.Object, _    ByVal AutoSizeDiameter As System.Boolean, _    ByVal LpMateReference As Entity, _    ByVal BoundingValues As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAssemblyDoc Dim ComponentIn As Component2 Dim RelatedComponents As System.Object Dim RelatedFeatures As System.Object Dim AutoSizeDiameter As System.Boolean Dim LpMateReference As Entity Dim BoundingValues As System.Object Dim value As System.Boolean   value = instance.CreateSmartComponent(ComponentIn, RelatedComponents, RelatedFeatures, AutoSizeDiameter, LpMateReference, BoundingValues) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool CreateSmartComponent(     Component2 ComponentIn,    System.object RelatedComponents,    System.object RelatedFeatures,    System.bool AutoSizeDiameter,    Entity LpMateReference,    System.object BoundingValues ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool CreateSmartComponent(  &   Component2^ ComponentIn, &   System.Object^ RelatedComponents, &   System.Object^ RelatedFeatures, &   System.bool AutoSizeDiameter, &   Entity^ LpMateReference, &   System.Object^ BoundingValues ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ComponentIn*
:   [IComponent2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2.html) to make smart

*RelatedComponents*
:   Array of the components to associate with the Smart Component

*RelatedFeatures*
:   Array of the [features](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html) contained in the components to associate with the Smart Component

*AutoSizeDiameter*
:   True to auto-size a cylindrical Smart Component that has multiple configurations, false to not

*LpMateReference*
:   Concentric mate reference between a cylindrical face or axis and a feature

*BoundingValues*
:   Array of doubles specifying minimum and maximum diameter values with which each configuration is compatible

#### Return Value

True if the Smart Component is created, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AssemblyDoc::CreateSmartComponent.

# ![](dotnetimages/collapse.gif)Example

[Make Smart Component (VBA)](Make_Smart_Component_Example_VB.htm)

[Make Smart Component With Mate (VBA)](Make_Smart_Component_with__Mate_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

For example, a component with these configurations:

* TenInchDiameter

  * ThirteenInchDiameter

    * TwentyInchDiameter

might have a BoundingValues array of [9,11,12,14,19,21], which specifies a +1 tolerance over each configuration parameter.

# ![](dotnetimages/collapse.gif)See Also

####

[IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html)

[IAssemblyDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc_members.html)

[IAssemblyDoc::AddSmartComponent Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~AddSmartComponent.html)

[IComponent2::GetSmartComponentData Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetSmartComponentData.html)

[IComponent2::IsSmartComponent Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IsSmartComponent.html)

[IComponent2::SetSmartComponentData Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~SetSmartComponentData.html)

[ISmartComponentFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISmartComponentFeatureData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15