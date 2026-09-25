<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISelectionMgr~AddSelectionListObject.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddSelectionListObject Method (ISelectionMgr) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISelectionMgr Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISelectionMgr.html) : AddSelectionListObject Method (ISelectionMgr) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Object*
:   Object to add to the selection list (see **Remarks**)

*SelectData*
:   [ISelectData](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISelectData.html)

Adds the specified object to the selection list.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddSelectionListObject( _    ByVal Object As System.Object, _    ByVal SelectData As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISelectionMgr Dim Object As System.Object Dim SelectData As System.Object Dim value As System.Boolean   value = instance.AddSelectionListObject(Object, SelectData) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool AddSelectionListObject(     System.object Object,    System.object SelectData ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool AddSelectionListObject(  &   System.Object^ Object, &   System.Object^ SelectData ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Object*
:   Object to add to the selection list (see **Remarks**)

*SelectData*
:   [ISelectData](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISelectData.html)

#### Return Value

True if successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SelectionMgr::AddSelectionListObject.

# ![](dotnetimages/collapse.gif)Example

[Insert Indent Feature (C#)](Insert_Indent_Feature_Example_CSharp.htm)

[Insert Indent Feature (VB.NET)](Insert_Indent_Feature_Example_VBNET.htm)

[Insert Indent Feature (VBA)](Insert_Indent_Feature_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Call [ISelectionMgr::CreateSelectData](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISelectionMgr~CreateSelectData.html) to specify SelectData.

To add objects to a selection list without pre-selecting the objects in the user interface:

1. Call [ISelectionMgr::SuspendSelectionList](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISelectionMgr~SuspendSelectionList.html) to suspend the current selection list, preserving its contents and starting a new selection list.- Call ISelectionMgr::AddSelectionListObject or [ISelectionMgr::AddSelectionListObjects](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISelectionMgr~AddSelectionListObjects.html) to populate the new selection list.- Process the objects in the new selection list.- Call [ISelectionMgr::ResumeSelectionList](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISelectionMgr~ResumeSelectionList.html) to reinstate the suspended selection list.

To programmatically pre-select objects in the user interface and add them to a selection list, use [IModelDocExtension::SelectByID2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SelectByID2.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ISelectionMgr Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISelectionMgr.html)

[ISelectionMgr Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISelectionMgr_members.html)

[ISelectionSetItem::GetCorrespondingItem Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISelectionSetItem~GetCorrespondingItem.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2012 FCS, Revision Number 20.0