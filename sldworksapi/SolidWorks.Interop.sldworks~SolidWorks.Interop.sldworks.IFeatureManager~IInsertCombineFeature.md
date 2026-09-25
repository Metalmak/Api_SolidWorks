<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~IInsertCombineFeature.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IInsertCombineFeature Method (IFeatureManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : IInsertCombineFeature Method (IFeatureManager) |

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

*ToolsCount*
:   Number of bodies to combine

*ToolsArr*
:   * in-process, unmanaged C++: Pointer to an array of [bodies](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html) to combine of size ToolsCount (see **Remarks**)* VBA, VB.NET, C#, and C++/CLI: Not supported

    See In-process Methods for details about this type of method.

Combines the specified bodies in the multibody part to create a combine feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IInsertCombineFeature( _    ByVal OperationType As System.Integer, _    ByVal MainBody As Body2, _    ByVal ToolsCount As System.Integer, _    ByRef ToolsArr As Body2 _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim OperationType As System.Integer Dim MainBody As Body2 Dim ToolsCount As System.Integer Dim ToolsArr As Body2 Dim value As Feature   value = instance.IInsertCombineFeature(OperationType, MainBody, ToolsCount, ToolsArr) ``` | |

| C# |  |
| --- | --- |
| ``` Feature IInsertCombineFeature(     System.int OperationType,    Body2 MainBody,    System.int ToolsCount,    ref Body2 ToolsArr ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ IInsertCombineFeature(  &   System.int OperationType, &   Body2^ MainBody, &   System.int ToolsCount, &   Body2^% ToolsArr ) ``` | |

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

*ToolsCount*
:   Number of bodies to combine

*ToolsArr*
:   * in-process, unmanaged C++: Pointer to an array of [bodies](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html) to combine of size ToolsCount (see **Remarks**)* VBA, VB.NET, C#, and C++/CLI: Not supported

    See In-process Methods for details about this type of method.

#### Return Value

[IFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html)

# ![](dotnetimages/collapse.gif)Remarks

You can either call this method, directly passing in the bodies with MainBody and ToolVar, or you can:

1. Select the bodies using [IModelDocExtension::SelectByID2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SelectByID2.html) as follows:

   | To select... | Use Mark... |
   | --- | --- |
   | MainBody | 1 |
   | ToolVar bodies | 2 |

   - Call this method, setting MainBody to Nothing or null and ToolVar to an empty array.

See the SOLIDWORKS Help for more information about the combined feature.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IFeatureManager::InsertCombineFeature Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertCombineFeature.html)

[ICombineBodiesFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICombineBodiesFeatureData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2003 FCS, Revision Number 11.0