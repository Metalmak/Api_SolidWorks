<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetBody.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetBody Method (IComponent2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IComponent2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2.html) : GetBody Method (IComponent2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the body that belongs to this instance of this component.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetBody() As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IComponent2 Dim value As System.Object   value = instance.GetBody() ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetBody() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetBody(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

Body

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Component2::GetBody.

# ![](dotnetimages/collapse.gif)Example

[Combine Assembly Components into Part (VBA)](Combine_Assembly_Components_into_Part_Example_VB.htm)

[Get Mass Properties of Assembly Component (VBA)](Get_Mass_Properties_of_Assembly_Component_Example_VB.htm)

[Get Material Properties (VBA)](Get_Material_Properties_Example_VB.htm)

[Select Component Face By Name (VBA)](Get_Component_Face_By_Name_Example_VB.htm)

[Display Temporary Body (C#)](Display_Temporary_Body_Example_CSharp.htm)

[Display Temporary Body (VB.NET)](Display_Temporary_Body_Example_VBNET.htm)

[Display Temporary Body (VBA)](Display_Temporary_Body_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method returns a valid IBody2 object only for fully resolved components that reference an [IPartDoc](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPartDoc.html). For the root component, lightweight components or components that reference an AssemblyDoc, this method returns a NULL body object. However, if a component is in a multibody part, then this method returns the first body.

For COM applications, this method returns the status code ITF\_E\_COMPONENTNOTRESOLVED.

This method is different from the IPartDoc::Body method in that it recognizes assembly-level features and returns that information based on the component instance. IPartDoc::Body never recognizes assembly-level features because the feature information is kept with the assembly, not propagated down to the part file.

For example, if PartABC is added to an assembly twice, then changes to that IPartDoc object would affect both instances of the assembly IComponent2. Likewise, querying information from that IPartDoc object will not recognize changes in the assembly that may have altered only one of the components (for example, an assembly-level feature was added to one of the components). However, the component object recognizes the two instances of PartABC as two distinct IComponent2 objects and returns its information from the assembly level.

For example, one assembly configuration might have an assembly-level feature that cuts a hole through each of the components in the assembly. Using this method on each of the assembly components returns the body of each component with the hole feature that was applied in this particular configuration. If you switch to the configuration
without the assembly-level hole and re-traverse the IComponent2 objects, then calling this method for each component returns the IBody2 object without the hole feature because it was applied in the other configuration.

For more information on lightweight components, see [IComponent2::GetSuppression](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2~GetSuppression.html), [IComponent2::SetSuppression2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2~SetSuppression2.html), and [IAssemblyDoc::ResolveAllLightWeightComponents](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAssemblyDoc~ResolveAllLightWeightComponents.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IComponent2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2.html)

[IComponent2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2_members.html)

[IComponent2::IGetBody Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IGetBody.html)

[IComponent2::EnumBodies2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~EnumBodies2.html)

[IComponent2::GetBodies3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetBodies3.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0