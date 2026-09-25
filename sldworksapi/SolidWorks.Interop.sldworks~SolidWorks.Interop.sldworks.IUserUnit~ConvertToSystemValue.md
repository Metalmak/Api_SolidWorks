<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IUserUnit~ConvertToSystemValue.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ConvertToSystemValue Method (IUserUnit) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IUserUnit Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IUserUnit.html) : ConvertToSystemValue Method (IUserUnit) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*UnitText*
:   Value to convert

*ComputedValue*
:   Converted value in document units

Converts a text string to a document unit value.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ConvertToSystemValue( _    ByVal UnitText As System.String, _    ByRef ComputedValue As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IUserUnit Dim UnitText As System.String Dim ComputedValue As System.Double Dim value As System.Boolean   value = instance.ConvertToSystemValue(UnitText, ComputedValue) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ConvertToSystemValue(     System.string UnitText,    out System.double ComputedValue ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ConvertToSystemValue(  &   System.String^ UnitText, &   [Out] System.double ComputedValue ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*UnitText*
:   Value to convert

*ComputedValue*
:   Converted value in document units

#### Return Value

True if successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See UserUnit::ConvertToSystemValue.

# ![](dotnetimages/collapse.gif)Example

See the [IUserUnit](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IUserUnit.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

This takes the value directly from a textbox control and passes it in to convert to a double value.

This imitates the behavior of when working in the SOLIDWORKS user interface and passing a value like "10 / 2" into one of the values on a dialog box.

# ![](dotnetimages/collapse.gif)See Also

####

[IUserUnit Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IUserUnit.html)

[IUserUnit Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IUserUnit_members.html)

[IUserUnit::ConvertDoubleToSystemValue Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IUserUnit~ConvertDoubleToSystemValue.html)

[IUserUnit::ConvertToUserUnit Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IUserUnit~ConvertToUserUnit.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001 FCS, Revision Number 9.0