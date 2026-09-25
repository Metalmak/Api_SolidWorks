<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetBodies3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetBodies3 Method (IComponent2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IComponent2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2.html) : GetBodies3 Method (IComponent2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BodyType*
:   Type of body as defined by swBodyType\_e

*BodiesInfo*
:   Array of information about the returned bodies as defined in swBodyInfo\_e

Gets the bodies in this component.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetBodies3( _    ByVal BodyType As System.Integer, _    ByRef BodiesInfo As System.Object _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IComponent2 Dim BodyType As System.Integer Dim BodiesInfo As System.Object Dim value As System.Object   value = instance.GetBodies3(BodyType, BodiesInfo) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetBodies3(     System.int BodyType,    out System.object BodiesInfo ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetBodies3(  &   System.int BodyType, &   [Out] System.Object^ BodiesInfo ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*BodyType*
:   Type of body as defined by swBodyType\_e

*BodiesInfo*
:   Array of information about the returned bodies as defined in swBodyInfo\_e

#### Return Value

Array of [bodies](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html) in the component

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Component2::GetBodies3.

# ![](dotnetimages/collapse.gif)Example

Also see the [IView::GetVisibleDrawingComponents](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetVisibleDrawingComponents.html) examples.

# ![](dotnetimages/collapse.gif)Example

[Get Bodies in Components (C#)](Get_Bodies_in_Components_Example_CSharp.htm)

[Get Bodies in Components (VB.NET)](Get_Bodies_in_Components_Example_VBNET.htm)

[Get Bodies in Components (VBA)](Get_Bodies_in_Components_Example_VB.htm)

[Get Bodies in Components (C++)](Get_Bodies_in_Components_Example_CPlusPlus_COM.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method:

* Only supports solid and surface bodies and part components,

* May vary the order in which bodies are returned,

* Supports lightweight components (the now obsolete IComponent2::GetBodies does not),

     - and -

* Returns an array in BodiesInfo containing information about bodies that indicates whether they are normal or user bodies. User bodies are original component bodies that have been modified in an assembly (e.g., a normal component body is cut in the assembly, resulting in two user component bodies). User bodies are not created for surface bodies.

# ![](dotnetimages/collapse.gif)See Also

####

[IComponent2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2.html)

[IComponent2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2_members.html)

[IComponent2::EnumBodies2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~EnumBodies2.html)

[IComponent2::GetBody Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetBody.html)

[IComponent2::IGetBody Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IGetBody.html)

[IPartDoc::GetBodies2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc~GetBodies2.html)

[IBody2::IsSheetMetal Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IsSheetMetal.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 SP4, Revision Number 17.4