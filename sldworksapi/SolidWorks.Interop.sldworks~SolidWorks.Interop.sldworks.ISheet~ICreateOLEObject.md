<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet~ICreateOLEObject.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ICreateOLEObject Method (ISheet) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISheet Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet.html) : ICreateOLEObject Method (ISheet) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Aspect*

*Position*

*ByteCount*

*Buffer*

Obsolete. Superseded by [IModelDocExtension::CreateOLEObject](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~CreateOLEObject.html) and [IModelDocExtension::ICreateOLEObject](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~ICreateOLEObject.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ICreateOLEObject( _    ByVal Aspect As System.Integer, _    ByRef Position As System.Double, _    ByVal ByteCount As System.Integer, _    ByRef Buffer As System.Byte _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISheet Dim Aspect As System.Integer Dim Position As System.Double Dim ByteCount As System.Integer Dim Buffer As System.Byte Dim value As System.Boolean   value = instance.ICreateOLEObject(Aspect, Position, ByteCount, Buffer) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ICreateOLEObject(     System.int Aspect,    ref System.double Position,    System.int ByteCount,    ref System.byte Buffer ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ICreateOLEObject(  &   System.int Aspect, &   System.double% Position, &   System.int ByteCount, &   System.byte% Buffer ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Aspect*

*Position*

*ByteCount*

*Buffer*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Sheet::ICreateOLEObject.

# ![](dotnetimages/collapse.gif)See Also

####

[ISheet Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet.html)

[ISheet Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet_members.html)