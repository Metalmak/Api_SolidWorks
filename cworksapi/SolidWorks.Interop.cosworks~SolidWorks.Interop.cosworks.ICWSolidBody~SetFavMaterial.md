<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidBody~SetFavMaterial.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetFavMaterial Method (ICWSolidBody) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWSolidBody Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidBody.html) : SetFavMaterial Method (ICWSolidBody) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NFav*
:   1 <= index of material in favorites list <= 100 (see **Remarks**)

Obsolete. Superseded by [ICWSolidBody::SetFavMaterial2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidBody~SetFavMaterial2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetFavMaterial( _    ByVal NFav As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWSolidBody Dim NFav As System.Integer Dim value As System.Integer   value = instance.SetFavMaterial(NFav) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetFavMaterial(     System.int NFav ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetFavMaterial(  &   System.int NFav ) ``` | |

#### Parameters

*NFav*
:   1 <= index of material in favorites list <= 100 (see **Remarks**)

#### Return Value

0 if material applied successfully, 1 if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWSolidBody::SetFavMaterial.

# ![](dotnetimages/collapse.gif)Remarks

The list of material favorites appears when you right-click a component in the Simulation study tree and click **Apply Favorite Material**.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWSolidBody Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidBody.html)

[ICWSolidBody Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidBody_members.html)

[ICWSolidBody::SetSolidBodyMaterial Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidBody~SetSolidBodyMaterial.html)

[ICWSolidBody::SetLibraryMaterial Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidBody~SetLibraryMaterial.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2015 SP3