<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc~GetBodies2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetBodies2 Method (IPartDoc) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPartDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc.html) : GetBodies2 Method (IPartDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BodyType*
:   Type of body as defined in swBodyType\_e

*BVisibleOnly*
:   True gets only the visible bodies, false gets all of the bodies in the part

Gets the bodies in this part.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetBodies2( _    ByVal BodyType As System.Integer, _    ByVal BVisibleOnly As System.Boolean _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPartDoc Dim BodyType As System.Integer Dim BVisibleOnly As System.Boolean Dim value As System.Object   value = instance.GetBodies2(BodyType, BVisibleOnly) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetBodies2(     System.int BodyType,    System.bool BVisibleOnly ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetBodies2(  &   System.int BodyType, &   System.bool BVisibleOnly ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*BodyType*
:   Type of body as defined in swBodyType\_e

*BVisibleOnly*
:   True gets only the visible bodies, false gets all of the bodies in the part

#### Return Value

Array of [bodies](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PartDoc::GetBodies2.

# ![](dotnetimages/collapse.gif)Example

[Get Bodies (C++)](Get_Bodies_Example_CPlusPlus_COM.htm)

[Traverse Bodies (C++)](Traverse_Bodies_Example_CPlusPlusCLI.htm)

[Set Body for View (C#)](Set_Body_for_View_Example_CSharp.htm)

[Set Body for Part (VB.NET)](Set_Body_for_View_Example_VBNET.htm)

[Set Body for Part (VBA)](Set_Body_for_View_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method:

* Only supports solid and sheet (surface) body types.* May vary the order in which bodies are returned.

# ![](dotnetimages/collapse.gif)See Also

####

[IPartDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc.html)

[IPartDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc_members.html)

[IComponent2::GetBodies2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetBodies2.html)

[IBodyFolder::GetBodies Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBodyFolder~GetBodies.html)

[IBodyFolder::IGetBodies Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBodyFolder~IGetBodies.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2003 FCS, Revision Number 11.0