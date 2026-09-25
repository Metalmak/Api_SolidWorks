<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension~AddDisplayEnt.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddDisplayEnt Method (IDisplayDimension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDisplayDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension.html) : AddDisplayEnt Method (IDisplayDimension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Type*
:   Type of graphical entity (see **Remarks**)

*Data*
:   Geometric data describing the entity (see **Remarks**)

Overrides the display graphics of objects.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddDisplayEnt( _    ByVal Type As System.Integer, _    ByVal Data As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDisplayDimension Dim Type As System.Integer Dim Data As System.Object Dim value As System.Boolean   value = instance.AddDisplayEnt(Type, Data) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool AddDisplayEnt(     System.int Type,    System.object Data ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool AddDisplayEnt(  &   System.int Type, &   System.Object^ Data ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Type*
:   Type of graphical entity (see **Remarks**)

*Data*
:   Geometric data describing the entity (see **Remarks**)

#### Return Value

True if successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DisplayDimension::AddDisplayEnt.

# ![](dotnetimages/collapse.gif)Example

[Replace Dimension with Text (VBA)](Replace_Dimension_with_Text_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

The new graphics displayed by this method are temporary. When the user changes the dimension, this display dimension reverts back to the SOLIDWORKS standard.

The type controls which geometry is added and what information is placed in the data array. All colors and line styles are taken from DisplayDimension.

|  |  |  |
| --- | --- | --- |
| type | Description | data |
| 1 | Line | 6 doubles; (x, y, z) start point and (x, y, z) end point |
| 2 | Filled triangle | 9 doubles; 3 (x, y, z) points of the triangle to fill |
| 3 | Filled 4 sided polygon | 12 doubles; 4 (x, y, z) points of the polygon to fill |
| 4 | Arc | 12 doubles; (x, y, z) center point, (x, y, z) normal vector, (x, y, z) start point and (x, y, z) end point |
| 5 | Circle | 7 doubles; (x, y, z) center point, (x, y, z) normal vector and radius |
| 6 | Filled dot | 4 doubles; (x, y, z) center point and radius |

# ![](dotnetimages/collapse.gif)See Also

####

[IDisplayDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension.html)

[IDisplayDimension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension_members.html)

[IDisplayDimension::IAddDisplayText Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension~IAddDisplayText.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001 FCS, Revision Number 9.0