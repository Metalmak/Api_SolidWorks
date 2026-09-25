<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAttributeDef~CreateInstance2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateInstance2 Method (IAttributeDef) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAttributeDef Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAttributeDef.html) : CreateInstance2 Method (IAttributeDef) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*OwnerDoc*

*OwnerEntity*

*NameIn*

*Options*

Obsolete. Superseded by [IAttributeDef::CreateInstance5](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAttributeDef~CreateInstance5.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateInstance2( _    ByVal OwnerDoc As System.Object, _    ByVal OwnerEntity As System.Object, _    ByVal NameIn As System.String, _    ByVal Options As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAttributeDef Dim OwnerDoc As System.Object Dim OwnerEntity As System.Object Dim NameIn As System.String Dim Options As System.Integer Dim value As System.Object   value = instance.CreateInstance2(OwnerDoc, OwnerEntity, NameIn, Options) ``` | |

| C# |  |
| --- | --- |
| ``` System.object CreateInstance2(     System.object OwnerDoc,    System.object OwnerEntity,    System.string NameIn,    System.int Options ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ CreateInstance2(  &   System.Object^ OwnerDoc, &   System.Object^ OwnerEntity, &   System.String^ NameIn, &   System.int Options ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*OwnerDoc*

*OwnerEntity*

*NameIn*

*Options*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AttributeDef::CreateInstance2.

# ![](dotnetimages/collapse.gif)See Also

####

[IAttributeDef Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAttributeDef.html)

[IAttributeDef Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAttributeDef_members.html)