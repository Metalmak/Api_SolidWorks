<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~GetModelBreakViewNames.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetModelBreakViewNames Method (IModelDocExtension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : GetModelBreakViewNames Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Views*
:   Names of Model Break Views

Gets the names and number of the Model Break Views in the current configuration of the active model.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetModelBreakViewNames( _    ByRef Views As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim Views As System.Object Dim value As System.Integer   value = instance.GetModelBreakViewNames(Views) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetModelBreakViewNames(     out System.object Views ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetModelBreakViewNames(  &   [Out] System.Object^ Views ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Views*
:   Names of Model Break Views

#### Return Value

Number of Model Break Views

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::GetModelBreakViewNames.

# ![](dotnetimages/collapse.gif)Example

[Get Names and Show Model Break Views (C#)](Get_Names_and_Show_Model_Break_Views_Example_CSharp.htm)

[Get Names and Show Model Break Views (VB.NET)](Get_Names_and_Show_Model_Break_Views_Example_VBNET.htm)

[Get Names and Show Model Break Views (VBA)](Get_Names_and_Show_Model_Break_Views_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

[IModelDocExtension::ShowModelBreakView Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~ShowModelBreakView.html)

[IView3D::ModelBreakViewName Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView3D~ModelBreakViewName.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2015 FCS, Revision Number 23.0