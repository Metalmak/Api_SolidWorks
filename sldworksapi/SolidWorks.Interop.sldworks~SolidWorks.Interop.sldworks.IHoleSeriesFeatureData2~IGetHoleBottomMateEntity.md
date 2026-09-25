<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleSeriesFeatureData2~IGetHoleBottomMateEntity.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetHoleBottomMateEntity Method (IHoleSeriesFeatureData2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IHoleSeriesFeatureData2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleSeriesFeatureData2.html) : IGetHoleBottomMateEntity Method (IHoleSeriesFeatureData2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*HoleInstance*
:   Index number of the hole whose entity you want

*HoleType*
:   Type of hole as defined by swWzdHoleTypes\_e

Gets the entity to which the bottom of the hole is mated in this hole series.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetHoleBottomMateEntity( _    ByVal HoleInstance As System.Integer, _    ByVal HoleType As System.Short _ ) As Entity ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IHoleSeriesFeatureData2 Dim HoleInstance As System.Integer Dim HoleType As System.Short Dim value As Entity   value = instance.IGetHoleBottomMateEntity(HoleInstance, HoleType) ``` | |

| C# |  |
| --- | --- |
| ``` Entity IGetHoleBottomMateEntity(     System.int HoleInstance,    System.short HoleType ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Entity^ IGetHoleBottomMateEntity(  &   System.int HoleInstance, &   System.short HoleType ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*HoleInstance*
:   Index number of the hole whose entity you want

*HoleType*
:   Type of hole as defined by swWzdHoleTypes\_e

#### Return Value

[Entity](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEntity.html) to which the bottom of the hole is mated

# ![](dotnetimages/collapse.gif)See Also

####

[IHoleSeriesFeatureData2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleSeriesFeatureData2.html)

[IHoleSeriesFeatureData2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleSeriesFeatureData2_members.html)

[IHoleSeriesFeatureData2::GetHoleBottomMateEntity Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleSeriesFeatureData2~GetHoleBottomMateEntity.html)

[IHoleSeriesFeatureData2::GetHoleTopMateEntity Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleSeriesFeatureData2~GetHoleTopMateEntity.html)

[IHoleSeriesFeatureData2::IGetHoleTopMateEntity Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleSeriesFeatureData2~IGetHoleTopMateEntity.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2014 FCS, Revision Number 22.0