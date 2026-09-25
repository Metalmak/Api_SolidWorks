<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DDrawingDocEvents_ChangeCustomPropertyNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DDrawingDocEvents\_ChangeCustomPropertyNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : DDrawingDocEvents\_ChangeCustomPropertyNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*propName*
:   Name of the changed property

*Configuration*
:   Configuration that contains the property

*oldValue*
:   Previous value of the property

*NewValue*
:   New value of the property

*valueType*
:   Valid type for VARIANT; see Microsoft MSDN for a list of the valid VARIANT types

Post-notifies the user program when the user has changed a custom property.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DDrawingDocEvents_ChangeCustomPropertyNotifyEventHandler( _    ByVal propName As System.String, _    ByVal Configuration As System.String, _    ByVal oldValue As System.String, _    ByVal NewValue As System.String, _    ByVal valueType As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DDrawingDocEvents_ChangeCustomPropertyNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DDrawingDocEvents_ChangeCustomPropertyNotifyEventHandler(     System.string propName,    System.string Configuration,    System.string oldValue,    System.string NewValue,    System.int valueType ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DDrawingDocEvents_ChangeCustomPropertyNotifyEventHandler(  &   System.String^ propName, &   System.String^ Configuration, &   System.String^ oldValue, &   System.String^ NewValue, &   System.int valueType ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*propName*
:   Name of the changed property

*Configuration*
:   Configuration that contains the property

*oldValue*
:   Previous value of the property

*NewValue*
:   New value of the property

*valueType*
:   Valid type for VARIANT; see Microsoft MSDN for a list of the valid VARIANT types

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ChangeCustomPropertyNotify Event (DrawingDoc).

# ![](dotnetimages/collapse.gif)Remarks

The ValueType argument is one of the valid types that VARIANT can contain.

If developing a C++ application, use swDrawingChangeCustomPropertyNotify to register for this notification.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus SP1, Revision Number 10.1