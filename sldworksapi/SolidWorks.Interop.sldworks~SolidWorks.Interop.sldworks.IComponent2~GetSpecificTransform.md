<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetSpecificTransform.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetSpecificTransform Method (IComponent2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IComponent2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2.html) : GetSpecificTransform Method (IComponent2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*IgnoreExplode*
:   True to get the component's collapsed transform when the assembly is exploded, false to get the component's exploded transform when the assembly is exploded

Get the collapsed or exploded transform of a component when the assembly is exploded.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetSpecificTransform( _    ByVal IgnoreExplode As System.Boolean _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IComponent2 Dim IgnoreExplode As System.Boolean Dim value As System.Object   value = instance.GetSpecificTransform(IgnoreExplode) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetSpecificTransform(     System.bool IgnoreExplode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetSpecificTransform(  &   System.bool IgnoreExplode ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*IgnoreExplode*
:   True to get the component's collapsed transform when the assembly is exploded, false to get the component's exploded transform when the assembly is exploded

#### Return Value

[Transform](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMathTransform.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Component2::GetSpecificTransform.

# ![](dotnetimages/collapse.gif)Example

[Get Collapsed Transform of Component in Exploded View (C#)](Get_Collapsed_Transform_of_Component_in_Exploded_View_Example_CSharp.htm)

[Get Collapsed Transform of Component in Exploded View (VB.NET)](Get_Collapsed_Transform_of_Component_in_Exploded_View_Example_VBNET.htm)

[Get Collapsed Transform of Component in Exploded View (VBA)](Get_Collapsed_Transform_of_Component_in_Exploded_View_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IComponent2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2.html)

[IComponent2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2_members.html)

[IComponent2::GetTotalTransform Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetTotalTransform.html)

[IComponent2::SetTransformAndSolve2 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~SetTransformAndSolve2.html)

[IComponent2::PresentationTransform Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~PresentationTransform.html)

[IComponent2::Transform2 Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~Transform2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2017 FCS, Revision Number 25.0