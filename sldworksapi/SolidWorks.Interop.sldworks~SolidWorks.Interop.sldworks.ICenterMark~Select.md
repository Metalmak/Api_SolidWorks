<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICenterMark~Select.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Select Method (ICenterMark) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICenterMark Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICenterMark.html) : Select Method (ICenterMark) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Append*
:   True appends the center mark to the selection list, false replaces the selection list with this center mark

*Data*
:   [SelectData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISelectData.html) object

Selects the center mark.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function Select( _    ByVal Append As System.Boolean, _    ByVal Data As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICenterMark Dim Append As System.Boolean Dim Data As System.Object Dim value As System.Boolean   value = instance.Select(Append, Data) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool Select(     System.bool Append,    System.object Data ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool Select(  &   System.bool Append, &   System.Object^ Data ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Append*
:   True appends the center mark to the selection list, false replaces the selection list with this center mark

*Data*
:   [SelectData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISelectData.html) object

#### Return Value

True if the center mark is selected, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CenterMark::Select.

# ![](dotnetimages/collapse.gif)See Also

####

[ICenterMark Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICenterMark.html)

[ICenterMark Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICenterMark_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2016 FCS, Revision Number 24.0