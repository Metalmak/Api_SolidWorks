<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWGravity~ReverseDirectionAlongPlaneDir2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| ReverseDirectionAlongPlaneDir2 Property (ICWGravity) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWGravity Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWGravity.html) : ReverseDirectionAlongPlaneDir2 Property (ICWGravity) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Obsolete. Superseded by [ICWGravity::ReverseDirectionAlongPlaneDir2\_2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWGravity~ReverseDirectionAlongPlaneDir2_2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property ReverseDirectionAlongPlaneDir2 As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWGravity Dim value As System.Integer   instance.ReverseDirectionAlongPlaneDir2 = value   value = instance.ReverseDirectionAlongPlaneDir2 ``` | |

| C# |  |
| --- | --- |
| ``` System.int ReverseDirectionAlongPlaneDir2 {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int ReverseDirectionAlongPlaneDir2 {    System.int get();    void set ( &   System.int value); } ``` | |

#### Property Value

1 to reverse the direction of gravity along direction 2, 0 to not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWGravity::ReverseDirectionAlongPlaneDir2.

# ![](dotnetimages/collapse.gif)Remarks

This property is valid only if the direction reference is a face or a plane. Call [ICWGravity::SetReferenceEntity](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWGravity~SetReferenceEntity.html) to set the direction reference.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWGravity Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWGravity.html)

[ICWGravity Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWGravity_members.html)

[ICWGravity::ReverseDirectionAlongPlaneDir1 Property ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWGravity~ReverseDirectionAlongPlaneDir1.html)

[ICWGravity::ReverseDirectionNormalToPlane Property ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWGravity~ReverseDirectionNormalToPlane.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2017 SP0