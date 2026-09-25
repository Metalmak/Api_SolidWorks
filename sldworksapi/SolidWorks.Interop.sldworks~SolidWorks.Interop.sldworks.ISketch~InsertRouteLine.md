<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~InsertRouteLine.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertRouteLine Method (ISketch) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketch Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch.html) : InsertRouteLine Method (ISketch) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ItemsToConnect*
:   Array of faces, edges, and vertices to which to connect the route line

*Reverse*
:   Array of Booleans indicating whether to reverse the route line at the corresponding item to connect; true to reverse the direction of the route line, false to not

*AlternatePath*
:   Array of Booleans indicating whether to display an alternate path at the corresponding item to connect; true to display another possible path for the route line, false to not

*AlongXYZ*
:   Array of Booleans indicating whether to create a path parallel to the X, Y, and Z directions from the corresponding item to connect; true to use the X, Y, and Z directions, false to use the shortest route

Inserts a route line in an explode line sketch or a 3D sketch to indicate component relationships.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertRouteLine( _    ByVal ItemsToConnect As System.Object, _    ByVal Reverse As System.Object, _    ByVal AlternatePath As System.Object, _    ByVal AlongXYZ As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketch Dim ItemsToConnect As System.Object Dim Reverse As System.Object Dim AlternatePath As System.Object Dim AlongXYZ As System.Object Dim value As System.Boolean   value = instance.InsertRouteLine(ItemsToConnect, Reverse, AlternatePath, AlongXYZ) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool InsertRouteLine(     System.object ItemsToConnect,    System.object Reverse,    System.object AlternatePath,    System.object AlongXYZ ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool InsertRouteLine(  &   System.Object^ ItemsToConnect, &   System.Object^ Reverse, &   System.Object^ AlternatePath, &   System.Object^ AlongXYZ ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ItemsToConnect*
:   Array of faces, edges, and vertices to which to connect the route line

*Reverse*
:   Array of Booleans indicating whether to reverse the route line at the corresponding item to connect; true to reverse the direction of the route line, false to not

*AlternatePath*
:   Array of Booleans indicating whether to display an alternate path at the corresponding item to connect; true to display another possible path for the route line, false to not

*AlongXYZ*
:   Array of Booleans indicating whether to create a path parallel to the X, Y, and Z directions from the corresponding item to connect; true to use the X, Y, and Z directions, false to use the shortest route

#### Return Value

True if a route line is inserted, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Sketch::InsertRouteLine.

# ![](dotnetimages/collapse.gif)Example

[Insert Explode Line Sketch and Route Line (VB.NET)](Insert_Exploded_Line_Sketch_and_Route_Line_Example_VBNET.htm)

[Insert Explode Line Sketch and Route Line (VBA)](Insert_Exploded_Line_Sketch_and_Route_Line_Example_VB.htm)

[Insert Explode Line Sketch and Route Line (C#)](Insert_Exploded_Line_Sketch_and_Route_Line_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

You insert a route line in an [explode line sketch](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchManager~InsertExplodeLineSketch.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ISketch Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch.html)

[ISketch Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch_members.html)

[IAssemblyDoc::AutoExplode Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~AutoExplode.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0