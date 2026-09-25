<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~GetSearchData.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetSearchData Method (IModelDocExtension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : GetSearchData Method (IModelDocExtension) |

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

*AppNames*
:   Array of strings of the third-party application name

*NodeNames*
:   Array of strings of the third-party application name's keywords

*NodeValues*
:   Array of strings of the third-party application name's keyword values

Gets the SOLIDWORKS Search, third-party, application keywords from the model document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetSearchData( _    ByVal AppName As System.String, _    ByRef AppNames As System.Object, _    ByRef NodeNames As System.Object, _    ByRef NodeValues As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim AppName As System.String Dim AppNames As System.Object Dim NodeNames As System.Object Dim NodeValues As System.Object Dim value As System.Integer   value = instance.GetSearchData(AppName, AppNames, NodeNames, NodeValues) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetSearchData(     System.string AppName,    out System.object AppNames,    out System.object NodeNames,    out System.object NodeValues ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetSearchData(  &   System.String^ AppName, &   [Out] System.Object^ AppNames, &   [Out] System.Object^ NodeNames, &   [Out] System.Object^ NodeValues ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*AppName*
:   Third-party application name whose keywords to get

*AppNames*
:   Array of strings of the third-party application name

*NodeNames*
:   Array of strings of the third-party application name's keywords

*NodeValues*
:   Array of strings of the third-party application name's keyword values

#### Return Value

Number of third-party application name's keywords

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::GetSearchData.

# ![](dotnetimages/collapse.gif)Example

[Get SOLIDWORKS Search Third-party Keywords (VBA)](Get_SOLIDWORKS_Search_Third-party_Keywords_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

[IModelDocExtension::IGetSearchData Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~IGetSearchData.html)

[IModelDocExtension::AddOrUpdateSearchData Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~AddOrUpdateSearchData.html)

[IModelDocExtension::DeleteSearchData Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~DeleteSearchData.html)

[IModelDocExtension::GetSearchDataCount Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~GetSearchDataCount.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0