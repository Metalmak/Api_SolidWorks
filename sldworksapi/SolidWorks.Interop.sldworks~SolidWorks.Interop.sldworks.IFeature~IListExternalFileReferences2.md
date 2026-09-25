<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~IListExternalFileReferences2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IListExternalFileReferences2 Method (IFeature) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeature Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature.html) : IListExternalFileReferences2 Method (IFeature) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NumRefs*
:   Number of external references

*ModelPathName*
:   * in-process, unmanaged C++: Pointer to an array of path names of documents of size NumRefs

    * VBA, VB.NET, C#, and C++/CLI: Not supported

*CompPathName*
:   * in-process, unmanaged C++: Pointer to an array of path names of referenced components of size NumRefs

    * VBA, VB.NET, C#, and C++/CLI: Not supported

*Feature*
:   * in-process, unmanaged C++: Pointer to an array of in-context items (sketches, features, and so on) of size NumRefs* VBA, VB.NET, C#, and C++/CLI: Not supported

*DataType*
:   * in-process, unmanaged C+: Pointer to an array of data used to create the items (converted edge or face, converted or offset sketch entity, body, and so on) of size NumRefs* VBA, VB.NET, C#, and C++/CLI: Not supported

*Status*
:   * in-process, unmanaged C++: Pointer of an array of the statuses of external references as defined in swExternalReferenceStatus\_e

    - VBA, VB.NET, C#, and C++/CLI: Not supported

*RefEntity*
:   * in-process, unmanaged C++: Pointer to an array of actual items being used and the names of the documents that contain the items of size NumRefs* VBA, VB.NET, C#, and C++/CLI: Not supported

*FeatComp*
:   * in-process, unmanaged C++: Pointer to an array of the names of the components in which the affected features exist of size NumRefs; this information is only displayed when one or more RefEntity is in a different component in an assembly and does not apply to derived parts* VBA, VB.NET, C#, and C++/CLI: Not supported

*ConfigOption*
:   Configuration option as defined by swExternalFileReferencesConfig\_e

*ConfigName*
:   Name of the configuration when ConfigOption is swExternalFileReferencesNamedConfig

Gets the names and statuses of the external references for this feature in a part or assembly.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub IListExternalFileReferences2( _    ByVal NumRefs As System.Integer, _    ByRef ModelPathName As System.String, _    ByRef CompPathName As System.String, _    ByRef Feature As System.String, _    ByRef DataType As System.String, _    ByRef Status As System.Integer, _    ByRef RefEntity As System.String, _    ByRef FeatComp As System.String, _    ByRef ConfigOption As System.Integer, _    ByRef ConfigName As System.String _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeature Dim NumRefs As System.Integer Dim ModelPathName As System.String Dim CompPathName As System.String Dim Feature As System.String Dim DataType As System.String Dim Status As System.Integer Dim RefEntity As System.String Dim FeatComp As System.String Dim ConfigOption As System.Integer Dim ConfigName As System.String   instance.IListExternalFileReferences2(NumRefs, ModelPathName, CompPathName, Feature, DataType, Status, RefEntity, FeatComp, ConfigOption, ConfigName) ``` | |

| C# |  |
| --- | --- |
| ``` void IListExternalFileReferences2(     System.int NumRefs,    out System.string ModelPathName,    out System.string CompPathName,    out System.string Feature,    out System.string DataType,    out System.int Status,    out System.string RefEntity,    out System.string FeatComp,    out System.int ConfigOption,    out System.string ConfigName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void IListExternalFileReferences2(  &   System.int NumRefs, &   [Out] System.String^ ModelPathName, &   [Out] System.String^ CompPathName, &   [Out] System.String^ Feature, &   [Out] System.String^ DataType, &   [Out] System.int Status, &   [Out] System.String^ RefEntity, &   [Out] System.String^ FeatComp, &   [Out] System.int ConfigOption, &   [Out] System.String^ ConfigName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*NumRefs*
:   Number of external references

*ModelPathName*
:   * in-process, unmanaged C++: Pointer to an array of path names of documents of size NumRefs

    * VBA, VB.NET, C#, and C++/CLI: Not supported

*CompPathName*
:   * in-process, unmanaged C++: Pointer to an array of path names of referenced components of size NumRefs

    * VBA, VB.NET, C#, and C++/CLI: Not supported

*Feature*
:   * in-process, unmanaged C++: Pointer to an array of in-context items (sketches, features, and so on) of size NumRefs* VBA, VB.NET, C#, and C++/CLI: Not supported

*DataType*
:   * in-process, unmanaged C+: Pointer to an array of data used to create the items (converted edge or face, converted or offset sketch entity, body, and so on) of size NumRefs* VBA, VB.NET, C#, and C++/CLI: Not supported

*Status*
:   * in-process, unmanaged C++: Pointer of an array of the statuses of external references as defined in swExternalReferenceStatus\_e

    - VBA, VB.NET, C#, and C++/CLI: Not supported

*RefEntity*
:   * in-process, unmanaged C++: Pointer to an array of actual items being used and the names of the documents that contain the items of size NumRefs* VBA, VB.NET, C#, and C++/CLI: Not supported

*FeatComp*
:   * in-process, unmanaged C++: Pointer to an array of the names of the components in which the affected features exist of size NumRefs; this information is only displayed when one or more RefEntity is in a different component in an assembly and does not apply to derived parts* VBA, VB.NET, C#, and C++/CLI: Not supported

*ConfigOption*
:   Configuration option as defined by swExternalFileReferencesConfig\_e

*ConfigName*
:   Name of the configuration when ConfigOption is swExternalFileReferencesNamedConfig

# ![](dotnetimages/collapse.gif)Remarks

Call [IFeature::ListExternalFileReferencesCount](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~ListExternalFileReferencesCount.html) before calling this method to specify NumRefs.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeature Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature.html)

[IFeature Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature_members.html)

[IFeature::ListExternalFileReferences2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~ListExternalFileReferences2.html)

[IFeature::UpdateExternalFileReferences Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~UpdateExternalFileReferences.html)

[IComponent2:IListExternalFileReferences2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IListExternalFileReferences2.html)

[IComponent2:ListExternalFileReferences2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~ListExternalFileReferences2.html)

[IComponent2:ListExternalFileReferencesCount Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~ListExternalFileReferencesCount.html)

[IComponent2::UpdateExternalFileReferences Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~UpdateExternalFileReferences.html)

[IModelDocExtension::IListExternalFileReferences Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~IListExternalFileReferences.html)

[IModelDocExtension::ListExternalFileReferences Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~ListExternalFileReferences.html)

[IModelDocExtension::ListExternalFileReferencesCount Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~ListExternalFileReferencesCount.html)

[IModelDocExtension::UpdateExternalFileReferences Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~UpdateExternalFileReferences.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12.0