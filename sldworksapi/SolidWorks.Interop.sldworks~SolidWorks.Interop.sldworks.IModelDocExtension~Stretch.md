<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~Stretch.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Stretch Method (IModelDocExtension) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : Stretch Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*KeepRelations*
:   True to keep the sketch relations intact, false to sever them

*BaseX*
:   x coordinate of the base point

*BaseY*
:   y coordinate of the base point

*DestX*
:   x coordinate of the destination stretch

*DestY*
:   y coordinate of the destination of the stretch

Stretch the selected entities.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub Stretch( _    ByVal KeepRelations As System.Boolean, _    ByVal BaseX As System.Double, _    ByVal BaseY As System.Double, _    ByVal DestX As System.Double, _    ByVal DestY As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim KeepRelations As System.Boolean Dim BaseX As System.Double Dim BaseY As System.Double Dim DestX As System.Double Dim DestY As System.Double   instance.Stretch(KeepRelations, BaseX, BaseY, DestX, DestY) ``` | |

| C# |  |
| --- | --- |
| ``` void Stretch(     System.bool KeepRelations,    System.double BaseX,    System.double BaseY,    System.double DestX,    System.double DestY ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void Stretch(  &   System.bool KeepRelations, &   System.double BaseX, &   System.double BaseY, &   System.double DestX, &   System.double DestY ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*KeepRelations*
:   True to keep the sketch relations intact, false to sever them

*BaseX*
:   x coordinate of the base point

*BaseY*
:   y coordinate of the base point

*DestX*
:   x coordinate of the destination stretch

*DestY*
:   y coordinate of the destination of the stretch

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::Stretch.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 FCS, Revision Number 17.0