<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView~InitializeShading.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InitializeShading Method (IModelView) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView.html) : InitializeShading Method (IModelView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Sets up the model view for OpenGL shading.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub InitializeShading() ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelView   instance.InitializeShading() ``` | |

| C# |  |
| --- | --- |
| ``` void InitializeShading() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void InitializeShading(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelView::InitializeShading.

# ![](dotnetimages/collapse.gif)Remarks

Third-party developers should call this method if they are going to use OpenGL shading and are unsure whether shading has already been used for the current window. This method needs to be called for any window drawn into with OpenGL calls.

This method is provided so third-party applications do not need to use any of the Choos...() functions provided in the OpenGL library. Many of the Choos..() functions, for example ChoosePixelFormat(), can only be called once per window. In the case of ChoosePixelFormat(), a second call to the function is ignored. The effect is harmless if the third-party application makes this call after the SOLIDWORKS application has made the call. However, it is dangerous if the third party were to call it first because the SOLIDWORKS application may require a more complicated format.

To make OpenGL calls,you must get an OpenGL render context (RC). We keep our render context private so that there are not any problems with corruption of SOLIDWORKS RC by an application. To get a rendering context to make OpenGL calls, you must:

uiModelView\_c::InitializeShading()

CClientDC dC(CWnd\* parentWindow);

HGLRC hRc = ::wglCreateContext(dC.m\_hDC);

::wglMakeCurrent(dC.m\_hDC, hRc); (call this before each 'paint' operation)

When you are done using OpenGL for this paint'operation, call:

::wglMakeCurrent(NULL, NULL);

When the DLL shuts down or the [IModelView](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelView.html) object is destroyed (watch for a [DModelViewEvents DestroyNotify2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.DModelViewEvents_DestroyNotify2EventHandler.html)), your application must do the following:

::wglMakeCurrent(NULL, NULL);

::wglDeleteContext(hRc);

# ![](dotnetimages/collapse.gif)See Also

####

[IModelView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView.html)

[IModelView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView_members.html)

[IModelDoc2::ViewOglShading Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ViewOglShading.html)