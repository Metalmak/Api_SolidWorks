<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~IListExternalFileReferences2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IListExternalFileReferences2 Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : IListExternalFileReferences2 Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NumRefs*

*ModelPathName*

*CompPathName*

*Feature*

*DataType*

*Status*

*RefEntity*

*FeatComp*

Obsolete. Superseded by [IModelDocExtension::ListExternalReferences](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~ListExternalFileReferences.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub IListExternalFileReferences2( _    ByVal NumRefs As System.Integer, _    ByRef ModelPathName As System.String, _    ByRef CompPathName As System.String, _    ByRef Feature As System.String, _    ByRef DataType As System.String, _    ByRef Status As System.Integer, _    ByRef RefEntity As System.String, _    ByRef FeatComp As System.String _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim NumRefs As System.Integer Dim ModelPathName As System.String Dim CompPathName As System.String Dim Feature As System.String Dim DataType As System.String Dim Status As System.Integer Dim RefEntity As System.String Dim FeatComp As System.String   instance.IListExternalFileReferences2(NumRefs, ModelPathName, CompPathName, Feature, DataType, Status, RefEntity, FeatComp) ``` | |

| C# |  |
| --- | --- |
| ``` void IListExternalFileReferences2(     System.int NumRefs,    out System.string ModelPathName,    out System.string CompPathName,    out System.string Feature,    out System.string DataType,    out System.int Status,    out System.string RefEntity,    out System.string FeatComp ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void IListExternalFileReferences2(  &   System.int NumRefs, &   [Out] System.String^ ModelPathName, &   [Out] System.String^ CompPathName, &   [Out] System.String^ Feature, &   [Out] System.String^ DataType, &   [Out] System.int Status, &   [Out] System.String^ RefEntity, &   [Out] System.String^ FeatComp ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*NumRefs*

*ModelPathName*

*CompPathName*

*Feature*

*DataType*

*Status*

*RefEntity*

*FeatComp*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::IListExternalFileReferences2.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)