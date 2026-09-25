<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMidSurface~IGetNextFaceArray.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetNextFaceArray Method (IMidSurface) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IMidSurface Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMidSurface.html) : IGetNextFaceArray Method (IMidSurface) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FromFrontFaceListDisp*

*SizeOfFrontFaceList*

*FromFaceBackListDisp*

*SizeOfBackFaceList*

*Thickness*

Obsolete. Superseded by [IMidSurface2::IGetNextFaceArray](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMidSurface2~IGetNextFaceArray.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetNextFaceArray( _    ByVal FromFrontFaceListDisp As System.IntPtr, _    ByRef SizeOfFrontFaceList As System.Integer, _    ByVal FromFaceBackListDisp As System.IntPtr, _    ByRef SizeOfBackFaceList As System.Integer, _    ByRef Thickness As System.Double _ ) As Face ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMidSurface Dim FromFrontFaceListDisp As System.IntPtr Dim SizeOfFrontFaceList As System.Integer Dim FromFaceBackListDisp As System.IntPtr Dim SizeOfBackFaceList As System.Integer Dim Thickness As System.Double Dim value As Face   value = instance.IGetNextFaceArray(FromFrontFaceListDisp, SizeOfFrontFaceList, FromFaceBackListDisp, SizeOfBackFaceList, Thickness) ``` | |

| C# |  |
| --- | --- |
| ``` Face IGetNextFaceArray(     out System.IntPtr FromFrontFaceListDisp,    out System.int SizeOfFrontFaceList,    out System.IntPtr FromFaceBackListDisp,    out System.int SizeOfBackFaceList,    out System.double Thickness ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Face^ IGetNextFaceArray(  &   [Out] System.IntPtr FromFrontFaceListDisp, &   [Out] System.int SizeOfFrontFaceList, &   [Out] System.IntPtr FromFaceBackListDisp, &   [Out] System.int SizeOfBackFaceList, &   [Out] System.double Thickness ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FromFrontFaceListDisp*

*SizeOfFrontFaceList*

*FromFaceBackListDisp*

*SizeOfBackFaceList*

*Thickness*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See MidSurface::IGetNextFaceArray.

# ![](dotnetimages/collapse.gif)See Also

####

[IMidSurface Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMidSurface.html)

[IMidSurface Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMidSurface_members.html)