<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DDrawingDocEvents_ModifyTableNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DDrawingDocEvents\_ModifyTableNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : DDrawingDocEvents\_ModifyTableNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*TableAnnotation*
:   [ITableAnnotation](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ITableAnnotation.html)

*TableType*
:   Type of table as defined in swTableAnnotationType\_e

*reason*
:   Reason as defined in swModifyTableNotifyReason\_e

*RowInfo*
:   Index of modified row

*ColumnInfo*
:   Index of modified column

*DataInfo*
:   Modified string

Notifies your program when a table has been modified in a drawing.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DDrawingDocEvents_ModifyTableNotifyEventHandler( _    ByVal TableAnnotation As TableAnnotation, _    ByVal TableType As System.Integer, _    ByVal reason As System.Integer, _    ByVal RowInfo As System.Integer, _    ByVal ColumnInfo As System.Integer, _    ByVal DataInfo As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DDrawingDocEvents_ModifyTableNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DDrawingDocEvents_ModifyTableNotifyEventHandler(     TableAnnotation TableAnnotation,    System.int TableType,    System.int reason,    System.int RowInfo,    System.int ColumnInfo,    System.string DataInfo ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DDrawingDocEvents_ModifyTableNotifyEventHandler(  &   TableAnnotation^ TableAnnotation, &   System.int TableType, &   System.int reason, &   System.int RowInfo, &   System.int ColumnInfo, &   System.String^ DataInfo ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*TableAnnotation*
:   [ITableAnnotation](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ITableAnnotation.html)

*TableType*
:   Type of table as defined in swTableAnnotationType\_e

*reason*
:   Reason as defined in swModifyTableNotifyReason\_e

*RowInfo*
:   Index of modified row

*ColumnInfo*
:   Index of modified column

*DataInfo*
:   Modified string

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModifyTableNotify Event (DrawingDoc).

# ![](dotnetimages/collapse.gif)Example

[Fire Notification When Changing a Table in a Drawing Document (C#)](Fire_Notification_When_Changing_a_Table_in_a_Drawing_Document_Example_CSharp.htm)

[Fire Notification When Changing a Table in a Drawing Document (VB.NET)](Fire_Notification_When_Changing_a_Table_in_a_Drawing_Document_Example_VBNET.htm)

[Fire Notification When Changing a Table in a Drawing Document (VBA)](Fire_Notification_When_Changing_a_Table_in_a_Drawing_Document_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

If developing a C++ application, use swDrawingModifyTableNotify to register for this notification.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0