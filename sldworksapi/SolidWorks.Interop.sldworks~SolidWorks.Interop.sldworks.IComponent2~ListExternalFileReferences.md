<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~ListExternalFileReferences.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ListExternalFileReferences Method (IComponent2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IComponent2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2.html) : ListExternalFileReferences Method (IComponent2) |

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

Obsolete. Superseded by [IComponent2::ListExternalFileReferences2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2~ListExternalFileReferences2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub ListExternalFileReferences( _    ByRef ModelPathName As System.Object, _    ByRef ComponentPathName As System.Object, _    ByRef Feature As System.Object, _    ByRef DataType As System.Object, _    ByRef Status As System.Object, _    ByRef RefEntity As System.Object, _    ByRef FeatCom As System.Object _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IComponent2 Dim ModelPathName As System.Object Dim ComponentPathName As System.Object Dim Feature As System.Object Dim DataType As System.Object Dim Status As System.Object Dim RefEntity As System.Object Dim FeatCom As System.Object   instance.ListExternalFileReferences(ModelPathName, ComponentPathName, Feature, DataType, Status, RefEntity, FeatCom) ``` | |

| C# |  |
| --- | --- |
| ``` void ListExternalFileReferences(     out System.object ModelPathName,    out System.object ComponentPathName,    out System.object Feature,    out System.object DataType,    out System.object Status,    out System.object RefEntity,    out System.object FeatCom ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void ListExternalFileReferences(  &   [Out] System.Object^ ModelPathName, &   [Out] System.Object^ ComponentPathName, &   [Out] System.Object^ Feature, &   [Out] System.Object^ DataType, &   [Out] System.Object^ Status, &   [Out] System.Object^ RefEntity, &   [Out] System.Object^ FeatCom ) ``` | |

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

See Component2::ListExternalFileReferences.

# ![](dotnetimages/collapse.gif)See Also

####

[IComponent2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2.html)

[IComponent2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2_members.html)