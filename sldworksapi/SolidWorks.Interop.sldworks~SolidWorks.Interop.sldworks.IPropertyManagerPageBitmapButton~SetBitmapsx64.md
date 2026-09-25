<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageBitmapButton~SetBitmapsx64.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetBitmapsx64 Method (IPropertyManagerPageBitmapButton) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPropertyManagerPageBitmapButton Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageBitmapButton.html) : SetBitmapsx64 Method (IPropertyManagerPageBitmapButton) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ModuleHandle*
:   Module handle of the application instance that contains the image resource

*BitmapUp*
:   Resource ID of the not-clicked state image resource

*BitmapDown*
:   Resource ID of the clicked state image resource

*BitmapDisabled*
:   Resource ID of the disabled state image resource

Sets the images for this button in 64-bit applications.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetBitmapsx64( _    ByVal ModuleHandle As System.Long, _    ByVal BitmapUp As System.Integer, _    ByVal BitmapDown As System.Integer, _    ByVal BitmapDisabled As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPropertyManagerPageBitmapButton Dim ModuleHandle As System.Long Dim BitmapUp As System.Integer Dim BitmapDown As System.Integer Dim BitmapDisabled As System.Integer Dim value As System.Boolean   value = instance.SetBitmapsx64(ModuleHandle, BitmapUp, BitmapDown, BitmapDisabled) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetBitmapsx64(     System.long ModuleHandle,    System.int BitmapUp,    System.int BitmapDown,    System.int BitmapDisabled ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetBitmapsx64(  &   System.int64 ModuleHandle, &   System.int BitmapUp, &   System.int BitmapDown, &   System.int BitmapDisabled ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ModuleHandle*
:   Module handle of the application instance that contains the image resource

*BitmapUp*
:   Resource ID of the not-clicked state image resource

*BitmapDown*
:   Resource ID of the clicked state image resource

*BitmapDisabled*
:   Resource ID of the disabled state image resource

#### Return Value

True if successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PropertyManagerPageBitmapButton::SetBitmapsx64.

# ![](dotnetimages/collapse.gif)Remarks

This method is only available through early binding and with 64-bit versions of the SOLIDWORKS software.

The ModuleHandle argument for this method is the handle to the instance ( HINSTANCE ) of the user DLL, and the resource IDs for the not-clicked, clicked, and disabled states are the image resource integers. The SOLIDWORKS application loads the images from the user DLL and uses them on this bitmap button control.

You must call this method after calling either of the following methods to create the bitmap button control:

* [IPropertyManagerPage2::AddControl](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPropertyManagerPage2~AddControl.html) or [IPropertyManagerPage2::IAddControl](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPropertyManagerPage2~IAddControl.html)

  * [IPropertyManagerPageGroup::AddControl](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPropertyManagerPageGroup~AddControl.html) or [IPropertyManagerPageGroup::IAddControl](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPropertyManagerPageGroup~IAddControl.html)

# ![](dotnetimages/collapse.gif)See Also

####

[IPropertyManagerPageBitmapButton Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageBitmapButton.html)

[IPropertyManagerPageBitmapButton Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageBitmapButton_members.html)

[IPropertyManagerPageBitmapButton::SetBitmaps Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageBitmapButton~SetBitmaps.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 SP4, Revision Number 18.4