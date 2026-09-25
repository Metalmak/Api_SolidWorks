<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetWitnessEntitiesCount.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetWitnessEntitiesCount Method (IView) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html) : GetWitnessEntitiesCount Method (IView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Size*
:   Size of the virtual sharp witness line data array (see **Remarks**)

Gets the number of virtual sharp witness lines in this drawing view.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetWitnessEntitiesCount( _    ByRef Size As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IView Dim Size As System.Integer Dim value As System.Integer   value = instance.GetWitnessEntitiesCount(Size) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetWitnessEntitiesCount(     out System.int Size ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetWitnessEntitiesCount(  &   [Out] System.int Size ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Size*
:   Size of the virtual sharp witness line data array (see **Remarks**)

#### Return Value

Number of virtual sharp witness lines in this drawing view

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See View::GetWitnessEntitiesCount.

# ![](dotnetimages/collapse.gif)Example

[Get Virtual Sharp Witness Line Data (VBA)](Get_Virtual_Sharp_Witness_Line_Data_Example_VB.htm)

[Get Virtual Sharp Witness Line Data (VB.NET)](Get_Virtual_Sharp_Witness_Line_Data_Example_VBNET.htm)

[Get Virtual Sharp Witness Line Data (C#)](Get_Virtual_Sharp_Witness_Line_Data_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Call this method to get the sizes of the arrays returned by [IView::GetWitnessGeomInfo](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~GetWitnessGeomInfo.html) and [IView::IGetWitnessGeomInfo](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~IGetWitnessGeomInfo.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html)

[IView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2012 FCS, Revision Number 20.0