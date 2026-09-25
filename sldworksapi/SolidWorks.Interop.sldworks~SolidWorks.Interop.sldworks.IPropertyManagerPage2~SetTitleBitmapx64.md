<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPage2~SetTitleBitmapx64.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetTitleBitmapx64 Method (IPropertyManagerPage2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPropertyManagerPage2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPage2.html) : SetTitleBitmapx64 Method (IPropertyManagerPage2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ModuleHandle*
:   Module handle of the application instance that contains the bitmap resource (see **Remarks**)

*Identifier*
:   Resource ID of the bitmap (see **Remarks**)

Sets the bitmap to display in the title of this PropertyManager page.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetTitleBitmapx64( _    ByVal ModuleHandle As System.Long, _    ByVal Identifier As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPropertyManagerPage2 Dim ModuleHandle As System.Long Dim Identifier As System.Integer Dim value As System.Boolean   value = instance.SetTitleBitmapx64(ModuleHandle, Identifier) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetTitleBitmapx64(     System.long ModuleHandle,    System.int Identifier ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetTitleBitmapx64(  &   System.int64 ModuleHandle, &   System.int Identifier ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ModuleHandle*
:   Module handle of the application instance that contains the bitmap resource (see **Remarks**)

*Identifier*
:   Resource ID of the bitmap (see **Remarks**)

#### Return Value

True if successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PropertyManagerPage2::SetTitleBitmapx64.

# ![](dotnetimages/collapse.gif)Remarks

This method is only available through early binding and with 64-bit versions of the SOLIDWORKS software. Its intended use is for SOLIDWORKS PropertyManager .NET add-ins. For VBA PropertyManager pages, use [IPropertyManagerPage2::SetTitleBitmap2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPage2~SetTitleBitmap2.html).

You can only use this method to set properties on the PropertyManager page before it is displayed or while it is closed. See [IPropertyManagerPage2::Show2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPropertyManagerPage2~Show2.html) and [IPropertyManagerPage2::Close](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPropertyManagerPage2~Close.html) for details.

The bitmap:

* must have less than 256 colors. Its recommended size is 18 - 22 cells wide. However, the bitmap can be any size, as long as it fits on the title bar.* appears transparent by mapping any white (RGB(255,255,255)) cells to the current PropertyManager page title bar background color. Remember the special use of this color as you design your bitmap.* must be a resource in your Visual Studio application.  You must discover its resource ID before you can specify Identifier.

Specify ModuleHandle using the add-in ID.

|  |  |
| --- | --- |
| **If this method is...** | **Then the title bar contains...** |
| Used | Specified bitmap starting at the left edge of the PropertyManager title bar, followed by the title bar text (see [ISldWorks::CreatePropertyManagerPage](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~CreatePropertyManagerPage.html) or [ISldWorks::ICreatePropertyManagerPage](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~ICreatePropertyManagerPage.html)). |
| Not used | Only the text, centered on the title bar. |

# ![](dotnetimages/collapse.gif)See Also

####

[IPropertyManagerPage2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPage2.html)

[IPropertyManagerPage2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPage2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 SP3, Revision Number 18.3