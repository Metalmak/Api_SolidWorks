<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~AddOrdinateDimension.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddOrdinateDimension Method (IModelDocExtension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : AddOrdinateDimension Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DimType*
:   Dimension type as defined in swAddOrdinateDims\_e

*LocX*
:   X location for the dimension

*LocY*
:   Y location for the dimension

*LocZ*
:   Z location for the dimension

Inserts an ordinate dimension.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddOrdinateDimension( _    ByVal DimType As System.Integer, _    ByVal LocX As System.Double, _    ByVal LocY As System.Double, _    ByVal LocZ As System.Double _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim DimType As System.Integer Dim LocX As System.Double Dim LocY As System.Double Dim LocZ As System.Double Dim value As System.Integer   value = instance.AddOrdinateDimension(DimType, LocX, LocY, LocZ) ``` | |

| C# |  |
| --- | --- |
| ``` System.int AddOrdinateDimension(     System.int DimType,    System.double LocX,    System.double LocY,    System.double LocZ ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int AddOrdinateDimension(  &   System.int DimType, &   System.double LocX, &   System.double LocY, &   System.double LocZ ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*DimType*
:   Dimension type as defined in swAddOrdinateDims\_e

*LocX*
:   X location for the dimension

*LocY*
:   Y location for the dimension

*LocZ*
:   Z location for the dimension

#### Return Value

Error as defined by swCreateOrdDimError\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::AddOrdinateDimension.

# ![](dotnetimages/collapse.gif)Example

[Display Grid Bubble (VBA)](Display_Grid_Bubble_Example_VB.htm)

[Create Ordinate Dimensions (C#)](Create_Ordinate_Dimensions_Example_CSharp.htm)

[Create Ordinate Dimensions (VB.NET)](Create_Ordinate_Dimensions_Example_VBNET.htm)

[Create Ordinate Dimensions (VBA)](Create_Ordinate_Dimensions_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Before using this method, select the base entity to act as the datum point for the ordinate dimension and any additional entities to include in the group of ordinate dimensions.

Selections made immediately after calling this method continue to add ordinate dimensions to the group of ordinate dimensions. When you finish adding ordinate dimensions to the group, use [IModelDoc2::SetPickMode](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~SetPickMode.html) to return to the default selection mode.

Use [IModelDoc2::EditOrdinate](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~EditOrdinate.html) to add ordinate dimensions to an existing group of ordinate dimensions.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

[IDisplayDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension.html)

[IModelDocExtension::JogDimension Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~JogDimension.html)

[IModelDoc2::AlignOrdinate Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~AlignOrdinate.html)

[IModelDoc2::ReattachOrdinate Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ReattachOrdinate.html)

[IDrawingDoc::AlignOrdinate Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~AlignOrdinate.html)

[IDrawingDoc::CreateOrdinateDim4 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~CreateOrdinateDim4.html)

[IDrawingDoc::EditOrdinate Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~EditOrdinate.html)

[IDrawingDoc::InsertHorizontalOrdinate Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~InsertHorizontalOrdinate.html)

[IDrawingDoc::InsertVerticalOrdinate Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~InsertVerticalOrdinate.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0