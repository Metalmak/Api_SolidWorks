<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DMouseEvents_MouseNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DMouseEvents\_MouseNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : DMouseEvents\_MouseNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Message*
:   Message to be sent

*WParam*
:   Additional message\_dependent information

*LParam*
:   X, Y in a packed long requiring unpacking; see GET\_X\_LPARAM and GET\_Y\_LPARAM in MSDN for details on how to unpack LParam

Fired whenever a mouse event occurs.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DMouseEvents_MouseNotifyEventHandler( _    ByVal Message As System.Integer, _    ByVal WParam As System.Integer, _    ByVal LParam As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DMouseEvents_MouseNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DMouseEvents_MouseNotifyEventHandler(     System.int Message,    System.int WParam,    System.int LParam ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DMouseEvents_MouseNotifyEventHandler(  &   System.int Message, &   System.int WParam, &   System.int LParam ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Message*
:   Message to be sent

*WParam*
:   Additional message\_dependent information

*LParam*
:   X, Y in a packed long requiring unpacking; see GET\_X\_LPARAM and GET\_Y\_LPARAM in MSDN for details on how to unpack LParam

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See MouseNotify Event (Mouse).

# ![](dotnetimages/collapse.gif)Example

The following sample code shows a possible approach to decoding WParam and LParam.

'--------------------------------------------------------------

void NotifyHandler( UINT message, WPARAM wParam, LPARAM lParam)

{

long x = GET\_X\_LPARAM(lParam);//Uses Windows macro

long y = GET\_Y\_LPARAM(lParam);//Uses Windows macro

switch(message)

{

case WM\_MOUSEWHEEL:

case WM\_MOUSEMOVE:

//Your code to process event

break;

case WM\_LBUTTONDOWN:

//Your code to process event

break;

case WM\_LBUTTONUP:

//Your code to process event

break;

case WM\_RBUTTONDOWN:

//Your code to process event

break;

case WM\_RBUTTONUP:

//Your code to process event

break;

case WM\_MBUTTONDOWN:

//Your code to process event

break;

case WM\_MBUTTONUP:

//Your code to process event

break;

case WM\_LBUTTONDBLCLK:

//Your code to process event

break;

case WM\_RBUTTONDBLCLK:

//Your code to process event

break;

case WM\_MBUTTONDBLCLK:

//Your code to process event

break;

}

}

# ![](dotnetimages/collapse.gif)Remarks

If developing a C++ application, use swMouseNotify to register for this notification.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0