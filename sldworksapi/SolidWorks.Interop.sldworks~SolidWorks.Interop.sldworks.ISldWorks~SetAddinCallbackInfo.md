<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~SetAddinCallbackInfo.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetAddinCallbackInfo Method (ISldWorks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : SetAddinCallbackInfo Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ModuleHandle*
:   Instance handle of the add-in

*AddinCallbacks*
:   Object that includes the add-in callback methods

*Cookie*
:   Add-in ID; this is the same Cookie you specified in ISwAddin::ConnectToSW

Obsolete. Superseded by [ISldWorks::SetAddinCallbackInfo2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~SetAddinCallbackInfo2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetAddinCallbackInfo( _    ByVal ModuleHandle As System.Integer, _    ByVal AddinCallbacks As System.Object, _    ByVal Cookie As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim ModuleHandle As System.Integer Dim AddinCallbacks As System.Object Dim Cookie As System.Integer Dim value As System.Boolean   value = instance.SetAddinCallbackInfo(ModuleHandle, AddinCallbacks, Cookie) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetAddinCallbackInfo(     System.int ModuleHandle,    System.object AddinCallbacks,    System.int Cookie ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetAddinCallbackInfo(  &   System.int ModuleHandle, &   System.Object^ AddinCallbacks, &   System.int Cookie ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ModuleHandle*
:   Instance handle of the add-in

*AddinCallbacks*
:   Object that includes the add-in callback methods

*Cookie*
:   Add-in ID; this is the same Cookie you specified in ISwAddin::ConnectToSW

#### Return Value

True if the add-in callback commands are set, false if if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::SetAddinCallbackInfo.

# ![](dotnetimages/collapse.gif)Example

'-----------------------------------------

' Module-level variables

Dim iSldWorks                   As SldWorks.SldWorks

Dim iCookie                     As Long

'-----------------------------------------

'Implementation methods of the SwAddin interface

Private Function SwAddin\_ConnectToSW(ByVal ThisSW As Object, ByVal Cookie As Long) As Boolean

    Dim bRet                As Boolean

    ' Store reference to SOLIDWORKS session

    Set iSldWorks = ThisSW

    ' Store cookie from SOLIDWORKS

    iCookie = Cookie

    'Inform SOLIDWORKS about the object that contains the callbacks

    bRet = iSldWorks.SetAddinCallbackInfo(App.hInstance, Me, iCookie)

    ...

    SwAddin\_ConnectToSW = True

End Function

'-----------------------------------------

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[ISldWorks::AddCallback Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~AddCallback.html)

[ISldWorks::CallBack Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~CallBack.html)

[ISldWorks::RemoveCallback Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~RemoveCallback.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0