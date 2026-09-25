<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimpleHoleFeatureData2~SetDirectionReference.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetDirectionReference Method (ISimpleHoleFeatureData2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISimpleHoleFeatureData2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimpleHoleFeatureData2.html) : SetDirectionReference Method (ISimpleHoleFeatureData2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Ref1*
:   First reference entity (see **Remarks**)

*Ref2*
:   Second reference entity (see **Remarks**)

Sets the direction of the cut extrude for this simple hole feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetDirectionReference( _    ByVal Ref1 As System.Object, _    ByVal Ref2 As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISimpleHoleFeatureData2 Dim Ref1 As System.Object Dim Ref2 As System.Object Dim value As System.Boolean   value = instance.SetDirectionReference(Ref1, Ref2) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetDirectionReference(     System.object Ref1,    System.object Ref2 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetDirectionReference(  &   System.Object^ Ref1, &   System.Object^ Ref2 ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Ref1*
:   First reference entity (see **Remarks**)

*Ref2*
:   Second reference entity (see **Remarks**)

#### Return Value

True if the direction for the cut is set, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SimpleHoleFeatureData2::SetDirectionReference.

# ![](dotnetimages/collapse.gif)Remarks

Sometimes one reference entity defines a direction; for example, an edge or axis. Other times, two reference entities define a direction; for example, two vertices or two sketch points.

Valid reference entities for Ref1 and Ref2:

* line segment

  * edge

    * axis

      * vertex

        * face

          * plane

            * sketch point

See Accessing Selections that Define Features for additional details.

# ![](dotnetimages/collapse.gif)See Also

####

[ISimpleHoleFeatureData2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimpleHoleFeatureData2.html)

[ISimpleHoleFeatureData2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimpleHoleFeatureData2_members.html)

[ISimpleHoleFeatureData2::GetDirectionReference Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimpleHoleFeatureData2~GetDirectionReference.html)

[ISimpleHoleFeatureData2::ReverseDirection Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimpleHoleFeatureData2~ReverseDirection.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 SP1, Revision Number 12.1