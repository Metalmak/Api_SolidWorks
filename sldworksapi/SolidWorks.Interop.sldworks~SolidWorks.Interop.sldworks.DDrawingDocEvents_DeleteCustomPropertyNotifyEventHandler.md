<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DDrawingDocEvents_DeleteCustomPropertyNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DDrawingDocEvents\_DeleteCustomPropertyNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : DDrawingDocEvents\_DeleteCustomPropertyNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*propName*
:   Name of the deleted property

*Configuration*
:   Cofniguration that contains the property

*Value*
:   Value of the deleted property

*valueType*
:   Valid type for VARIANT; see Microsoft MSDN for a list of valid VARIANT types

Post-notifies the user program when the user deletes a custom property.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DDrawingDocEvents_DeleteCustomPropertyNotifyEventHandler( _    ByVal propName As System.String, _    ByVal Configuration As System.String, _    ByVal Value As System.String, _    ByVal valueType As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DDrawingDocEvents_DeleteCustomPropertyNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DDrawingDocEvents_DeleteCustomPropertyNotifyEventHandler(     System.string propName,    System.string Configuration,    System.string Value,    System.int valueType ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DDrawingDocEvents_DeleteCustomPropertyNotifyEventHandler(  &   System.String^ propName, &   System.String^ Configuration, &   System.String^ Value, &   System.int valueType ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*propName*
:   Name of the deleted property

*Configuration*
:   Cofniguration that contains the property

*Value*
:   Value of the deleted property

*valueType*
:   Valid type for VARIANT; see Microsoft MSDN for a list of valid VARIANT types

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DeleteCustomPropertyNotify Event (DrawingDoc).

# ![](dotnetimages/collapse.gif)Remarks

The ValueType argument is one of the valid types that VARIANT can contain.

If developing a C++ application, use swDrawingDeleteCustomPropertyNotify to register for this notification.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus SP1, Revision Number 10.1