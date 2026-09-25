<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~CreateMassProperty.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateMassProperty Method (IModelDocExtension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : CreateMassProperty Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Obsolete. Superseded by [IModelDocExtension::CreateMassProperty2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~CreateMassProperty2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateMassProperty() As MassProperty ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim value As MassProperty   value = instance.CreateMassProperty() ``` | |

| C# |  |
| --- | --- |
| ``` MassProperty CreateMassProperty() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` MassProperty^ CreateMassProperty(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

[IMassProperty](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMassProperty.html) object

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::CreateMassProperty.

# ![](dotnetimages/collapse.gif)Example

[Insert Coordinate System at Center of Mass (VBA)](Insert_Coordinate_System_at_Center_of_Mass_Example_VB.htm)

[Set Dimensions to Mid-Tolerance (VBA)](Set_Dimensions_to_Mid-Tolerance_Example_VB.htm)

[Get Mass Properties of Multibody Assembly Component (VBA)](Get_Mass_Properties_of_Multibody_Assembly_Component_Example_VB.htm)

[Get Mass Properties of Multibody Assembly Component (C#)](Get_Mass_Properties_of_Multibody_Assembly_Component_Example_CSharp.htm)

[Get Mass Properties of Multibody Assembly Component (VB.NET)](Get_Mass_Properties_of_Multibody_Assembly_Component_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

The IMassProperty object obtains mass property information about one or more solid bodies in the document from which the IMassProperty object is obtained.

Only use solid bodies for the mass property calculations. You can specify the coordinate system about which the moments is calculated using [IMassProperty::SetCoordinateSystem](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMassProperty~SetCoordinateSystem.html). If you do not use IMassProperty::SetCoordinateSystem, then the documents origin is the coordinate system.

The results of the mass property calculations vary based on whether or not [IMassProperty::AddBodies](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMassProperty~AddBodies.html) or [IMassProperty::IAddBodies](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMassProperty~IAddBodies.html) is used.

|  |  |
| --- | --- |
| **If IMassProperty::AddBodies or IMassProperty::IAddBodies is...** | **Then...** |
| Called and bodies are specified | These bodies can either be from a subset of the documents body list or from temporary bodies.    NOTE: Each specified body should either come from the owning document or be a temporary body. If the body does not satisfy either case, then it is not used when calculating the mass properties. |
| Not called | Mass properties' calculations include all available bodies in the document.   * Part. All of the solid bodies are included in the calculations.   * Assembly. All of the bodies in all of the components are used in the calculations. |

If the document from which the IMassProperty object came is an assembly, then any body from any of the child components can be used. To obtain the body, call [IComponent2::GetBodies2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2~GetBodies2.html). Your application does not need to make a copy of the body or apply a transform to the body.

IModelDocExtension::CreateMassProperty gets the recalculated up-to-date values regardless of the [IModelDocExtension::NeedsRebuild](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~NeedsRebuild.html) status.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

[IModelDocExtension::GetMassProperties2 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~GetMassProperties2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2003 SP2, Revision Number 11.2