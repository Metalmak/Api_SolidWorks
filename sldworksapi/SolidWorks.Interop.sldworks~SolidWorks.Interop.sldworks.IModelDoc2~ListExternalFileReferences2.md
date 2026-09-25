<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ListExternalFileReferences2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ListExternalFileReferences2 Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : ListExternalFileReferences2 Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ModelPathName*

*ComponentPathName*

*Feature*

*DataType*

*Status*

*RefEntity*

*FeatCom*

Obsolete. Superseded by [IModelDocExtension::ListExternalReferences](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~ListExternalFileReferences.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub ListExternalFileReferences2( _    ByRef ModelPathName As System.Object, _    ByRef ComponentPathName As System.Object, _    ByRef Feature As System.Object, _    ByRef DataType As System.Object, _    ByRef Status As System.Object, _    ByRef RefEntity As System.Object, _    ByRef FeatCom As System.Object _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim ModelPathName As System.Object Dim ComponentPathName As System.Object Dim Feature As System.Object Dim DataType As System.Object Dim Status As System.Object Dim RefEntity As System.Object Dim FeatCom As System.Object   instance.ListExternalFileReferences2(ModelPathName, ComponentPathName, Feature, DataType, Status, RefEntity, FeatCom) ``` | |

| C# |  |
| --- | --- |
| ``` void ListExternalFileReferences2(     out System.object ModelPathName,    out System.object ComponentPathName,    out System.object Feature,    out System.object DataType,    out System.object Status,    out System.object RefEntity,    out System.object FeatCom ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void ListExternalFileReferences2(  &   [Out] System.Object^ ModelPathName, &   [Out] System.Object^ ComponentPathName, &   [Out] System.Object^ Feature, &   [Out] System.Object^ DataType, &   [Out] System.Object^ Status, &   [Out] System.Object^ RefEntity, &   [Out] System.Object^ FeatCom ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ModelPathName*

*ComponentPathName*

*Feature*

*DataType*

*Status*

*RefEntity*

*FeatCom*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::ListExternalFileReferences2.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)