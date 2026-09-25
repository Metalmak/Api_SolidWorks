<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~IGetTessPtsSize.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetTessPtsSize Method (ICurve) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICurve Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve.html) : IGetTessPtsSize Method (ICurve) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ChordTolerance*
:   Chord tolerance to be used in tessellation (meters); this is the maximum permitted
    distance from a cord to the curve between the cord endpoints

*LengthTolerance*
:   Length tolerance to be used to filter out very short segments (meters);  tessellated
    segments shorter than this value are not returned

*StartPoint*
:   Pointer to an array containing the start point of the curve

*EndPoint*
:   Pointer to an array containing the end point of the curve

Gets the size of the array required by [ICurve::IGetTessPts](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve~IGetTessPts.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetTessPtsSize( _    ByVal ChordTolerance As System.Double, _    ByVal LengthTolerance As System.Double, _    ByRef StartPoint As System.Double, _    ByRef EndPoint As System.Double _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICurve Dim ChordTolerance As System.Double Dim LengthTolerance As System.Double Dim StartPoint As System.Double Dim EndPoint As System.Double Dim value As System.Integer   value = instance.IGetTessPtsSize(ChordTolerance, LengthTolerance, StartPoint, EndPoint) ``` | |

| C# |  |
| --- | --- |
| ``` System.int IGetTessPtsSize(     System.double ChordTolerance,    System.double LengthTolerance,    ref System.double StartPoint,    ref System.double EndPoint ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int IGetTessPtsSize(  &   System.double ChordTolerance, &   System.double LengthTolerance, &   System.double% StartPoint, &   System.double% EndPoint ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ChordTolerance*
:   Chord tolerance to be used in tessellation (meters); this is the maximum permitted
    distance from a cord to the curve between the cord endpoints

*LengthTolerance*
:   Length tolerance to be used to filter out very short segments (meters);  tessellated
    segments shorter than this value are not returned

*StartPoint*
:   Pointer to an array containing the start point of the curve

*EndPoint*
:   Pointer to an array containing the end point of the curve

#### Return Value

Number of doubles returned when [ICurve::IGetTessPts](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve~IGetTessPts.html) is called

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Curve::IGetTessPtsSize.

# ![](dotnetimages/collapse.gif)Remarks

To get the actual tessellation points, use [ICurve::IGetTessPts](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurve~IGetTessPts.html). Arguments passed to ICurve::IGetTessPts must match the arguments passed to this method.

# ![](dotnetimages/collapse.gif)See Also

####

[ICurve Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve.html)

[ICurve Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve_members.html)

[ICurve::GetTessPts Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~GetTessPts.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 98Plus, datecode 1998319