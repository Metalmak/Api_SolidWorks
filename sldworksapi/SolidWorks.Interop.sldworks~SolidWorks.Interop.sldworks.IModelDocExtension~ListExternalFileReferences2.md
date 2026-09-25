<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~ListExternalFileReferences2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ListExternalFileReferences2 Method (IModelDocExtension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : ListExternalFileReferences2 Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ModelPathName*
:   Array of path names of externally referenced model documents

*ComponentPathName*
:   Array of path names of externally referenced assembly components

*Feature*
:   Array of in-context items (e.g., FeatureManager design tree sketches, features, and so on) that externally reference ModelPathName and ComponentPathName elements

*DataType*
:   Array of data types used to create RefEntity (e.g., arc, line, sketch plane, converted edge or face, converted or offset sketch entity, body, and so on)

*Status*
:   Array of statuses of the external references as defined by swExternalReferenceStatus\_e

*RefEntity*
:   Array of actual items being used (FeatureManager design tree entities in the Feature parameter's external references) and the names of the documents containing the items

*FeatCom*
:   Array of names of the components in which the affected Features exist; valid only if one or more RefEntity is in a different component in an assembly; not valid for derived parts

*ConfigOptions*
:   Array of configuration options as defined by swExternalFileReferencesConfig\_e

*ConfigNames*
:   Array of configuration names when corresponding element of ConfigOptions array contains swExternalFileReferencesNamedConfig, empty strings otherwise

Gets the specified external file reference information for this part or assembly.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub ListExternalFileReferences2( _    ByRef ModelPathName As System.Object, _    ByRef ComponentPathName As System.Object, _    ByRef Feature As System.Object, _    ByRef DataType As System.Object, _    ByRef Status As System.Object, _    ByRef RefEntity As System.Object, _    ByRef FeatCom As System.Object, _    ByRef ConfigOptions As System.Object, _    ByRef ConfigNames As System.Object _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim ModelPathName As System.Object Dim ComponentPathName As System.Object Dim Feature As System.Object Dim DataType As System.Object Dim Status As System.Object Dim RefEntity As System.Object Dim FeatCom As System.Object Dim ConfigOptions As System.Object Dim ConfigNames As System.Object   instance.ListExternalFileReferences2(ModelPathName, ComponentPathName, Feature, DataType, Status, RefEntity, FeatCom, ConfigOptions, ConfigNames) ``` | |

| C# |  |
| --- | --- |
| ``` void ListExternalFileReferences2(     out System.object ModelPathName,    out System.object ComponentPathName,    out System.object Feature,    out System.object DataType,    out System.object Status,    out System.object RefEntity,    out System.object FeatCom,    out System.object ConfigOptions,    out System.object ConfigNames ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void ListExternalFileReferences2(  &   [Out] System.Object^ ModelPathName, &   [Out] System.Object^ ComponentPathName, &   [Out] System.Object^ Feature, &   [Out] System.Object^ DataType, &   [Out] System.Object^ Status, &   [Out] System.Object^ RefEntity, &   [Out] System.Object^ FeatCom, &   [Out] System.Object^ ConfigOptions, &   [Out] System.Object^ ConfigNames ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ModelPathName*
:   Array of path names of externally referenced model documents

*ComponentPathName*
:   Array of path names of externally referenced assembly components

*Feature*
:   Array of in-context items (e.g., FeatureManager design tree sketches, features, and so on) that externally reference ModelPathName and ComponentPathName elements

*DataType*
:   Array of data types used to create RefEntity (e.g., arc, line, sketch plane, converted edge or face, converted or offset sketch entity, body, and so on)

*Status*
:   Array of statuses of the external references as defined by swExternalReferenceStatus\_e

*RefEntity*
:   Array of actual items being used (FeatureManager design tree entities in the Feature parameter's external references) and the names of the documents containing the items

*FeatCom*
:   Array of names of the components in which the affected Features exist; valid only if one or more RefEntity is in a different component in an assembly; not valid for derived parts

*ConfigOptions*
:   Array of configuration options as defined by swExternalFileReferencesConfig\_e

*ConfigNames*
:   Array of configuration names when corresponding element of ConfigOptions array contains swExternalFileReferencesNamedConfig, empty strings otherwise

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::ListExternalFileReferences2.

# ![](dotnetimages/collapse.gif)Example

[Get External References (VBA)](Get_External_References_Example_VB.htm)

[Get External References (VB.NET)](Get_External_References_Example_VBNET.htm)

[Get External References (C#)](Get_External_References_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method conveniently collects the same information that is displayed when you right-click on a feature or component with **{ -> }** at the end of its name in the FeatureManager design tree and select **External References...** from the context menu.

The External References dialog displays the assembly or part name of the external reference, configuration if applicable, name of the feature in this document that has an external reference, status of the external reference, the entity in the external reference to which this feature or component points, and the data type of the external reference entity.

For more information, see the **SOLIDWORKS user-interface help > Assemblies > Top-Down Design > External References > External References Dialog Box**.

The elements of the arrays returned by this method map one to one.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

[IModelDocExtension::ListExternalFileReferencesCount Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~ListExternalFileReferencesCount.html)

[IModelDocExtension::UpdateExternalFileReferences Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~UpdateExternalFileReferences.html)

[IModelDoc2::BreakAllExternalReferences Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~BreakAllExternalReferences.html)

[IModelDoc2::ListAuxiliaryExternalFileReferences Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ListAuxiliaryExternalFileReferences.html)

[IModelDoc2::LockAllExternalReferences Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~LockAllExternalReferences.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2021 SP01, Revision Number 29.1