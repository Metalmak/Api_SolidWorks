<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRoutingSettings~SetFromToListHeaderDefinitions.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetFromToListHeaderDefinitions Method (IRoutingSettings) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IRoutingSettings Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRoutingSettings.html) : SetFromToListHeaderDefinitions Method (IRoutingSettings) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*WireNameHdr*
:   Wire name header

*FromRefHdr*
:   "From" reference header

*FromPinHdr*
:   "From" pin header

*FromPartnoHdr*
:   "From" part number header

*ToRefHdr*
:   "To" reference header

*ToPinHdr*
:   "To" pin header

*ToPartnoHdr*
:   "To" part number header

*CableNameHdr*
:   Cable name header

*CoreNameHdr*
:   Core name header

*ColourHdr*
:   Color header

*WireSpecHdr*
:   Wire specification header

*OtherAttribHdr*
:   Miscellaneous header

Sets the headers in a routing from-to list.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetFromToListHeaderDefinitions( _    ByVal WireNameHdr As System.String, _    ByVal FromRefHdr As System.String, _    ByVal FromPinHdr As System.String, _    ByVal FromPartnoHdr As System.String, _    ByVal ToRefHdr As System.String, _    ByVal ToPinHdr As System.String, _    ByVal ToPartnoHdr As System.String, _    ByVal CableNameHdr As System.String, _    ByVal CoreNameHdr As System.String, _    ByVal ColourHdr As System.String, _    ByVal WireSpecHdr As System.String, _    ByVal OtherAttribHdr As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IRoutingSettings Dim WireNameHdr As System.String Dim FromRefHdr As System.String Dim FromPinHdr As System.String Dim FromPartnoHdr As System.String Dim ToRefHdr As System.String Dim ToPinHdr As System.String Dim ToPartnoHdr As System.String Dim CableNameHdr As System.String Dim CoreNameHdr As System.String Dim ColourHdr As System.String Dim WireSpecHdr As System.String Dim OtherAttribHdr As System.String Dim value As System.Boolean   value = instance.SetFromToListHeaderDefinitions(WireNameHdr, FromRefHdr, FromPinHdr, FromPartnoHdr, ToRefHdr, ToPinHdr, ToPartnoHdr, CableNameHdr, CoreNameHdr, ColourHdr, WireSpecHdr, OtherAttribHdr) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetFromToListHeaderDefinitions(     System.string WireNameHdr,    System.string FromRefHdr,    System.string FromPinHdr,    System.string FromPartnoHdr,    System.string ToRefHdr,    System.string ToPinHdr,    System.string ToPartnoHdr,    System.string CableNameHdr,    System.string CoreNameHdr,    System.string ColourHdr,    System.string WireSpecHdr,    System.string OtherAttribHdr ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetFromToListHeaderDefinitions(  &   System.String^ WireNameHdr, &   System.String^ FromRefHdr, &   System.String^ FromPinHdr, &   System.String^ FromPartnoHdr, &   System.String^ ToRefHdr, &   System.String^ ToPinHdr, &   System.String^ ToPartnoHdr, &   System.String^ CableNameHdr, &   System.String^ CoreNameHdr, &   System.String^ ColourHdr, &   System.String^ WireSpecHdr, &   System.String^ OtherAttribHdr ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*WireNameHdr*
:   Wire name header

*FromRefHdr*
:   "From" reference header

*FromPinHdr*
:   "From" pin header

*FromPartnoHdr*
:   "From" part number header

*ToRefHdr*
:   "To" reference header

*ToPinHdr*
:   "To" pin header

*ToPartnoHdr*
:   "To" part number header

*CableNameHdr*
:   Cable name header

*CoreNameHdr*
:   Core name header

*ColourHdr*
:   Color header

*WireSpecHdr*
:   Wire specification header

*OtherAttribHdr*
:   Miscellaneous header

#### Return Value

True if successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See RoutingSettings::SetFromToListHeaderDefinitions.

# ![](dotnetimages/collapse.gif)See Also

####

[IRoutingSettings Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRoutingSettings.html)

[IRoutingSettings Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRoutingSettings_members.html)

[IRoutingSettings::GetFromToListHeaderDefinitions Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRoutingSettings~GetFromToListHeaderDefinitions.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0