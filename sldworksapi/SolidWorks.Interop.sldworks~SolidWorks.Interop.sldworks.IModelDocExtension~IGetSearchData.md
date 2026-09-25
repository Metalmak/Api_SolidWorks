<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~IGetSearchData.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetSearchData Method (IModelDocExtension) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : IGetSearchData Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*AppName*
:   Third-party application name whose keywords to get

*Count*
:   Number of third-party application keywords

*AppNames*
:   * in-process, unmanaged C++: Pointer to an array of the third-party application names

    - VBA, VB.NET, C#, and C++/CLI: Not supported

      See In-process Methods for details about this type of method.

*NodeNames*
:   * in-process, unmanaged C++: Pointer to an array of the third-party application name's keywords

    - VBA, VB.NET, C#, and C++/CLI: Not supported

*NodeValues*
:   * in-process, unmanaged C++: Pointer to an array of the third-party application name's keyword values

    - VBA, VB.NET, C#, and C++/CLI: Not supported

Gets the SOLIDWORKS Search, third-party, application keywords from the model document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub IGetSearchData( _    ByVal AppName As System.String, _    ByVal Count As System.Integer, _    ByRef AppNames As System.String, _    ByRef NodeNames As System.String, _    ByRef NodeValues As System.String _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim AppName As System.String Dim Count As System.Integer Dim AppNames As System.String Dim NodeNames As System.String Dim NodeValues As System.String   instance.IGetSearchData(AppName, Count, AppNames, NodeNames, NodeValues) ``` | |

| C# |  |
| --- | --- |
| ``` void IGetSearchData(     System.string AppName,    System.int Count,    out System.string AppNames,    out System.string NodeNames,    out System.string NodeValues ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void IGetSearchData(  &   System.String^ AppName, &   System.int Count, &   [Out] System.String^ AppNames, &   [Out] System.String^ NodeNames, &   [Out] System.String^ NodeValues ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*AppName*
:   Third-party application name whose keywords to get

*Count*
:   Number of third-party application keywords

*AppNames*
:   * in-process, unmanaged C++: Pointer to an array of the third-party application names

    - VBA, VB.NET, C#, and C++/CLI: Not supported

      See In-process Methods for details about this type of method.

*NodeNames*
:   * in-process, unmanaged C++: Pointer to an array of the third-party application name's keywords

    - VBA, VB.NET, C#, and C++/CLI: Not supported

*NodeValues*
:   * in-process, unmanaged C++: Pointer to an array of the third-party application name's keyword values

    - VBA, VB.NET, C#, and C++/CLI: Not supported

#### Return Value

Number of third-party application name's keywords

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, call [IModelDocExtension::GetSearchDataCount](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~GetSearchDataCount.html) to get the value of Count.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

[IModelDocExtension::AddOrUpdateSearchData Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~AddOrUpdateSearchData.html)

[IModelDocExtension::DeleteSearchData Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~DeleteSearchData.html)

[IModelDocExtension::GetSearchData Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~GetSearchData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0