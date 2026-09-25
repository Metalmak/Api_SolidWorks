<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~CheckFeatureUse.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CheckFeatureUse Method (ISketch) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketch Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch.html) : CheckFeatureUse Method (ISketch) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FeatureType*
:   Determine if this type of feature can be created as defined in swSketchCheckFeatureProfileUsage\_e

*OpenCount*
:   Number of open contours found in this sketch

*ClosedCount*
:   Number of closed contours found in this sketch

Checks to see if this sketch is valid for use in creating a specified feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CheckFeatureUse( _    ByVal FeatureType As System.Integer, _    ByRef OpenCount As System.Integer, _    ByRef ClosedCount As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketch Dim FeatureType As System.Integer Dim OpenCount As System.Integer Dim ClosedCount As System.Integer Dim value As System.Integer   value = instance.CheckFeatureUse(FeatureType, OpenCount, ClosedCount) ``` | |

| C# |  |
| --- | --- |
| ``` System.int CheckFeatureUse(     System.int FeatureType,    out System.int OpenCount,    out System.int ClosedCount ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int CheckFeatureUse(  &   System.int FeatureType, &   [Out] System.int OpenCount, &   [Out] System.int ClosedCount ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FeatureType*
:   Determine if this type of feature can be created as defined in swSketchCheckFeatureProfileUsage\_e

*OpenCount*
:   Number of open contours found in this sketch

*ClosedCount*
:   Number of closed contours found in this sketch

#### Return Value

swSketchCheckFeatureStatus\_OK if this sketch can be used to create the specified feature; see swSketchCheckFeatureStatus\_e for possible failure values

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Sketch::CheckFeatureUse.

# ![](dotnetimages/collapse.gif)Example

[Determine If Sketch Suitable for Feature (VBA)](Determine_If_Sketch_Suitable_for_Feature_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method is equivalent to the SOLIDWORKS interactive tool Check Sketch for Feature Usage. See the SOLIDWORKS Help for details.

The OpenCount and ClosedCount arguments are output values. If this method returns swSketchCheckFeatureStatus\_OK, meaning that the sketch can be used to create the specified feature, then these two arguments contain useful information. If this method returns something else, then OpenCount and ClosedCount both return 0.

If the featureType value is not valid, this method returns  swSketchCheckFeatureStatus\_UnknownError.

# ![](dotnetimages/collapse.gif)See Also

####

[ISketch Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch.html)

[ISketch Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2000 SP03, Revision Number 8.3