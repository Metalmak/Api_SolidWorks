<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFlatPatternFolder~GetFlatPatterns.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetFlatPatterns Method (IFlatPatternFolder) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFlatPatternFolder Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFlatPatternFolder.html) : GetFlatPatterns Method (IFlatPatternFolder) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the flat-pattern features in this folder.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetFlatPatterns() As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFlatPatternFolder Dim value As System.Object   value = instance.GetFlatPatterns() ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetFlatPatterns() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetFlatPatterns(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

Array of [IFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html)s

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FlatPatternFolder::GetFlatPatterns.

# ![](dotnetimages/collapse.gif)Example

See [IFlatPatternFolder](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFlatPatternFolder.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[IFlatPatternFolder Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFlatPatternFolder.html)

[IFlatPatternFolder Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFlatPatternFolder_members.html)

[IFlatPatternFolder::GetFlatPatternCount Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFlatPatternFolder~GetFlatPatternCount.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2014 FCS, Revision Number 22.0