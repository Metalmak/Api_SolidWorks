<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~GetObjectId.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetObjectId Method (IModelDocExtension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : GetObjectId Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Annotation*
:   [Annotation](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation.html)

Gets the object ID for the specified annotation.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetObjectId( _    ByVal Annotation As Annotation _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim Annotation As Annotation Dim value As System.Integer   value = instance.GetObjectId(Annotation) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetObjectId(     Annotation Annotation ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetObjectId(  &   Annotation^ Annotation ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Annotation*
:   [Annotation](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation.html)

#### Return Value

Object ID

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::GetObjectId.

# ![](dotnetimages/collapse.gif)Example

[Get Object ID of GTol Annotation (C#)](Get_Object_ID_of_GTol_Annotation_Example_CSharp.htm)

[Get Object ID of GTol Annotation (VB.NET)](Get_Object_ID_of_GTol_Annotation_Example_VBNET.htm)

[Get Object ID of GTol Annotation (VBA)](Get_Object_ID_of_GTol_Annotation_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2014 SP5, Revision Number 22.5