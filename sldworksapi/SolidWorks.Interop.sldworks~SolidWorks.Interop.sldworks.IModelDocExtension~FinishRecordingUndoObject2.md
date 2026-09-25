<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~FinishRecordingUndoObject2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| FinishRecordingUndoObject2 Method (IModelDocExtension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : FinishRecordingUndoObject2 Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*UndoObjectName*
:   String that appears in the SOLIDWORKS Undo list

*MakeHidden*
:   True to hide this object in the Undo list and from the user; false to make this object visible in the Undo list and to the user

Ends recording of a SOLIDWORKS Undo object with the specified name and visibility.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function FinishRecordingUndoObject2( _    ByVal UndoObjectName As System.String, _    ByVal MakeHidden As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim UndoObjectName As System.String Dim MakeHidden As System.Boolean Dim value As System.Boolean   value = instance.FinishRecordingUndoObject2(UndoObjectName, MakeHidden) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool FinishRecordingUndoObject2(     System.string UndoObjectName,    System.bool MakeHidden ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool FinishRecordingUndoObject2(  &   System.String^ UndoObjectName, &   System.bool MakeHidden ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*UndoObjectName*
:   String that appears in the SOLIDWORKS Undo list

*MakeHidden*
:   True to hide this object in the Undo list and from the user; false to make this object visible in the Undo list and to the user

#### Return Value

True if recording of the SOLIDWORKS Undo object ends, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::FinishRecordingUndoObject2.

# ![](dotnetimages/collapse.gif)Example

[Create Hidden Undo Object (VBA)](Create_Multiple_Undo_Command_Example_VB.htm)

[Create Hidden Undo Object (VB.NET)](Create_Multiple_Undo_Command_Example_VBNET.htm)

[Create Hidden Undo Object (C#)](Create_Multiple_Undo_Command_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

To add an object with the name UndoObjectName to the SOLIDWORKS Undo list, place the SOLIDWORKS API calls between [IModelDocExtension::StartRecordingUndoObject](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~StartRecordingUndoObject.html) and IModelDocExtension::FinishRecordingUndoObject2:

For example, assume that your application creates a complex gear that requires many SOLIDWORKS API calls and you would like your SOLIDWORKS user to be able to undo that gear from the user interface at a later time. Your application can create an Undo object by calling:

1. IModelDocExtension::StartRecordingUndoObject

   - SOLIDWORKS API calls that create the gear

     - IModelDocExtension::FinishRecordingUndoObject2 with MakeHidden = False

Now assume that your application performs many temporary operations that you do not want your users to see in the SOLIDWORKS Undo list, because they are not essential to the modeling and design process. For this case, your application can place the non-essential SOLIDWORKS API calls between IModelDocExtension::StartRecordingUndoObject and IModelDocExtension::FinishRecordingUndoObject2 with MakeHidden = True. The Undo object is still added to the SOLIDWORKS Undo list, but the user does not see it in the list.

****WARNING**:** If your application hides an Undo object in the Undo list by setting MakeHidden = True and the Undo object is the first item in the SOLIDWORKS Undo list, then SOLIDWORKS discards the Undo object from the Undo list. If this happens, then the SOLIDWORKS API calls in this Undo object cannot be undone.

Similarly if the last item to be redone is a hidden API Undo object, then SOLIDWORKS discards it and the SOLIDWORKS API calls cannot be redone.

Only SOLIDWORKS operations that support Undo are undone. Both SOLIDWORKS API and non-API operations are undone.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

[IModelDoc2::ClearUndoList Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ClearUndoList.html)

[IModelDoc2::EditUndo2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~EditUndo2.html)

[IModelDoc2::EditRedo2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~EditRedo2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2013 FCS, Revision Number 21.0