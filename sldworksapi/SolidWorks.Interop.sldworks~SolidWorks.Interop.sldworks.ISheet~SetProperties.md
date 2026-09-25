<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet~SetProperties.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetProperties Method (ISheet) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISheet Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet.html) : SetProperties Method (ISheet) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*PaperSz*
:   Paper size as defined in swDwgPaperSizes\_e

*Templ*
:   Template as defined in swDwgTemplates\_e

*Scale1*
:   Scale numerator

*Scale2*
:   Scale denominator

*FirstAngle*
:   True if you want first angle projection, false if not

*Width*
:   Custom paper width if PaperSz = swDwgPaperSizes\_e.swDwgPapersUserDefined

*Height*
:   Custom paper height if PaperSz = swDwgPaperSizes\_e.swDwgPapersUserDefined

Obsolete. Superseded by [ISheet::SetProperties2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet~SetProperties2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetProperties( _    ByVal PaperSz As System.Integer, _    ByVal Templ As System.Integer, _    ByVal Scale1 As System.Double, _    ByVal Scale2 As System.Double, _    ByVal FirstAngle As System.Boolean, _    ByVal Width As System.Double, _    ByVal Height As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISheet Dim PaperSz As System.Integer Dim Templ As System.Integer Dim Scale1 As System.Double Dim Scale2 As System.Double Dim FirstAngle As System.Boolean Dim Width As System.Double Dim Height As System.Double   instance.SetProperties(PaperSz, Templ, Scale1, Scale2, FirstAngle, Width, Height) ``` | |

| C# |  |
| --- | --- |
| ``` void SetProperties(     System.int PaperSz,    System.int Templ,    System.double Scale1,    System.double Scale2,    System.bool FirstAngle,    System.double Width,    System.double Height ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetProperties(  &   System.int PaperSz, &   System.int Templ, &   System.double Scale1, &   System.double Scale2, &   System.bool FirstAngle, &   System.double Width, &   System.double Height ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*PaperSz*
:   Paper size as defined in swDwgPaperSizes\_e

*Templ*
:   Template as defined in swDwgTemplates\_e

*Scale1*
:   Scale numerator

*Scale2*
:   Scale denominator

*FirstAngle*
:   True if you want first angle projection, false if not

*Width*
:   Custom paper width if PaperSz = swDwgPaperSizes\_e.swDwgPapersUserDefined

*Height*
:   Custom paper height if PaperSz = swDwgPaperSizes\_e.swDwgPapersUserDefined

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Sheet::SetProperties.

# ![](dotnetimages/collapse.gif)Remarks

If you specify a custom template, then the current custom template is used by this sheet until you call [ISheet::SetTemplateName](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISheet~SetTemplateName.html) and pass in a different custom template name.

NOTE: If Templ does not match the PaperSz specification, then you get a template that does not fit the paper size. This parameter does not override the PaperSz setting. Also, if you change the scale of the sheet using Scale1 and Scale2, then any drawing view that is set to use the sheet's scale takes the new scale setting.

You can also use [ISheet::SetSize](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISheet~SetSize.html) to set the size of the sheet and the standard sheet size.

# ![](dotnetimages/collapse.gif)See Also

####

[ISheet Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet.html)

[ISheet Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet_members.html)

[ISheet::GetProperties Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet~GetProperties.html)

[ISheet::IGetProperties Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet~IGetProperties.html)

[ISheet::GetSize Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet~GetSize.html)

[ISheet::GetTemplateName Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet~GetTemplateName.html)

[ISheet::IPageSetup Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet~IPageSetup.html)

[ISheet::PageSetup Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet~PageSetup.html)

[ISheet::SetTemplateName Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet~SetTemplateName.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0