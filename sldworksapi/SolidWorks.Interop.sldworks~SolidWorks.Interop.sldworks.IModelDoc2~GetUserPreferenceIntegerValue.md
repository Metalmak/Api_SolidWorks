<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~GetUserPreferenceIntegerValue.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetUserPreferenceIntegerValue Method (IModelDoc2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : GetUserPreferenceIntegerValue Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*UserPreferenceValue*
:   Value as defined in swUserPreferenceIntegerValue\_e

Obsolete. Superseded by [IModelDocExtension::GetUserPreferenceInteger](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~GetUserPreferenceInteger.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetUserPreferenceIntegerValue( _    ByVal UserPreferenceValue As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim UserPreferenceValue As System.Integer Dim value As System.Integer   value = instance.GetUserPreferenceIntegerValue(UserPreferenceValue) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetUserPreferenceIntegerValue(     System.int UserPreferenceValue ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetUserPreferenceIntegerValue(  &   System.int UserPreferenceValue ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*UserPreferenceValue*
:   Value as defined in swUserPreferenceIntegerValue\_e

#### Return Value

Numeric value associated with the specified UserPreferenceValue

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::GetUserPreferenceIntegerValue.

# ![](dotnetimages/collapse.gif)Example

[Get Material Properties (VBA)](Get_Material_Properties_Example_VB.htm)

[Make Part Transparent (VBA)](Make_Part_Transparent_Example_VB.htm)

[Save Document as TIFF (VBA)](Save_As_Tiff_Example_VB.htm)

[Set Grid Lines (VBA)](Set_Grid_Lines_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method is equivalent to interactively getting document properties in the SOLIDWORKS product. See System Options and Document Properties for details.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0