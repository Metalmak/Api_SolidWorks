<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~GetCorresponding2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetCorresponding2 Method (IModelDocExtension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : GetCorresponding2 Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*InputObject*
:   Object in this drawing view or assembly (see **Remarks**)

Gets the object in the underlying part or subassembly document that corresponds to the specified input object in this drawing view or assembly.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetCorresponding2( _    ByVal InputObject As System.Object _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim InputObject As System.Object Dim value As System.Object   value = instance.GetCorresponding2(InputObject) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetCorresponding2(     System.object InputObject ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetCorresponding2(  &   System.Object^ InputObject ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*InputObject*
:   Object in this drawing view or assembly (see **Remarks**)

#### Return Value

Corresponding object in the underlying part or subassembly; null or Nothing if none found (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::GetCorresponding2.

# ![](dotnetimages/collapse.gif)Example

[Get Corresponding Entities Between Parts and Drawing Views (VBA)](Get_Corresponding_Entities_Between_Parts_and_Views_Example_VB.htm)

[Get Corresponding Entities Between Parts and Drawing Views (VB.NET)](Get_Corresponding_Entities_Between_Parts_and_Views_Example_VBNET.htm)

[Get Corresponding Entities Between Parts and Drawing Views (C#)](Get_Corresponding_Entities_Between_Parts_and_Views_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

InputObject can be any object assigned a persistent reference ID; for example, a [IFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html), [IAnnotation](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAnnotation.html) or [ISketch](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch.html) object.

To get the assembly object corresponding to a given component object, use [IComponent2::GetCorresponding](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetCorresponding.html).

To get the drawing view object corresponding to a given part or assembly object, use [IView::GetCorresponding](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetCorresponding.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

[IModelDocExtension::GetCorrespondingEntity2 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~GetCorrespondingEntity2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2018 FCS, Revision Number 26.0