<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DPartDocEvents_InsertTableNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DPartDocEvents\_InsertTableNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : DPartDocEvents\_InsertTableNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) |

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

*TemplatePath*
:   Full path of template used to create this table

Notifies your program when a table has been inserted in a part.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DPartDocEvents_InsertTableNotifyEventHandler( _    ByVal TableAnnotation As TableAnnotation, _    ByVal TableType As System.Integer, _    ByVal TemplatePath As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DPartDocEvents_InsertTableNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DPartDocEvents_InsertTableNotifyEventHandler(     TableAnnotation TableAnnotation,    System.int TableType,    System.string TemplatePath ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DPartDocEvents_InsertTableNotifyEventHandler(  &   TableAnnotation^ TableAnnotation, &   System.int TableType, &   System.String^ TemplatePath ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*TableAnnotation*
:   [ITableAnnotation](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ITableAnnotation.html)

*TableType*
:   Type of table as defined in swTableAnnotationType\_e

*TemplatePath*
:   Full path of template used to create this table

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See InsertTableNotify Event (PartDoc).

# ![](dotnetimages/collapse.gif)Example

[Fire Notification When Inserting a Table in a Part Document (C#)](Fire_Notification_When_Inserting_a_Table_in_a_Part_Document_Example_CSharp.htm)

[Fire Notification When Inserting a Table in a Part Document (VB.NET)](Fire_Notification_When_Inserting_a_Table_in_a_Part_Document_Example_VBNET.htm)

[Fire Notification When Inserting a Table in a Part Document (VBA)](Fire_Notification_When_Inserting_a_Table_in_a_Part_Document_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

If developing a C++ application, use swPartInsertTableNotify to register for this notification.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0