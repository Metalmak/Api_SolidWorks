<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurfaceTrimFeatureData~IGetPiecesToKeep.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetPiecesToKeep Method (ISurfaceTrimFeatureData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISurfaceTrimFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurfaceTrimFeatureData.html) : IGetPiecesToKeep Method (ISurfaceTrimFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Count*
:   Number of pieces to keep

Gets the pieces to keep for this surface trim feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetPiecesToKeep( _    ByVal Count As System.Integer _ ) As Body2 ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISurfaceTrimFeatureData Dim Count As System.Integer Dim value As Body2   value = instance.IGetPiecesToKeep(Count) ``` | |

| C# |  |
| --- | --- |
| ``` Body2 IGetPiecesToKeep(     System.int Count ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Body2^ IGetPiecesToKeep(  &   System.int Count ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Count*
:   Number of pieces to keep

#### Return Value

* in-process, unmanaged C++: Pointer to an array of pieces to keep of size Count

- VBA, VB.NET, C#, and C++/CLI: Not supported

  See In-process Methods for details about this type of method.

# ![](dotnetimages/collapse.gif)Remarks

Call [ISurfaceTrimFeatureData::GetPiecesToKeepCount](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISurfaceTrimFeatureData~GetPiecesToKeepCount.html) before calling this method to get the value for Count.

See Accessing Selections that Define Features for additional details.

# ![](dotnetimages/collapse.gif)See Also

####

[ISurfaceTrimFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurfaceTrimFeatureData.html)

[ISurfaceTrimFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurfaceTrimFeatureData_members.html)

[ISurfaceTrimFeatureData::ISetPiecesToKeep Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurfaceTrimFeatureData~ISetPiecesToKeep.html)

[ISurfaceTrimFeatureData::PiecesToKeep Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurfaceTrimFeatureData~PiecesToKeep.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus SP2, Revision Number 10.2