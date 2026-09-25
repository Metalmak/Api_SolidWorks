<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExtrudeFeatureData2~GetDirectionReference.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetDirectionReference Method (IExtrudeFeatureData2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IExtrudeFeatureData2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExtrudeFeatureData2.html) : GetDirectionReference Method (IExtrudeFeatureData2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Ref1*
:   First reference entity

*Type1*
:   Type of reference entity as defined by swSelectType\_e (see **Remarks**)

*Ref2*
:   Second reference entity

*Type2*
:   Type of reference entity as defined by swSelectType\_e

Gets the direction of the extrusion.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetDirectionReference( _    ByRef Ref1 As System.Object, _    ByRef Type1 As System.Integer, _    ByRef Ref2 As System.Object, _    ByRef Type2 As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IExtrudeFeatureData2 Dim Ref1 As System.Object Dim Type1 As System.Integer Dim Ref2 As System.Object Dim Type2 As System.Integer Dim value As System.Integer   value = instance.GetDirectionReference(Ref1, Type1, Ref2, Type2) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetDirectionReference(     out System.object Ref1,    out System.int Type1,    out System.object Ref2,    out System.int Type2 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetDirectionReference(  &   [Out] System.Object^ Ref1, &   [Out] System.int Type1, &   [Out] System.Object^ Ref2, &   [Out] System.int Type2 ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Ref1*
:   First reference entity

*Type1*
:   Type of reference entity as defined by swSelectType\_e (see **Remarks**)

*Ref2*
:   Second reference entity

*Type2*
:   Type of reference entity as defined by swSelectType\_e

#### Return Value

Number of reference entities used to define the direction of the extrusion

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ExtrudeFeatureData2::GetDirectionReference.

# ![](dotnetimages/collapse.gif)Remarks

Sometimes one reference entity defines a direction; for example, an edge or axis. Other times, two reference entities define a direction; for example, two vertices or two sketch points.

|  |  |
| --- | --- |
| **If...** | **Then...** |
| One reference entity defined the direction | Ref2 is NULL and the return value is 1 |
| Two reference entities defined the direction | Both Ref1 and Ref2 are non-NULL and the return value is 2 |

Valid reference entities for Type1 and Type2:

* line segment

  * edge

    * axis

      * vertex

        * face

          * plane

            * sketch point

# ![](dotnetimages/collapse.gif)See Also

####

[IExtrudeFeatureData2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExtrudeFeatureData2.html)

[IExtrudeFeatureData2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExtrudeFeatureData2_members.html)

[IExtrudeFeatureData2::SetDirectionReference Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExtrudeFeatureData2~SetDirectionReference.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12.0