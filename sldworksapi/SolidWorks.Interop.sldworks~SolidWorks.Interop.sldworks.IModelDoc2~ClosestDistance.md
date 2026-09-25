<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ClosestDistance.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ClosestDistance Method (IModelDoc2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : ClosestDistance Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Object1*
:   Pointer to first object (see **Remarks**)

*Object2*
:   Pointer to second object (see **Remarks**)

*Point1*
:   Array of x, y, z coordinates for the point on Object1 that is nearest to Point2

*Point2*
:   Array of x, y, z coordinates for the point on Object2 that is nearest to Point1

Calculates the minimum distance between the specified geometric objects.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ClosestDistance( _    ByVal Object1 As System.Object, _    ByVal Object2 As System.Object, _    ByRef Point1 As System.Object, _    ByRef Point2 As System.Object _ ) As System.Double ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim Object1 As System.Object Dim Object2 As System.Object Dim Point1 As System.Object Dim Point2 As System.Object Dim value As System.Double   value = instance.ClosestDistance(Object1, Object2, Point1, Point2) ``` | |

| C# |  |
| --- | --- |
| ``` System.double ClosestDistance(     System.object Object1,    System.object Object2,    out System.object Point1,    out System.object Point2 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.double ClosestDistance(  &   System.Object^ Object1, &   System.Object^ Object2, &   [Out] System.Object^ Point1, &   [Out] System.Object^ Point2 ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Object1*
:   Pointer to first object (see **Remarks**)

*Object2*
:   Pointer to second object (see **Remarks**)

*Point1*
:   Array of x, y, z coordinates for the point on Object1 that is nearest to Point2

*Point2*
:   Array of x, y, z coordinates for the point on Object2 that is nearest to Point1

#### Return Value

Distance in meters between Point1 and Point2; -1.0 if no solution

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::ClosestDistance.

# ![](dotnetimages/collapse.gif)Example

[Calculate Closest Distance Between Faces (VBA)](Calculate_Closest_Distance_Between_Faces_Example_VB.htm)

[Calculate Closest Distance Between Model Components (VBA)](Calculate_Closest_Distance_Between_Model_Components_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Supported types of Object1 and Object2 include swSelectType\_e:

* swSelFACES (face)

  * swSelEDGES (edge)

    * swSelVERTICES (vertex)

      * swSelSKETCHSEGS (sketch segment)

        * swSelDATUMPLANES (reference plane)

          * swSelEXTSKETCHPOINTS (point on origin)

            * swSelDATUMAXES (reference axis)

              * swSelCOMPONENTS (component; multi-body part supported, but not multi-part sub-assembly)

                * swSelREFCURVES (reference curve)

                  * swSelSOLIDBODIES (solid bodies only; surface bodies not supported)

This method has these restrictions for drawings:

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