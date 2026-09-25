<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRoutingSettings~GetFromToListHeaderDefinitions.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetFromToListHeaderDefinitions Method (IRoutingSettings) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IRoutingSettings Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRoutingSettings.html) : GetFromToListHeaderDefinitions Method (IRoutingSettings) |

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

Gets the headers from a routing from-to list.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetFromToListHeaderDefinitions( _    ByRef WireNameHdr As System.String, _    ByRef FromRefHdr As System.String, _    ByRef FromPinHdr As System.String, _    ByRef FromPartnoHdr As System.String, _    ByRef ToRefHdr As System.String, _    ByRef ToPinHdr As System.String, _    ByRef ToPartnoHdr As System.String, _    ByRef CableNameHdr As System.String, _    ByRef CoreNameHdr As System.String, _    ByRef ColourHdr As System.String, _    ByRef WireSpecHdr As System.String, _    ByRef OtherAttribHdr As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IRoutingSettings Dim WireNameHdr As System.String Dim FromRefHdr As System.String Dim FromPinHdr As System.String Dim FromPartnoHdr As System.String Dim ToRefHdr As System.String Dim ToPinHdr As System.String Dim ToPartnoHdr As System.String Dim CableNameHdr As System.String Dim CoreNameHdr As System.String Dim ColourHdr As System.String Dim WireSpecHdr As System.String Dim OtherAttribHdr As System.String Dim value As System.Boolean   value = instance.GetFromToListHeaderDefinitions(WireNameHdr, FromRefHdr, FromPinHdr, FromPartnoHdr, ToRefHdr, ToPinHdr, ToPartnoHdr, CableNameHdr, CoreNameHdr, ColourHdr, WireSpecHdr, OtherAttribHdr) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetFromToListHeaderDefinitions(     out System.string WireNameHdr,    out System.string FromRefHdr,    out System.string FromPinHdr,    out System.string FromPartnoHdr,    out System.string ToRefHdr,    out System.string ToPinHdr,    out System.string ToPartnoHdr,    out System.string CableNameHdr,    out System.string CoreNameHdr,    out System.string ColourHdr,    out System.string WireSpecHdr,    out System.string OtherAttribHdr ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetFromToListHeaderDefinitions(  &   [Out] System.String^ WireNameHdr, &   [Out] System.String^ FromRefHdr, &   [Out] System.String^ FromPinHdr, &   [Out] System.String^ FromPartnoHdr, &   [Out] System.String^ ToRefHdr, &   [Out] System.String^ ToPinHdr, &   [Out] System.String^ ToPartnoHdr, &   [Out] System.String^ CableNameHdr, &   [Out] System.String^ CoreNameHdr, &   [Out] System.String^ ColourHdr, &   [Out] System.String^ WireSpecHdr, &   [Out] System.String^ OtherAttribHdr ) ``` | |

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

See RoutingSettings::GetFromToListHeaderDefinitions.

# ![](dotnetimages/collapse.gif)Example

See the [IRoutingSettings](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRoutingSettings.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[IRoutingSettings Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRoutingSettings.html)

[IRoutingSettings Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRoutingSettings_members.html)

[IRoutingSettings::SetFromToListHeaderDefinitions Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRoutingSettings~SetFromToListHeaderDefinitions.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0