<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDatumTargetSym~GetDatumReferenceLabel.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetDatumReferenceLabel Method (IDatumTargetSym) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDatumTargetSym Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDatumTargetSym.html) : GetDatumReferenceLabel Method (IDatumTargetSym) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*WhichOne*
:   0-based index indicating the datum reference label to get

Gets the specified datum target reference label.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetDatumReferenceLabel( _    ByVal WhichOne As System.Integer _ ) As System.String ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDatumTargetSym Dim WhichOne As System.Integer Dim value As System.String   value = instance.GetDatumReferenceLabel(WhichOne) ``` | |

| C# |  |
| --- | --- |
| ``` System.string GetDatumReferenceLabel(     System.int WhichOne ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.String^ GetDatumReferenceLabel(  &   System.int WhichOne ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*WhichOne*
:   0-based index indicating the datum reference label to get

#### Return Value

Datum reference label

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DatumTargetSym::GetDatumReferenceLabel.

# ![](dotnetimages/collapse.gif)Example

[Insert and Modify Datum Target Symbol (C#)](Insert_and_Modify_Datum_Target_Symbol_Example_CSharp.htm)

[Insert and Modify Datum Target Symbol (VB.NET)](Insert_and_Modify_Datum_Target_Symbol_Example_VBNET.htm)

[Insert and Modify Datum Target Symbol (VBA)](Insert_and_Modify_Datum_Target_Symbol_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IDatumTargetSym Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDatumTargetSym.html)

[IDatumTargetSym Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDatumTargetSym_members.html)

[IDatumTargetSym::SetDatumReferenceLabel Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDatumTargetSym~SetDatumReferenceLabel.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2000 FCS, Revision Number 8.0