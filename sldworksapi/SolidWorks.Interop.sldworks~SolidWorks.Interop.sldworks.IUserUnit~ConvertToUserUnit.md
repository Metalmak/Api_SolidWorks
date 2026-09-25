<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IUserUnit~ConvertToUserUnit.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ConvertToUserUnit Method (IUserUnit) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IUserUnit Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IUserUnit.html) : ConvertToUserUnit Method (IUserUnit) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ValueIn*
:   Value to convert

*ShowUsernames*
:   True to show the user names, false to not

*NameInEnglish*
:   True to return the name in English, false to not

Converts the input value to document units.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ConvertToUserUnit( _    ByVal ValueIn As System.Double, _    ByVal ShowUsernames As System.Boolean, _    ByVal NameInEnglish As System.Boolean _ ) As System.String ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IUserUnit Dim ValueIn As System.Double Dim ShowUsernames As System.Boolean Dim NameInEnglish As System.Boolean Dim value As System.String   value = instance.ConvertToUserUnit(ValueIn, ShowUsernames, NameInEnglish) ``` | |

| C# |  |
| --- | --- |
| ``` System.string ConvertToUserUnit(     System.double ValueIn,    System.bool ShowUsernames,    System.bool NameInEnglish ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.String^ ConvertToUserUnit(  &   System.double ValueIn, &   System.bool ShowUsernames, &   System.bool NameInEnglish ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ValueIn*
:   Value to convert

*ShowUsernames*
:   True to show the user names, false to not

*NameInEnglish*
:   True to return the name in English, false to not

#### Return Value

Conversion to a string

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See UserUnit::ConvertToUserUnit.

# ![](dotnetimages/collapse.gif)Example

See the [IUserUnit](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IUserUnit.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[IUserUnit Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IUserUnit.html)

[IUserUnit Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IUserUnit_members.html)

[IUserUnit::ConvertDoubleToSystemValue Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IUserUnit~ConvertDoubleToSystemValue.html)

[IUserUnit::ConvertToSystemValue Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IUserUnit~ConvertToSystemValue.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001 FCS, Revision Number 9.0