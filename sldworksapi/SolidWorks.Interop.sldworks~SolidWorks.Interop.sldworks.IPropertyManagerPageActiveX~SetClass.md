<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageActiveX~SetClass.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetClass Method (IPropertyManagerPageActiveX) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPropertyManagerPageActiveX Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageActiveX.html) : SetClass Method (IPropertyManagerPageActiveX) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ClassID*
:   Class ID for the control

*LicenseKey*
:   License key for the control

Sets the interface to this ActiveX control.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetClass( _    ByVal ClassID As System.String, _    ByVal LicenseKey As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPropertyManagerPageActiveX Dim ClassID As System.String Dim LicenseKey As System.String Dim value As System.Boolean   value = instance.SetClass(ClassID, LicenseKey) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetClass(     System.string ClassID,    System.string LicenseKey ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetClass(  &   System.String^ ClassID, &   System.String^ LicenseKey ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ClassID*
:   Class ID for the control

*LicenseKey*
:   License key for the control

#### Return Value

Always returns true

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PropertyManagerPageActiveX::SetClass.

# ![](dotnetimages/collapse.gif)Example

See the [IPropertyManagerPageActiveX](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageActiveX.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

This method sets the class ID and license key information for the ActiveX control when a PropertyManager page created using the API is shown and the ActiveX control is created. ClassId can be either the name of the control (ProgID) or the class ID (CLSID), for example, "MSCAL.calendar" or "{8E27C92B-1264-101C-8A2F-040224009C02}". Both provide the calendar protocol. You can obtain these strings using a combination of the Microsoft OLE/COM Object Viewer and the registry editor.

VBA example:

' ProgID

bRet = m\_pActiveXControl.SetClass("MSCAL.Calendar", "")

bRet = m\_pActiveXControl2.SetClass("MSComctlLib.ListViewCtrl", "")

' CLSID

bRet = m\_pActiveXControl.SetClass("{8E27C92B-1264-101C-8A2F-040224009C02}", "")

bRet = m\_pActiveXControl2.SetClass("{BDD1F04B-858B-11D1-B16A-00C0F0283628}", "")

This method does not check to determine if the creation of the control worked. Instead, the IPropertyManagerPage2Handler5::OnActiveXControlCreated sends notification when an attempt to create the ActiveX control occurs, regardless if it is created or not. Use the IPropertyManagerPage2Handler5::OnActiveXControlCreated method's return value to indicate what action to take if the creation of the control failed.

# ![](dotnetimages/collapse.gif)See Also

####

[IPropertyManagerPageActiveX Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageActiveX.html)

[IPropertyManagerPageActiveX Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageActiveX_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2003 FCS, Revision Number 11.0