<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAttributeDef.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IAttributeDef Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAttributeDef_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IAttributeDef Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Allows access to an attribute definition.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface IAttributeDef ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAttributeDef ``` | |

| C# |  |
| --- | --- |
| ``` public interface IAttributeDef ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IAttributeDef ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AttributeDef.

# ![](dotnetimages/collapse.gif)Example

[Create Attribute (VBA)](Create_Attribute_Example_VB.htm)

[Add Attribute to Feature and Include in Library Feature (C#)](Add_Attribute_to_Feature_and_Include_in_Library_Feature_Example_CSharp.htm)

[Add Attribute to Feature and Include in Library Feature (VB.NET)](Add_Attribute_to_Feature_and_Include_in_Library_Feature_Example_VBNET.htm)

[Add Attribute to Feature and Include in Library Feature (VBA)](Add_Attribute_to_Feature_and_Include_In_Library_Feature_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

An attribute definition is an application-specific data packet that is automatically saved with the SOLIDWORKS file and reloaded when the file is opened. An application can create [attribute](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAttribute.html) data that is attached to an entity in a SOLIDWORKS document.

The attribute definition describes a template for the data packet. The definition contains the names of the parameters in the attribute, their types and default values. It also allows you to create instances of the definition on entities in your model.

The general sequence of steps in IAttribute creation is to:

1. Create an attribute definition ([ISldWorks::DefineAttribute](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~DefineAttribute.html))- Add parameters to the attribute definition ([IAttributeDef::AddParameter](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAttributeDef~AddParameter.html))- Register the attribute definition ([IAttributeDef::Register](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAttributeDef~Register.html))- Create instances of the attribute definition on objects throughout the model ([IAttributeDef::CreateInstance5](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAttributeDef~CreateInstance5.html))

Perform Steps 1 through 3 only once for each working session. In other words, perform Steps 1 through 3 when your DLL or EXE is initially loaded or run. Until the DLL is unloaded or the EXE is closed, you can create an unlimited number of instances of the attribute definition.

# ![](dotnetimages/collapse.gif)Accessors

[IAttribute::GetDefinition](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAttribute~GetDefinition.html) and [IAttribute::IGetDefinition Method](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAttribute~IGetDefinition.html)

[ISldWorks::DefineAttribute](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~DefineAttribute.html) and [ISldWorks::IDefineAttribute Method](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~IDefineAttribute.html)

# ![](dotnetimages/collapse.gif)Access Diagram

[AttributeDef](SWObjectModel.pdf#AttributeDef)

# ![](dotnetimages/collapse.gif)See Also

####

[IAttributeDef Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAttributeDef_members.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)