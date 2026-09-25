<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~IEnableStereoDisplay.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IEnableStereoDisplay Method (ISldWorks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : IEnableStereoDisplay Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BEnable*
:   Bitfield flags that control the application's stereo support status

Obsolete and not superseded. Functionality no longer implemented.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IEnableStereoDisplay( _    ByVal BEnable As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim BEnable As System.Boolean Dim value As System.Boolean   value = instance.IEnableStereoDisplay(BEnable) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool IEnableStereoDisplay(     System.bool BEnable ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool IEnableStereoDisplay(  &   System.bool BEnable ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*BEnable*
:   Bitfield flags that control the application's stereo support status

#### Return Value

True if stereo attribute setting was successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::IEnableStereoDisplay.

# ![](dotnetimages/collapse.gif)Remarks

You must select the Enable Quadbuffered Stereo API check box for NVIDIA Quadro4 OpenGL video cards before opening any windows.

Calling this method with bit #0, the low bit, of the flags field set (flags |= 0x01) sets up all subsequently opened document windows to be capable of displaying stereo; already opened document windows are not affected. If this method is not called, or if it is called with the low bit of flags cleared, the document windows are not be capable of displaying stereo.

Bit #1 controls whether or not3D scenes are displayed to separate left-eye and right-eye stereoscopic buffers. If bit #1 of the flags field is set (flags |= 0x02), separately buffered stereo pairs are rendered for all windows with 3D scenes that are capable of displaying stereo.

Thus, any plug-in that might need to display stereoscopically should, upon loading, immediately call this method, with the flags field set to 0x01. To actually activate stereo display, call this method with the flags field set to 0x03. To deactivate stereo display, call this method with the flags field set to 0x01. Finally, just before the plug-in uninstalls, restore SOLIDWORKS' default behavior by calling this method with the flags field set to 0x00.

For the stereo pair renderings to appear stereoscopic, call [IModelView::SetStereoSeparation](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelView~SetStereoSeparation.html) or [IModelView::ISetStereoSeparation](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelView~ISetStereoSeparation.html). By default, the stereo rendering-control attributes that are set by IModelView::SetStereoSeparation or IModelView::ISetStereoSeparation are set for identical left-eye and right-eye renderings.

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)