<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkageRod~SetLibraryMaterial.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetLibraryMaterial Method (ICWLinkageRod) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWLinkageRod Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkageRod.html) : SetLibraryMaterial Method (ICWLinkageRod) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SMaterialLibPathWithName*
:   Material library path name

*SMaterialName*
:   Material name

Sets the specified library material for this linkage rod connector.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetLibraryMaterial( _    ByVal SMaterialLibPathWithName As System.String, _    ByVal SMaterialName As System.String _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWLinkageRod Dim SMaterialLibPathWithName As System.String Dim SMaterialName As System.String   instance.SetLibraryMaterial(SMaterialLibPathWithName, SMaterialName) ``` | |

| C# |  |
| --- | --- |
| ``` void SetLibraryMaterial(     System.string SMaterialLibPathWithName,    System.string SMaterialName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetLibraryMaterial(  &   System.String^ SMaterialLibPathWithName, &   System.String^ SMaterialName ) ``` | |

#### Parameters

*SMaterialLibPathWithName*
:   Material library path name

*SMaterialName*
:   Material name

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWLinkageRod::SetLibraryMaterial.

# ![](dotnetimages/collapse.gif)Example

See the [ICWLinkageRod](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkageRod.html) examples

# ![](dotnetimages/collapse.gif)See Also

####

[ICWLinkageRod Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkageRod.html)

[ICWLinkageRod Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkageRod_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2022 SP0