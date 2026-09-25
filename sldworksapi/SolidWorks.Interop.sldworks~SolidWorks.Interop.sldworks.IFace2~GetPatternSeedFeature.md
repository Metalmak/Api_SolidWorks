<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2~GetPatternSeedFeature.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetPatternSeedFeature Method (IFace2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFace2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2.html) : GetPatternSeedFeature Method (IFace2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the seed feature of a pattern.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetPatternSeedFeature() As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFace2 Dim value As System.Object   value = instance.GetPatternSeedFeature() ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetPatternSeedFeature() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetPatternSeedFeature(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

Seed feature of the current face; if the face does not belong to a pattern, this method returns NULL

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Face2::GetPatternSeedFeature.

# ![](dotnetimages/collapse.gif)See Also

####

[IFace2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2.html)

[IFace2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2_members.html)

[IFace2::IGetPatternSeedFeature Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2~IGetPatternSeedFeature.html)

[IModelDoc2::EditSeedFeat Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~EditSeedFeat.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0