<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITitleBlockTableFeature~IGetTableAnnotations.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetTableAnnotations Method (ITitleBlockTableFeature) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ITitleBlockTableFeature Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITitleBlockTableFeature.html) : IGetTableAnnotations Method (ITitleBlockTableFeature) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Count*
:   Number of annotations in this title block feature

Gets all of the title block table annotations in this title block table feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetTableAnnotations( _    ByVal Count As System.Integer _ ) As TitleBlockTableAnnotation ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ITitleBlockTableFeature Dim Count As System.Integer Dim value As TitleBlockTableAnnotation   value = instance.IGetTableAnnotations(Count) ``` | |

| C# |  |
| --- | --- |
| ``` TitleBlockTableAnnotation IGetTableAnnotations(     System.int Count ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` TitleBlockTableAnnotation^ IGetTableAnnotations(  &   System.int Count ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Count*
:   Number of annotations in this title block feature

#### Return Value

* in-process, unmanaged C++: Pointer to an array of [title block table annotations](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ITitleBlockTableAnnotation.html)* VBA, VB.NET, C#, and C++/CLI: Not supported

See In-process Methods for details about this type of method.

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, call [ITitleBlockTableFeature::GetTableAnnotationCount](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ITitleBlockTableFeature~GetTableAnnotationCount.html) to get the value for Count.

# ![](dotnetimages/collapse.gif)See Also

####

[ITitleBlockTableFeature Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITitleBlockTableFeature.html)

[ITitleBlockTableFeature Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITitleBlockTableFeature_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0