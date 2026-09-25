<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~InsertCoordinateSystem.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertCoordinateSystem Method (IModelDoc2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : InsertCoordinateSystem Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*XFlippedIn*
:   True to flip the x direction, false to not

*YFlippedIn*
:   True to flip the y direction, false to not

*ZFlippedIn*
:   True to flip the z direction, false to not

Obsolete. Superseded by [IFeatureManager::InsertCoordinateSystem](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~InsertCoordinateSystem.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertCoordinateSystem( _    ByVal XFlippedIn As System.Boolean, _    ByVal YFlippedIn As System.Boolean, _    ByVal ZFlippedIn As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim XFlippedIn As System.Boolean Dim YFlippedIn As System.Boolean Dim ZFlippedIn As System.Boolean Dim value As System.Boolean   value = instance.InsertCoordinateSystem(XFlippedIn, YFlippedIn, ZFlippedIn) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool InsertCoordinateSystem(     System.bool XFlippedIn,    System.bool YFlippedIn,    System.bool ZFlippedIn ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool InsertCoordinateSystem(  &   System.bool XFlippedIn, &   System.bool YFlippedIn, &   System.bool ZFlippedIn ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*XFlippedIn*
:   True to flip the x direction, false to not

*YFlippedIn*
:   True to flip the y direction, false to not

*ZFlippedIn*
:   True to flip the z direction, false to not

#### Return Value

True if coordinate system is added successfully, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::InsertCoordinateSystem.

# ![](dotnetimages/collapse.gif)Example

[Insert Coordinate System at Center of Mass (VBA)](Insert_Coordinate_System_at_Center_of_Mass_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Make the selections using [IModelDocExtension::SelectByID2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SelectByID2.html) with a mark of:

* 1 - Origin

  * 2 - X axis

    * 4 - Y axis

      * 8 - Z axis

This method:

* does not require all three axis to be selected. The behavior is the same as interactively creating a coordinate system. See the SOLIDWORKS Help for more information.* works in section-view mode, but not if temporary geometry that only exists in section-view mode is selected.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

[IModelDoc2::GetCurrentCoordinateSystemName Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~GetCurrentCoordinateSystemName.html)

[IModelDocExtension::GetCoordinateSystemTransformByName Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~GetCoordinateSystemTransformByName.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0