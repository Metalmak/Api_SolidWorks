<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertCombineFeature.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertCombineFeature Method (IFeatureManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertCombineFeature Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*OperationType*
:   Operation as defined in swBodyOperationType\_e

*MainBody*
:   | If OperationType is ... | Then set MainBody to ... |
    | --- | --- |
    | swBodyOperationType\_e.SWBODYADD | Nothing or null |
    | swBodyOperationType\_e.SWBODYCUT | Target [body](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html) |
    | swBodyOperationType\_e.SWBODYINTERSECT | Nothing or null |

    (See **Remarks**)

*ToolVar*
:   Array of [bodies](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html) to combine (see **Remarks**)

Combines the specified bodies in the multibody part to create a combine feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertCombineFeature( _    ByVal OperationType As System.Integer, _    ByVal MainBody As Body2, _    ByVal ToolVar As System.Object _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim OperationType As System.Integer Dim MainBody As Body2 Dim ToolVar As System.Object Dim value As Feature   value = instance.InsertCombineFeature(OperationType, MainBody, ToolVar) ``` | |

| C# |  |
| --- | --- |
| ``` Feature InsertCombineFeature(     System.int OperationType,    Body2 MainBody,    System.object ToolVar ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ InsertCombineFeature(  &   System.int OperationType, &   Body2^ MainBody, &   System.Object^ ToolVar ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*OperationType*
:   Operation as defined in swBodyOperationType\_e

*MainBody*
:   | If OperationType is ... | Then set MainBody to ... |
    | --- | --- |
    | swBodyOperationType\_e.SWBODYADD | Nothing or null |
    | swBodyOperationType\_e.SWBODYCUT | Target [body](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html) |
    | swBodyOperationType\_e.SWBODYINTERSECT | Nothing or null |

    (See **Remarks**)

*ToolVar*
:   Array of [bodies](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html) to combine (see **Remarks**)

#### Return Value

[IFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertCombineFeature.

# ![](dotnetimages/collapse.gif)Example

[Combine Bodies (C#)](Combine_Bodies_Example_CSharp.htm)

[Combine Bodies (VB.NET)](Combine_Bodies_Example_VBNET.htm)

[Combine Bodies (VBA)](Combine_Bodies_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

You can either call this method, directly passing in the bodies with MainBody and ToolVar, or you can:

1. Select the bodies using [IModelDocExtension::SelectByID2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SelectByID2.html) as follows:

   | To select... | Use Mark... |
   | --- | --- |
   | MainBody | 1 |
   | ToolVar bodies | 2 |

   - Call this method, setting MainBody to Nothing or null and ToolVar to an empty array.

See the SOLIDWORKS Help for more information about the combine feature.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IFeatureManager::IInsertCombineFeature Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~IInsertCombineFeature.html)

[ICombineBodiesFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICombineBodiesFeatureData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2003 FCS, Revision Number 11.0