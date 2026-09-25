<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~DeleteRenderMaterial.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DeleteRenderMaterial Method (IModelDocExtension) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : DeleteRenderMaterial Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*PwMaterialId*
:   Appearance ID

*BReassignIdsAndInvalidate*
:   True if the appearance IDs are reassigned and this appearance ID is invalidated, false if not

Not supported in SOLIDWORKS 2011 and later. Superseded by [IModelDocExtension::DeleteDisplayStateSpecificRenderMaterial](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~DeleteDisplayStateSpecificRenderMaterial.html) and [IModelDocExtension::IDeleteDisplayStateSpecificRenderMaterial](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~IDeleteDisplayStateSpecificRenderMaterial.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function DeleteRenderMaterial( _    ByVal PwMaterialId As System.Integer, _    ByVal BReassignIdsAndInvalidate As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim PwMaterialId As System.Integer Dim BReassignIdsAndInvalidate As System.Boolean Dim value As System.Boolean   value = instance.DeleteRenderMaterial(PwMaterialId, BReassignIdsAndInvalidate) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool DeleteRenderMaterial(     System.int PwMaterialId,    System.bool BReassignIdsAndInvalidate ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool DeleteRenderMaterial(  &   System.int PwMaterialId, &   System.bool BReassignIdsAndInvalidate ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*PwMaterialId*
:   Appearance ID

*BReassignIdsAndInvalidate*
:   True if the appearance IDs are reassigned and this appearance ID is invalidated, false if not

#### Return Value

True if the appearance is deleted, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::DeleteRenderMaterial.

# ![](dotnetimages/collapse.gif)Remarks

By default, appearance IDs are persistent, which means if three appearances (IDs 1, 2, and 3) were applied to the model, and you removed appearance ID 2, then the remaining appearance IDs are 1 and 3. However, if you set BReassignIdsAndInvalidate to true, then appearance ID 2 is invalidated and appearance ID 3 becomes appearance ID 2.

To get the IDs of all of the appearances applied to this model document, call [IModelDocExtension::GetRenderMaterialsCount](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~GetRenderMaterialsCount.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0