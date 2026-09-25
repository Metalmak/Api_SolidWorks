<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFaultEntity~ErrorCode.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ErrorCode Property (IFaultEntity) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFaultEntity Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFaultEntity.html) : ErrorCode Property (IFaultEntity) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Index*
:   0-based index number indicating the entity with the fault

Gets the error for the fault for the specified entity.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` ReadOnly Property ErrorCode( _    ByVal Index As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFaultEntity Dim Index As System.Integer Dim value As System.Integer   value = instance.ErrorCode(Index) ``` | |

| C# |  |
| --- | --- |
| ``` System.int ErrorCode(     System.int Index ) {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int ErrorCode {    System.int get(System.int Index); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Index*
:   0-based index number indicating the entity with the fault

#### Property Value

Error as defined by swFaultEntityErrorCode\_e; -1 indicates an unknown error

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FaultEntity::ErrorCode.

# ![](dotnetimages/collapse.gif)Example

[Check Bodies for Faults (VBA)](Check_Bodies_for_Faults_Example_VB.htm)

[Check Faces for Faults (VBA)](Check_Faces_for_Faults_Example_VB.htm)

[Check Edges for Faults (C#)](Check_Edges_for_Faults_Example_CSharp.htm)

[Check Edges for Faults (VB.NET)](Check_Edges_for_Faults_Example_VBNET.htm)

[Check Edges for Faults (VBA)](Check_Edges_for_Faults_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

To determine the value for index, call [IFaultEntity::Count](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFaultEntity~Count.html) before calling this property. Call [IFaultEntity::Entity2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFaultEntity~Entity2.html) to get the entity.

# ![](dotnetimages/collapse.gif)See Also

####

[IFaultEntity Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFaultEntity.html)

[IFaultEntity Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFaultEntity_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 SP4, Revision Number 12.4