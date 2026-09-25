<!-- source: swdocmgrapi/SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument28~SetSplitFeatureReferences.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Document Manager API Help | Send comments on this topic. |
| SetSplitFeatureReferences Method (ISwDMDocument28) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdocumentmgr Namespace](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr_namespace.html) > [ISwDMDocument28 Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument28.html) : SetSplitFeatureReferences Method (ISwDMDocument28) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ListOfSplitPartPaths*
:   Array of paths of split parts

*ListOfModifiedSplitPartPaths*
:   Array of renamed paths of split parts

*NewPathName*
:   New path name

Sets the specified split parts in this document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetSplitFeatureReferences( _    ByVal ListOfSplitPartPaths As System.Object, _    ByVal ListOfModifiedSplitPartPaths As System.Object, _    ByVal NewPathName As System.String _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwDMDocument28 Dim ListOfSplitPartPaths As System.Object Dim ListOfModifiedSplitPartPaths As System.Object Dim NewPathName As System.String   instance.SetSplitFeatureReferences(ListOfSplitPartPaths, ListOfModifiedSplitPartPaths, NewPathName) ``` | |

| C# |  |
| --- | --- |
| ``` void SetSplitFeatureReferences(     System.object ListOfSplitPartPaths,    System.object ListOfModifiedSplitPartPaths,    System.string NewPathName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetSplitFeatureReferences(  &   System.Object^ ListOfSplitPartPaths, &   System.Object^ ListOfModifiedSplitPartPaths, &   System.String^ NewPathName ) ``` | |

#### Parameters

*ListOfSplitPartPaths*
:   Array of paths of split parts

*ListOfModifiedSplitPartPaths*
:   Array of renamed paths of split parts

*NewPathName*
:   New path name

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwDMDocument28::SetSplitFeatureReferences.

# ![](dotnetimages/collapse.gif)Remarks

SOLIDWORKS 2022 allows you to Pack and Go parts created by the Save Bodies and Split features. The split
parts created are listed as references of the parent part.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwDMDocument28 Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument28.html)

[ISwDMDocument28 Members](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument28_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Document Manager API 2022 SP0