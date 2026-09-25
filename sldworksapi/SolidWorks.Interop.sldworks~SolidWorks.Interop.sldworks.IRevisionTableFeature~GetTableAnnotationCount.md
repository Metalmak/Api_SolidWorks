<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRevisionTableFeature~GetTableAnnotationCount.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetTableAnnotationCount Method (IRevisionTableFeature) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IRevisionTableFeature Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRevisionTableFeature.html) : GetTableAnnotationCount Method (IRevisionTableFeature) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the number of revision table annotations for this revision table.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetTableAnnotationCount() As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IRevisionTableFeature Dim value As System.Integer   value = instance.GetTableAnnotationCount() ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetTableAnnotationCount() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetTableAnnotationCount(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

Number of revision table annotations

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See RevisionTableFeature::GetTableAnnotationCount.

# ![](dotnetimages/collapse.gif)Example

See the [IRevisionTableFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRevisionTableFeature.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

Call this method before calling [IRevisionTableFeature::IGetTableAnnotations](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IRevisionTableFeature~IGetTableAnnotations.html) to get the size of the array for that method.

# ![](dotnetimages/collapse.gif)See Also

####

[IRevisionTableFeature Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRevisionTableFeature.html)

[IRevisionTableFeature Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRevisionTableFeature_members.html)

[IRevisionTableFeature::GetTableAnnotations Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRevisionTableFeature~GetTableAnnotations.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12.0