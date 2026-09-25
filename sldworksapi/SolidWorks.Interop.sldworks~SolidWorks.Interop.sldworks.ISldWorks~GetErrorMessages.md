<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetErrorMessages.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetErrorMessages Method (ISldWorks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : GetErrorMessages Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Msgs*
:   Array of the last 20 messages issued by SOLIDWORKS in this SOLIDWORKS session

*MsgIDs*
:   Array of the resource IDs of the last 20  messages issued by SOLIDWORKS in this SOLIDWORKS
    session

*MsgTypes*
:   Array of the types of the last 20 messages issued by SOLIDWORKS in this SOLIDWORKS
    session (see Remarks)

Gets the last 20 messages issued by SOLIDWORKS in the current SOLIDWORKS session.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetErrorMessages( _    ByRef Msgs As System.Object, _    ByRef MsgIDs As System.Object, _    ByRef MsgTypes As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim Msgs As System.Object Dim MsgIDs As System.Object Dim MsgTypes As System.Object Dim value As System.Integer   value = instance.GetErrorMessages(Msgs, MsgIDs, MsgTypes) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetErrorMessages(     out System.object Msgs,    out System.object MsgIDs,    out System.object MsgTypes ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetErrorMessages(  &   [Out] System.Object^ Msgs, &   [Out] System.Object^ MsgIDs, &   [Out] System.Object^ MsgTypes ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Msgs*
:   Array of the last 20 messages issued by SOLIDWORKS in this SOLIDWORKS session

*MsgIDs*
:   Array of the resource IDs of the last 20  messages issued by SOLIDWORKS in this SOLIDWORKS
    session

*MsgTypes*
:   Array of the types of the last 20 messages issued by SOLIDWORKS in this SOLIDWORKS
    session (see Remarks)

#### Return Value

Number of messages issued by SOLIDWORKS in this SOLIDWORKS session

**NOTE:**The stack is cleared after calling this method.

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::GetErrorMessages.

# ![](dotnetimages/collapse.gif)Example

[Get Messages (VBA)](Get_Messages_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

The elements of the MsgTypes array are bitmasks of the Microsoft message-box system constants.

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[ISldWorks::GetLastSaveError Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetLastSaveError.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 SP1, Revision Number 14.1