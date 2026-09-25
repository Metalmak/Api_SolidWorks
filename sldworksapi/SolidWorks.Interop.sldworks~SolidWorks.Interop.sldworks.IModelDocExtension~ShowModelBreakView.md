<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~ShowModelBreakView.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ShowModelBreakView Method (IModelDocExtension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : ShowModelBreakView Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ShowView*
:   True to show the Model Break View, false to hide it

*ViewName*
:   Name of Model Break View to show or hide

Gets whether to show or hide the specified Model Break View in the current configuration of the active model.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ShowModelBreakView( _    ByVal ShowView As System.Boolean, _    ByVal ViewName As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim ShowView As System.Boolean Dim ViewName As System.String Dim value As System.Boolean   value = instance.ShowModelBreakView(ShowView, ViewName) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ShowModelBreakView(     System.bool ShowView,    System.string ViewName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ShowModelBreakView(  &   System.bool ShowView, &   System.String^ ViewName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ShowView*
:   True to show the Model Break View, false to hide it

*ViewName*
:   Name of Model Break View to show or hide

#### Return Value

True if the method executed, false if it did not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::ShowModelBreakView.

# ![](dotnetimages/collapse.gif)Example

[Get Names and Show Model Break Views (C#)](Get_Names_and_Show_Model_Break_Views_Example_CSharp.htm)

[Get Names and Show Model Break Views (VB.NET)](Get_Names_and_Show_Model_Break_Views_Example_VBNET.htm)

[Get Names and Show Model Break Views (VBA)](Get_Names_and_Show_Model_Break_Views_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

[IModelDocExtension::GetModelBreakViewNames Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~GetModelBreakViewNames.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2015 FCS, Revision Number 23.0