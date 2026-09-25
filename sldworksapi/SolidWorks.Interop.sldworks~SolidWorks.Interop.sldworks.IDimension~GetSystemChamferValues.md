<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~GetSystemChamferValues.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetSystemChamferValues Method (IDimension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension.html) : GetSystemChamferValues Method (IDimension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Length*
:   Length of chamfer

*Angle*
:   Angle of chamfer

Gets the chamfer dimension values in system units.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetSystemChamferValues( _    ByRef Length As System.Double, _    ByRef Angle As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDimension Dim Length As System.Double Dim Angle As System.Double Dim value As System.Boolean   value = instance.GetSystemChamferValues(Length, Angle) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetSystemChamferValues(     out System.double Length,    out System.double Angle ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetSystemChamferValues(  &   [Out] System.double Length, &   [Out] System.double Angle ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Length*
:   Length of chamfer

*Angle*
:   Angle of chamfer

#### Return Value

True if the dimension is a chamfer dimension, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Dimension::GetSystemChamferValues.

# ![](dotnetimages/collapse.gif)Example

[Get Chamfer Dimension (C#)](Get_Chamfer_Dimension_Example_CSharp.htm)

[Get Chamfer Dimension (VB.NET)](Get_Chamfer_Dimension_Example_VBNET.htm)

[Get Chamfer Dimension (VBA)](Get_Chamfer_Dimension_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Unlike most other types of dimensions, the values returned for a chamfer dimension are not necessarily the values seen by the user in the displayed dimension text. The display dimension interprets these values and considers the type of chamfer display requested by the user and then creates an appropriate output string.

# ![](dotnetimages/collapse.gif)See Also

####

[IDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension.html)

[IDimension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension_members.html)

[IDrawingDoc::AddChamferDim Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~AddChamferDim.html)

[IDrawingDoc::IAddChamferDim Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~IAddChamferDim.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 SP1, Revision Number 14.1