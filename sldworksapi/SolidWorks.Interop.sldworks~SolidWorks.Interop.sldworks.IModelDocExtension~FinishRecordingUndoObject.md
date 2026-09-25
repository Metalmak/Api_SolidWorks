<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~FinishRecordingUndoObject.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| FinishRecordingUndoObject Method (IModelDocExtension) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : FinishRecordingUndoObject Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*UndoObjectName*
:   String to appear in SOLIDWORKS Undo list

Obsolete. Superseded by [IModelDocExtension::FinishRecordingUndoObject2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~FinishRecordingUndoObject2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function FinishRecordingUndoObject( _    ByVal UndoObjectName As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim UndoObjectName As System.String Dim value As System.Boolean   value = instance.FinishRecordingUndoObject(UndoObjectName) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool FinishRecordingUndoObject(     System.string UndoObjectName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool FinishRecordingUndoObject(  &   System.String^ UndoObjectName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*UndoObjectName*
:   String to appear in SOLIDWORKS Undo list

#### Return Value

True if recording of the SOLIDWORKS Undo object ends, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::FinishRecordingUndoObject.

# ![](dotnetimages/collapse.gif)Remarks

Place [IModelDocExtension::StartRecordingUndoObject](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~StartRecordingUndoObject.html) at the beginning and this method at the end of any SOLIDWORKS API calls in your application that you want your user to undo as a group.

For example, if your application creates a complex gear that requires many SOLIDWORKS API calls, place IModelDocExtension::StartRecordingUndoObject and this method around the SOLIDWORKS API calls that create that gear. Then your user need only select the string specified for UndoObjectName in the SOLIDWORKS Undo list to undo all of the SOLIDWORKS API calls that created the gear.

NOTE: Only SOLIDWORKS operations that support Undo will be undone. Both SOLIDWORKS API and non-API operations are undone.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

[IModelDoc2::ClearUndoList Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ClearUndoList.html)

[IModelDoc2::EditUndo2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~EditUndo2.html)

[IModelDoc2::EditRedo2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~EditRedo2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0