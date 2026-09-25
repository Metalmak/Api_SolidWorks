<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~AddOrUpdateSearchData.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddOrUpdateSearchData Method (IModelDocExtension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : AddOrUpdateSearchData Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*AppName*
:   Third-party application name

*AppKeyword*
:   Third-party application keyword

*AppValue*
:   Value for AppKeyword

Adds or updates the SOLIDWORKS Search, third-party, application keyword and value to the model document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddOrUpdateSearchData( _    ByVal AppName As System.String, _    ByVal AppKeyword As System.String, _    ByVal AppValue As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim AppName As System.String Dim AppKeyword As System.String Dim AppValue As System.String Dim value As System.Boolean   value = instance.AddOrUpdateSearchData(AppName, AppKeyword, AppValue) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool AddOrUpdateSearchData(     System.string AppName,    System.string AppKeyword,    System.string AppValue ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool AddOrUpdateSearchData(  &   System.String^ AppName, &   System.String^ AppKeyword, &   System.String^ AppValue ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*AppName*
:   Third-party application name

*AppKeyword*
:   Third-party application keyword

*AppValue*
:   Value for AppKeyword

#### Return Value

True if the SOLIDWORKS Search, third-party, application keyword and value are added to the model document, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::AddOrUpdateSearchData.

# ![](dotnetimages/collapse.gif)Example

[Add Third-party Application Keywords to SOLIDWORKS Search and Model (VBA)](Add_Third-party_Application_Keywords_to_SOLIDWORKS_Search_and_Model_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

After calling this method and after the keyword has been indexed in SOLIDWORKS Search, type the third-party application name, keyword, or keyword value in the SOLIDWORKS Search box and press Enter. Any documents assigned any of these three strings will appear on the Search tab in the Task Pane.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

[IModelDocExtension::DeleteSearchData Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~DeleteSearchData.html)

[IModelDocExtension::GetSearchData Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~GetSearchData.html)

[IModelDocExtension::GetSearchDataCount Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~GetSearchDataCount.html)

[IModelDocExtension::IGetSearchData Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~IGetSearchData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0