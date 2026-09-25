<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~ListExternalFileReferences2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ListExternalFileReferences2 Method (IFeature) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeature Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature.html) : ListExternalFileReferences2 Method (IFeature) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ModelPathName*
:   Array of path names of documents

*ComponentPathName*
:   Array of path names of referenced components

*Feature*
:   Array of in-context items (sketches, features, and so on)

*DataType*
:   Array of data used to create the items (converted edge or face, converted or offset sketch entity, body, and so on)

*Status*
:   Array of statuses of external reference as defined in swExternalReferenceStatus\_e

*RefEntity*
:   Array of actual items being used and the names of the documents that contain the items

*FeatCom*
:   Array of the names of the components in which the affected features exist; this information is only displayed when one or more RefEntity is in a different component in an assembly and does not apply to derived parts

*ConfigOption*
:   Configuration option as defined by swExternalFileReferencesConfig\_e

*ConfigName*
:   Name of the configuration when ConfigOption is swExternalFileReferencesNamedConfig

Gets the names and statuses of the external references on the feature in a part or assembly.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub ListExternalFileReferences2( _    ByRef ModelPathName As System.Object, _    ByRef ComponentPathName As System.Object, _    ByRef Feature As System.Object, _    ByRef DataType As System.Object, _    ByRef Status As System.Object, _    ByRef RefEntity As System.Object, _    ByRef FeatCom As System.Object, _    ByRef ConfigOption As System.Integer, _    ByRef ConfigName As System.String _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeature Dim ModelPathName As System.Object Dim ComponentPathName As System.Object Dim Feature As System.Object Dim DataType As System.Object Dim Status As System.Object Dim RefEntity As System.Object Dim FeatCom As System.Object Dim ConfigOption As System.Integer Dim ConfigName As System.String   instance.ListExternalFileReferences2(ModelPathName, ComponentPathName, Feature, DataType, Status, RefEntity, FeatCom, ConfigOption, ConfigName) ``` | |

| C# |  |
| --- | --- |
| ``` void ListExternalFileReferences2(     out System.object ModelPathName,    out System.object ComponentPathName,    out System.object Feature,    out System.object DataType,    out System.object Status,    out System.object RefEntity,    out System.object FeatCom,    out System.int ConfigOption,    out System.string ConfigName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void ListExternalFileReferences2(  &   [Out] System.Object^ ModelPathName, &   [Out] System.Object^ ComponentPathName, &   [Out] System.Object^ Feature, &   [Out] System.Object^ DataType, &   [Out] System.Object^ Status, &   [Out] System.Object^ RefEntity, &   [Out] System.Object^ FeatCom, &   [Out] System.int ConfigOption, &   [Out] System.String^ ConfigName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ModelPathName*
:   Array of path names of documents

*ComponentPathName*
:   Array of path names of referenced components

*Feature*
:   Array of in-context items (sketches, features, and so on)

*DataType*
:   Array of data used to create the items (converted edge or face, converted or offset sketch entity, body, and so on)

*Status*
:   Array of statuses of external reference as defined in swExternalReferenceStatus\_e

*RefEntity*
:   Array of actual items being used and the names of the documents that contain the items

*FeatCom*
:   Array of the names of the components in which the affected features exist; this information is only displayed when one or more RefEntity is in a different component in an assembly and does not apply to derived parts

*ConfigOption*
:   Configuration option as defined by swExternalFileReferencesConfig\_e

*ConfigName*
:   Name of the configuration when ConfigOption is swExternalFileReferencesNamedConfig

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Feature::ListExternalFileReferences2.

# ![](dotnetimages/collapse.gif)Example

[Get External References (VBA)](Get_External_References_Example_VB.htm)

[Get External References (VB.NET)](Get_External_References_Example_VBNET.htm)

[Get External References (C#)](Get_External_References_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IFeature Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature.html)

[IFeature Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature_members.html)

[IFeature::ListExternalFileReferencesCount Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~ListExternalFileReferencesCount.html)

[IFeature::UpdateExternalFileReferences Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~UpdateExternalFileReferences.html)

[IFeature::IListExternalFileReferences2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~IListExternalFileReferences2.html)

[IComponent2::IListExternalFileReferences2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IListExternalFileReferences2.html)

[IComponent2::ListExternalFileReferences2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~ListExternalFileReferences2.html)

[IComponent2::ListExternalFileReferencesCount Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~ListExternalFileReferencesCount.html)

[IComponent2::UpdateExternalFileReferences Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~UpdateExternalFileReferences.html)

[IModelDocExtension::IListExternalFileReferences Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~IListExternalFileReferences.html)

[IModelDocExtension::ListExternalFileReferences Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~ListExternalFileReferences.html)

[IModelDocExtension::ListExternalFileReferencesCount Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~ListExternalFileReferencesCount.html)

[IModelDocExtension::UpdateExternalFileReferences Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~UpdateExternalFileReferences.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12.0