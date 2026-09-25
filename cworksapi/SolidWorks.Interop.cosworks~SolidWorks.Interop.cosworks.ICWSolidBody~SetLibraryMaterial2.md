<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidBody~SetLibraryMaterial2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetLibraryMaterial2 Method (ICWSolidBody) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWSolidBody Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidBody.html) : SetLibraryMaterial2 Method (ICWSolidBody) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SLibWithPathName*
:   Path to the material library folder

*SMaterialName*
:   Material name

Sets the material library for the solid body.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetLibraryMaterial2( _    ByVal SLibWithPathName As System.String, _    ByVal SMaterialName As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWSolidBody Dim SLibWithPathName As System.String Dim SMaterialName As System.String Dim value As System.Boolean   value = instance.SetLibraryMaterial2(SLibWithPathName, SMaterialName) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetLibraryMaterial2(     System.string SLibWithPathName,    System.string SMaterialName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetLibraryMaterial2(  &   System.String^ SLibWithPathName, &   System.String^ SMaterialName ) ``` | |

#### Parameters

*SLibWithPathName*
:   Path to the material library folder

*SMaterialName*
:   Material name

#### Return Value

-1 or true if material library and name are set, 0 or false if not

# ![](dotnetimages/collapse.gif)Example

See the [ICWSolidBody](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidBody.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWSolidBody Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidBody.html)

[ICWSolidBody Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidBody_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2022 FCS, Revision Number 30