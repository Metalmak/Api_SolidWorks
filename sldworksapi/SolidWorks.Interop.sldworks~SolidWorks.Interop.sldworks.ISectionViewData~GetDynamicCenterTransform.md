<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISectionViewData~GetDynamicCenterTransform.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetDynamicCenterTransform Method (ISectionViewData) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISectionViewData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISectionViewData.html) : GetDynamicCenterTransform Method (ISectionViewData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Index*
:   Section (see **Remarks**)

Gets the translation between the center of the model and the plane in the specified section in this section view.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetDynamicCenterTransform( _    ByVal Index As System.Integer _ ) As MathTransform ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISectionViewData Dim Index As System.Integer Dim value As MathTransform   value = instance.GetDynamicCenterTransform(Index) ``` | |

| C# |  |
| --- | --- |
| ``` MathTransform GetDynamicCenterTransform(     System.int Index ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` MathTransform^ GetDynamicCenterTransform(  &   System.int Index ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Index*
:   Section (see **Remarks**)

#### Return Value

[Translation](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMathTransform.html) between the center of the model and the plane in the section specified for Index

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SectionViewData::GetDynamicCenterTransform.

# ![](dotnetimages/collapse.gif)Example

[Get Section View Data (C#)](Get_Section_View_Data_Example_CSharp.htm)

[Get Section View Data (VB.NET)](Get_Section_View_Data_Example_VBNET.htm)

[Get Section View Data (VBA)](Get_Section_View_Data_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method is only valid for section views having more than one section. Specify:

* 1 for Section 1* 2 for Section 2* 3 for Section 3

If the section view contains only one section and you specify 1 for Index, then this method returns Nothing or null.

# ![](dotnetimages/collapse.gif)See Also

####

[ISectionViewData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISectionViewData.html)

[ISectionViewData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISectionViewData_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2015 SP2, Revision Number 23.2