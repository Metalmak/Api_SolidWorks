<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~DefineAttribute.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DefineAttribute Method (ISldWorks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : DefineAttribute Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Name*
:   Name to give to the attribute definition; the name must be unique and qualified among the attributes defined in the current session (see Remarks)

Creates an attribute definition, which is the first step in generating attributes.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function DefineAttribute( _    ByVal Name As System.String _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim Name As System.String Dim value As System.Object   value = instance.DefineAttribute(Name) ``` | |

| C# |  |
| --- | --- |
| ``` System.object DefineAttribute(     System.string Name ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ DefineAttribute(  &   System.String^ Name ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Name*
:   Name to give to the attribute definition; the name must be unique and qualified among the attributes defined in the current session (see Remarks)

#### Return Value

[Attribute definition](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAttributeDef.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::DefineAttribute.

# ![](dotnetimages/collapse.gif)Example

[Create Attribute (VBA)](Create_Attribute_Example_VB.htm)

[Delete Faces (VBA)](Delete_Faces_Example_VB.htm)

[Add Attribute to Feature and Include in Library Feature (C#)](Add_Attribute_to_Feature_and_Include_in_Library_Feature_Example_CSharp.htm)

[Add Attribute to Feature and Include in Library Feature (VB.NET)](Add_Attribute_to_Feature_and_Include_in_Library_Feature_Example_VBNET.htm)

[Add Attribute to Feature and Include in Library Feature (VBA)](Add_Attribute_to_Feature_and_Include_In_Library_Feature_Example_VB.htm)

[Delete Blended Faces (C#)](Delete_Blended_Faces_Example_CSharp.htm)

[Delete Blended Faces (VB.NET)](Delete_Blended_Faces_Example_VBNET.htm)

[Delete Blended Faces (VBA)](Delete_Blended_Faces_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

An attribute definition is a container that can hold a group of parameters. For example, you can use this container to hold machining information or BOM data. Instances of this container may then be created as [IAttribute](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAttribute.html) objects on the document object, or on faces, edges, vertices, and features within the document. Once created, you can get any of the IAttribute objects and query or change its parameter values.

The Name argument used for this attribute definition must be unique and qualified among the attributes defined in the current session. To ensure this, the first three letters of the name must be an officially recognized third-party identifier. Contact SOLIDWORKS Corporation if you need one. You can also use the prefix: "pub" ( for "public" ) if you are just testing.

**General sequence of steps in attribute creation**

1. Create an attribute definition (ISldWorks::DefineAttribute or [ISldWorks::IDefineAttribute](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~IDefineAttribute.html))

   - Add parameters to the attribute definition ([IAttributeDef::AddParameter](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAttributeDef~AddParameter.html))

     - Register the attribute definition ([IAttributeDef::Register](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAttributeDef~Register.html))

       - Create instances of the attribute definition on objects throughout the model ([IAttributeDef::CreateInstance5](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAttributeDef~CreateInstance5.html))

Perform steps 1 through 3 only once for each working session. In other words, perform steps 1 through 3 when your DLL or EXE is initially loaded or run. Until the DLL is unloaded, or the EXE is closed, you can create as many instances of the attribute definition as you want as shown in step 4.

Calling this method attaches to an existing attribute definition with the specified Name or creates new attribute definition if a match is not found. The attribute definition exists throughout the current SOLIDWORKS session and persistent across SOLIDWORKS sessions if an attribute instance with that definition exists in the document. If an attribute definition exists, you cannot add or remove its parameters.

After an attribute instance is added to a face, edge, vertex, loop, feature, or document, there are several ways to get back to the attribute for query or modification.

1. Because an attribute instance is a feature, you can use any of the standard feature traversal routines (the FeatureByName methods, [IModelDoc2::FirstFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~FirstFeature.html) or [IModelDoc2::IFirstFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~IFirstFeature.html), and [IFeature::GetNextFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~GetNextFeature.html) or [IModelDoc2::IGetNextFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~IGetNextFeature.html)) to grab the feature representation of the attribute. After you have the [IFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html) object that represents the attribute instance, you can call [IFeature::GetSpecificFeature2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~GetSpecificFeature2.html) to get the underlying [IAttribute](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAttribute.html) object.

   - If the end-user selected the attribute in the FeatureManager design tree, you can use standard selection control to get the IFeature object representing the attribute instance ([ISelectionMgr::GetSelectedObject6](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISelectionMgr~GetSelectedObject6.html)) and then call IFeature::GetSpecificFeature2 to get the underlying IAttribute object.

     - If you are traversing body topology, then you can locate any IAttribute objects with a call to [IEntity::FindAttribute](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEntity~FindAttribute.html) or [IEntity::IFindAttribute](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEntity~IFindAttribute.html) from the particular [IEntity](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEntity.html) object (that is, face, edge, and so on). If the attribute instance was placed on the document, then you would need to use option 1 to get back to it.

After you have the IAttribute object that you want to query or modify, use the [IAttribute::GetParameter](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAttribute~GetParameter.html) or [IAttribute::IGetParameter](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAttribute~IGetParameter.html) method to return the desired attribute parameter object. The [IParameter](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IParameter.html) object provides a set of functions to query or modify specific attribute values.

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[ISldWorks::IDefineAttribute Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~IDefineAttribute.html)