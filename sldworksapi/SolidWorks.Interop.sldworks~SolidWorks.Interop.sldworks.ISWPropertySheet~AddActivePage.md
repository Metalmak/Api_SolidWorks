<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISWPropertySheet~AddActivePage.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddActivePage Method (ISWPropertySheet) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISWPropertySheet Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISWPropertySheet.html) : AddActivePage Method (ISWPropertySheet) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Title*
:   Title of CPropertyPage

*ProgId*
:   Name, ProgID, or CLSID of the ActiveX control (see Remarks)

*LicenseKey*
:   License key for the ActiveX control

Adds a third-party CPropertyPage to [ISWPropertySheet](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISWPropertySheet.html) and adds an ActiveX control on top of the page.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddActivePage( _    ByVal Title As System.String, _    ByVal ProgId As System.String, _    ByVal LicenseKey As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISWPropertySheet Dim Title As System.String Dim ProgId As System.String Dim LicenseKey As System.String Dim value As System.Integer   value = instance.AddActivePage(Title, ProgId, LicenseKey) ``` | |

| C# |  |
| --- | --- |
| ``` System.int AddActivePage(     System.string Title,    System.string ProgId,    System.string LicenseKey ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int AddActivePage(  &   System.String^ Title, &   System.String^ ProgId, &   System.String^ LicenseKey ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Title*
:   Title of CPropertyPage

*ProgId*
:   Name, ProgID, or CLSID of the ActiveX control (see Remarks)

*LicenseKey*
:   License key for the ActiveX control

#### Return Value

Index of CPropertyPage on ISWPropertySheet

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SWPropertySheet::AddActivePage.

# ![](dotnetimages/collapse.gif)Example

```
'VBA Main module
```

```
Dim swApp As SldWorks.SldWorks
Option Explicit
Sub main()
    UserForm1.Show (swModeLess)
End Sub
```

```
'Insert UserForm module to VBA application
```

```
Option Explicit
```

```
Public WithEvents swAppEvents As SldWorks.SldWorks
Dim swApp As SldWorks.SldWorks
```

```
Private Function swAppEvents_PropertySheetCreateNotify(ByVal Sheet As Object, ByVal sheetType As Long) As Long
    Dim msrcSWPropertySheet As SWPropertySheet
    Set msrcSWPropertySheet = Sheet
    Call msrcSWPropertySheet.AddActivePage("PropertySheetExample2", "", "")
End Function
```

```
Private Sub UserForm_Initialize()
    Set swApp = Application.SldWorks
    Set swAppEvents = swApp
End Sub
```

# ![](dotnetimages/collapse.gif)Remarks

Typically, this method is called from the ISldWorks [PropertySheetCreateNotify](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.DSldWorksEvents_PropertySheetCreateNotifyEventHandler.html) event handler. See the Example section.

The ProgID argument accepts any of these values:

* OLE short name  or ProgID for the class; for example, "MSCAL.Calendar".  The name must match the name registered by the control.

* String form of a CLSID, contained within braces, for example, "{9DBAFCCF-592F-101B-85CE-00608CEC297B}".

See also Keystrokes and Accelerator Keys in ActiveX Modeless Dialogs and PropertyManager Pages.

# ![](dotnetimages/collapse.gif)See Also

####

[ISWPropertySheet Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISWPropertySheet.html)

[ISWPropertySheet Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISWPropertySheet_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 SP4, Revision Number 12.4