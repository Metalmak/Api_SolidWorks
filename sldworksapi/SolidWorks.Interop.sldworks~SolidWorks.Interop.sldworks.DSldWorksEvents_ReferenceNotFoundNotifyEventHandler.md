<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DSldWorksEvents_ReferenceNotFoundNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DSldWorksEvents\_ReferenceNotFoundNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : DSldWorksEvents\_ReferenceNotFoundNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FileName*
:   Path and filename of the referenced file

Notifies the user program before the SOLIDWORKS software displays a dialog box prompting the end-user to browse for the referenced file.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DSldWorksEvents_ReferenceNotFoundNotifyEventHandler( _    ByVal FileName As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DSldWorksEvents_ReferenceNotFoundNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DSldWorksEvents_ReferenceNotFoundNotifyEventHandler(     System.string FileName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DSldWorksEvents_ReferenceNotFoundNotifyEventHandler(  &   System.String^ FileName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FileName*
:   Path and filename of the referenced file

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ReferenceNotFoundNotify Event (SldWorks).

# ![](dotnetimages/collapse.gif)Example

This code illustrates the proper use of this event:

HRESULT swAppEvents::AppReferenceNotFoundNotify (BSTR FileName)

{

static bool test = true;

TRACE( \_T(" TestbedEvents - SldWorks.swAppReferenceNotFoundNotify event fired\n"));

if( test)

{

LPSLDWORKS pSldWorks = NULL;

m\_lpObject->QueryInterface(IID\_ISldWorks, (void\*\*)&pSldWorks);

pSldWorks->SetMissingReferencePathName( FileName);

pSldWorks->Release();

return S\_false;

}

else

return S\_OK;

}

# ![](dotnetimages/collapse.gif)Remarks

Use this event with [ISldWorks::SetMissingReferencePathName](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~SetMissingReferencePathName.html). Returning S\_false from your event handler successfully replaces the specified fileName with the filename specified in the call to ISldWorks::SetMissingReferencePathName.

This event is generated when a document is opened and one of its dependencies is not found.

If developing a C++ application, use swAppReferenceNotFoundNotify to register for this notification.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0