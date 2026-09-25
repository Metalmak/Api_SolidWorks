<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartingLineFeatureData~IGetEntitiesToSplit.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetEntitiesToSplit Method (IPartingLineFeatureData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPartingLineFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartingLineFeatureData.html) : IGetEntitiesToSplit Method (IPartingLineFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Count*
:   Number of entities

*TypeArr*
:   * in-process, unmanaged C++: Pointer to an array of these entities as defined in swSelectType\_e:

      + swSelVERTICES

        + swSelSKETCHSEGS* VBA, VB.NET, C#, and C++/CLI: Not supported

    See In-process Methods for details about this type of method.

Gets the entities that are used to split a face.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetEntitiesToSplit( _    ByVal Count As System.Integer, _    ByRef TypeArr As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPartingLineFeatureData Dim Count As System.Integer Dim TypeArr As System.Integer Dim value As System.Object   value = instance.IGetEntitiesToSplit(Count, TypeArr) ``` | |

| C# |  |
| --- | --- |
| ``` System.object IGetEntitiesToSplit(     System.int Count,    out System.int TypeArr ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ IGetEntitiesToSplit(  &   System.int Count, &   [Out] System.int TypeArr ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Count*
:   Number of entities

*TypeArr*
:   * in-process, unmanaged C++: Pointer to an array of these entities as defined in swSelectType\_e:

      + swSelVERTICES

        + swSelSKETCHSEGS* VBA, VB.NET, C#, and C++/CLI: Not supported

    See In-process Methods for details about this type of method.

#### Return Value

* in-process, unmanaged C++: Pointer to an array of [vertices](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IVertex.html) or [sketch segments](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchSegment.html)

- VBA, VB.NET, C#, and C++/CLI: Not supported

# ![](dotnetimages/collapse.gif)Remarks

The resulting edges are added to the parting line feature.

Call [IPartingLineFeatureData::GetEntitiesToSplitCount](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPartingLineFeatureData~GetEntitiesToSplitCount.html) before this method.

When two vertices are specified, then an edge is created between them for the parting line feature.

See Accessing Selections that Define Features for additional details on using this method.

# ![](dotnetimages/collapse.gif)See Also

####

[IPartingLineFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartingLineFeatureData.html)

[IPartingLineFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartingLineFeatureData_members.html)

[IPartingLineFeatureData::GetEntitiesToSplit Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartingLineFeatureData~GetEntitiesToSplit.html)

[IPartingLineFeatureData::ISetEntitiesToSplit Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartingLineFeatureData~ISetEntitiesToSplit.html)

[IPartingLineFeatureData::SetEntitiesToSplit Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartingLineFeatureData~SetEntitiesToSplit.html)

[IPartingLineFeatureData::SplitFaces Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartingLineFeatureData~SplitFaces.html)

[IPartingLineFeatureData::SplitFacesOption Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartingLineFeatureData~SplitFacesOption.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2005 FCS, Revision Number 13.0