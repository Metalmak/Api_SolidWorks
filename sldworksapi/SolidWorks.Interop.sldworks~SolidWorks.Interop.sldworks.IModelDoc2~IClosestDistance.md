<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~IClosestDistance.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IClosestDistance Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : IClosestDistance Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Object1*
:   Pointer to first object

*Object2*
:   Pointer to second object

*Point1*
:   Array of x, y, z coordinates for the first point

*Point2*
:   Array of x, y, z coordinates for the second point

Calculates the distance and closest points between two geometric objects.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IClosestDistance( _    ByVal Object1 As System.Object, _    ByVal Object2 As System.Object, _    ByRef Point1 As System.Double, _    ByRef Point2 As System.Double _ ) As System.Double ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim Object1 As System.Object Dim Object2 As System.Object Dim Point1 As System.Double Dim Point2 As System.Double Dim value As System.Double   value = instance.IClosestDistance(Object1, Object2, Point1, Point2) ``` | |

| C# |  |
| --- | --- |
| ``` System.double IClosestDistance(     System.object Object1,    System.object Object2,    out System.double Point1,    out System.double Point2 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.double IClosestDistance(  &   System.Object^ Object1, &   System.Object^ Object2, &   [Out] System.double Point1, &   [Out] System.double Point2 ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Object1*
:   Pointer to first object

*Object2*
:   Pointer to second object

*Point1*
:   Array of x, y, z coordinates for the first point

*Point2*
:   Array of x, y, z coordinates for the second point

#### Return Value

Minimum distance; -1.0 if no solution

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::IClosestDistance.

# ![](dotnetimages/collapse.gif)Remarks

Supported input object types include:

* swSelFACES (face)

  * swSelEDGES (edge)

    * swSelVERTICES (vertex)

      * swSelSKETCHSEGS (sketch segments)

        * swSelDATUMPLANES (reference plane)

          * swSelEXTSKETCHPOINTS (point on origin)

            * swSelDATUMAXES  (reference axis)

              * swSelCOMPONENTS (component)

                * swSelREFCURVES (reference curves)

This method includes these restrictions for drawings:

* Cannot measure between a sketch entity and a model entity

  * Measured sketch entities have to belong to the same sheet

    * Model entity measurements are based on the model origin

      * Measured object cannot be a temporary geometric entity

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0