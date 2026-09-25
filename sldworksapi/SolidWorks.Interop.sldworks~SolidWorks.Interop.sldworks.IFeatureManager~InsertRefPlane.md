<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertRefPlane.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertRefPlane Method (IFeatureManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertRefPlane Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FirstConstraint*
:   First constraint as defined in swRefPlaneReferenceConstraints\_e

*FirstConstraintAngleOrDistance*
:   Angle or distance of the first constraint

*SecondConstraint*
:   Second constraint as defined in swRefPlaneReferenceConstraints\_e

*SecondConstraintAngleOrDistance*
:   Angle or distance of the second constraint

*ThirdConstraint*
:   Third constraint as defined in swRefPlaneReferenceConstraints\_e

*ThirdConstraintAngleOrDistance*
:   Angle or distance of the third constraint

Inserts a constraint-based reference plane using the selected reference entities.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertRefPlane( _    ByVal FirstConstraint As System.Integer, _    ByVal FirstConstraintAngleOrDistance As System.Double, _    ByVal SecondConstraint As System.Integer, _    ByVal SecondConstraintAngleOrDistance As System.Double, _    ByVal ThirdConstraint As System.Integer, _    ByVal ThirdConstraintAngleOrDistance As System.Double _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim FirstConstraint As System.Integer Dim FirstConstraintAngleOrDistance As System.Double Dim SecondConstraint As System.Integer Dim SecondConstraintAngleOrDistance As System.Double Dim ThirdConstraint As System.Integer Dim ThirdConstraintAngleOrDistance As System.Double Dim value As System.Object   value = instance.InsertRefPlane(FirstConstraint, FirstConstraintAngleOrDistance, SecondConstraint, SecondConstraintAngleOrDistance, ThirdConstraint, ThirdConstraintAngleOrDistance) ``` | |

| C# |  |
| --- | --- |
| ``` System.object InsertRefPlane(     System.int FirstConstraint,    System.double FirstConstraintAngleOrDistance,    System.int SecondConstraint,    System.double SecondConstraintAngleOrDistance,    System.int ThirdConstraint,    System.double ThirdConstraintAngleOrDistance ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ InsertRefPlane(  &   System.int FirstConstraint, &   System.double FirstConstraintAngleOrDistance, &   System.int SecondConstraint, &   System.double SecondConstraintAngleOrDistance, &   System.int ThirdConstraint, &   System.double ThirdConstraintAngleOrDistance ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FirstConstraint*
:   First constraint as defined in swRefPlaneReferenceConstraints\_e

*FirstConstraintAngleOrDistance*
:   Angle or distance of the first constraint

*SecondConstraint*
:   Second constraint as defined in swRefPlaneReferenceConstraints\_e

*SecondConstraintAngleOrDistance*
:   Angle or distance of the second constraint

*ThirdConstraint*
:   Third constraint as defined in swRefPlaneReferenceConstraints\_e

*ThirdConstraintAngleOrDistance*
:   Angle or distance of the third constraint

#### Return Value

[Reference plane](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IRefPlane.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertRefPlane.

# ![](dotnetimages/collapse.gif)Example

[Insert Reference Plane (C#)](Insert_Reference_Plane_Example_CSharp.htm)

[Insert Reference Plane (VB.NET)](Insert_Reference_Plane_Example_VBNET.htm)

[Insert Reference Plane (VBA)](Insert_Reference_Plane_Example_VB.htm)

[Insert Fill-surface Feature (C#)](Insert_Fill-surface_Feature_Example_CSharp.htm)

[Insert Fill-surface Feature (VB.NET)](Insert_Fill-surface_Feature_Example_VBNET.htm)

[Insert Fill-surface Feature (VBA)](Insert_Fill-surface_Feature_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, you must have selected the reference entities using these marks with [IModelDocExtension::SelectByID2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SelectByID2.html):

* 0 = First reference entity* 1 = Second reference entity* 2 = Third reference entity

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IRefPlane Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlane.html)

[IRefPlaneFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlaneFeatureData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0