<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkageRod~SetSectionParams.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetSectionParams Method (ICWLinkageRod) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWLinkageRod Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkageRod.html) : SetSectionParams Method (ICWLinkageRod) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NSectionType*
:   Cross-section parameter type as defined by [swsCRSectionType\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsCRSectionType_e.html)

*ArrayParamValues*
:   Array of parameter values (see **Remarks**)

Sets the specified cross-section parameter values.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetSectionParams( _    ByVal NSectionType As System.Integer, _    ByVal ArrayParamValues As System.Object _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWLinkageRod Dim NSectionType As System.Integer Dim ArrayParamValues As System.Object   instance.SetSectionParams(NSectionType, ArrayParamValues) ``` | |

| C# |  |
| --- | --- |
| ``` void SetSectionParams(     System.int NSectionType,    System.object ArrayParamValues ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetSectionParams(  &   System.int NSectionType, &   System.Object^ ArrayParamValues ) ``` | |

#### Parameters

*NSectionType*
:   Cross-section parameter type as defined by [swsCRSectionType\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsCRSectionType_e.html)

*ArrayParamValues*
:   Array of parameter values (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWLinkageRod::SetSectionParams.

# ![](dotnetimages/collapse.gif)Example

See the [ICWLinkageRod](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkageRod.html) examples

# ![](dotnetimages/collapse.gif)Remarks

If NSectionType is swsCRSectionType\_e.:

* swsSolidCircular, then specify ArrayParamValues with an array containing outer radius.* swsSolidRectangular, then specify ArrayParamValues with an array containing width and height.* swsHollowCircular, then specify ArrayParamValues with an array containing outer radius and wall thickness.* swsHollowRectangular, then specify ArrayParamValues with an array containing width, height, and wall thickness.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWLinkageRod Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkageRod.html)

[ICWLinkageRod Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkageRod_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2022 SP0