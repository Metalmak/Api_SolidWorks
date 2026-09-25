<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreateEllipse.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateEllipse Method (ISketchManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html) : CreateEllipse Method (ISketchManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*XC*
:   X coordinate of the ellipse center point

*YC*
:   Y coordinate of the ellipse center point

*Zc*
:   Z coordinate of the ellipse center point

*XMajor*
:   X coordinate of the point on the ellipse that is on the major axis

*YMajor*
:   Y coordinate of the point on the ellipse that is on the major axis

*ZMajor*
:   Z coordinate of the point on the ellipse that is on the major axis

*XMinor*
:   X coordinate of the point on the ellipse that is on the minor axis

*YMinor*
:   Y coordinate of the point on the ellipse that is on the minor axis

*ZMinor*
:   Z coordinate of the point on the ellipse that is on the minor axis

Creates an ellipse using the specified center, major-axis, and minor-axis points.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateEllipse( _    ByVal XC As System.Double, _    ByVal YC As System.Double, _    ByVal Zc As System.Double, _    ByVal XMajor As System.Double, _    ByVal YMajor As System.Double, _    ByVal ZMajor As System.Double, _    ByVal XMinor As System.Double, _    ByVal YMinor As System.Double, _    ByVal ZMinor As System.Double _ ) As SketchSegment ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchManager Dim XC As System.Double Dim YC As System.Double Dim Zc As System.Double Dim XMajor As System.Double Dim YMajor As System.Double Dim ZMajor As System.Double Dim XMinor As System.Double Dim YMinor As System.Double Dim ZMinor As System.Double Dim value As SketchSegment   value = instance.CreateEllipse(XC, YC, Zc, XMajor, YMajor, ZMajor, XMinor, YMinor, ZMinor) ``` | |

| C# |  |
| --- | --- |
| ``` SketchSegment CreateEllipse(     System.double XC,    System.double YC,    System.double Zc,    System.double XMajor,    System.double YMajor,    System.double ZMajor,    System.double XMinor,    System.double YMinor,    System.double ZMinor ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` SketchSegment^ CreateEllipse(  &   System.double XC, &   System.double YC, &   System.double Zc, &   System.double XMajor, &   System.double YMajor, &   System.double ZMajor, &   System.double XMinor, &   System.double YMinor, &   System.double ZMinor ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*XC*
:   X coordinate of the ellipse center point

*YC*
:   Y coordinate of the ellipse center point

*Zc*
:   Z coordinate of the ellipse center point

*XMajor*
:   X coordinate of the point on the ellipse that is on the major axis

*YMajor*
:   Y coordinate of the point on the ellipse that is on the major axis

*ZMajor*
:   Z coordinate of the point on the ellipse that is on the major axis

*XMinor*
:   X coordinate of the point on the ellipse that is on the minor axis

*YMinor*
:   Y coordinate of the point on the ellipse that is on the minor axis

*ZMinor*
:   Z coordinate of the point on the ellipse that is on the minor axis

#### Return Value

[Sketch segment](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchSegment.html) for the ellipse

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SketchManager::CreateEllipse.

# ![](dotnetimages/collapse.gif)Example

[Create Ellipse (VBA)](Create_Ellipse_Example_VB.htm)

[Create Ellipse (VB.NET)](Create_Ellipse_Example_VBNET.htm)

[Create Ellipse (C#)](Create_Ellipse_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method creates a full ellipse in the active 2D sketch. If a sketch is not active, then a new sketch is created. You can check for an active sketch using [ISketchManager::ActiveSketch](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchManager~ActiveSketch.html).

[ISketchManager::AddToDB](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchManager~AddToDB.html) and [ISketchManager::DisplayWhenAdded](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchManager~DisplayWhenAdded.html) increase performance during entity creation by adding entities directly to the SOLIDWORKS database.

ISketchManager::AddToDB also avoids some of the peculiarities involved with creating entities via the user interface, such as inferencing, automatic relations, and snapping to the grid. Adding entities directly to the database also significantly increases the performance of this method. When you are done creating entities, it is important to ISketchManager::AddToDB(False), to restore SOLIDWORKS to its normal operating mode.

This method also works with ISketchManager::DisplayWhenAdded. If you have called ISketchManager::AddToDB(True), additional performance can be gained by calling ISketchManager::DisplayWhenAdded(False) to disable immediate display of entities as they are added to the database. When you are done creating all of your sketch entities, you must redraw your document window (see [IModelView::GraphicsRedraw](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelView~GraphicsRedraw.html) or [IModelView::IGraphicsRedraw](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelView~IGraphicsRedraw.html)) to see the entities you added. You should also restore the original display settings by calling ISketchManager::DisplayWhenAdded(True).

To create a partial ellipse, use [ISketchManager::CreateEllipticalArc](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchManager~CreateEllipticalArc.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html)

[ISketchManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager_members.html)

[ISketchManager::CreateConic Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreateConic.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0