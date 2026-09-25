<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEntity~ModelName.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ModelName Property (IEntity) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IEntity Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEntity.html) : ModelName Property (IEntity) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the standard Parasolid name attribute of the entity.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property ModelName As System.String ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IEntity Dim value As System.String   instance.ModelName = value   value = instance.ModelName ``` | |

| C# |  |
| --- | --- |
| ``` System.string ModelName {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.String^ ModelName {    System.String^ get();    void set ( &   System.String^ value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

Standard Parasolid name attribute

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Entity::ModelName.

# ![](dotnetimages/collapse.gif)Example

This Visual Basic subroutine shows how to write a Parasolid name attribute to each face in the model.

Private Sub NameAllFaces (ByRef swBody as SldWorks.body2)

> Dim swFace as Sldworks.Face2
>
> Dim swEnt As Sldworks.Entity
>
> Dim Name, RootName As String
>
> Dim Index As Integer
>
> Dim ret as Boolean

> swFace = swBody.GetFirstFace
>
> Index = 0
>
> RootName = "My Face #"
>
> Do While Not swFace is Nothing
>
> > swEnt = swFace
> >
> > Name = RootName + str(Index)
> >
> > swEnt.ModelName = Name
> >
> > Index = Index + 1
> >
> > swFace = swFace.GetNextFace
>
> Loop

End Sub

# ![](dotnetimages/collapse.gif)See Also

####

[IEntity Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEntity.html)

[IEntity Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEntity_members.html)