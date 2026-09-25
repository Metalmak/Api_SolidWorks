<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMouse~MouseWheelXYZ.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| MouseWheelXYZ Method (IMouse) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IMouse Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMouse.html) : MouseWheelXYZ Method (IMouse) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*X*
:   x coordinate where to move the pointer

*Y*
:   y coordinate where to move the pointer

*Z*
:   z coordinate where to move the pointer

*Clicks*
:   Number of clicks to zoom in and out; specify -120 to to zoom in one click and specify 120 to to zoom out

*Flags*
:   Mouse command as defined in swMouse\_e (see **Remarks**)

Zoom in or zoom out using the mouse.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function MouseWheelXYZ( _    ByVal X As System.Double, _    ByVal Y As System.Double, _    ByVal Z As System.Double, _    ByVal Clicks As System.Integer, _    ByVal Flags As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMouse Dim X As System.Double Dim Y As System.Double Dim Z As System.Double Dim Clicks As System.Integer Dim Flags As System.Integer Dim value As System.Boolean   value = instance.MouseWheelXYZ(X, Y, Z, Clicks, Flags) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool MouseWheelXYZ(     System.double X,    System.double Y,    System.double Z,    System.int Clicks,    System.int Flags ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool MouseWheelXYZ(  &   System.double X, &   System.double Y, &   System.double Z, &   System.int Clicks, &   System.int Flags ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*X*
:   x coordinate where to move the pointer

*Y*
:   y coordinate where to move the pointer

*Z*
:   z coordinate where to move the pointer

*Clicks*
:   Number of clicks to zoom in and out; specify -120 to to zoom in one click and specify 120 to to zoom out

*Flags*
:   Mouse command as defined in swMouse\_e (see **Remarks**)

#### Return Value

True if the operation succeeded, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Mouse::MouseWheelXYZ.

# ![](dotnetimages/collapse.gif)Example

**Visual Basic for Applications (VBA)**

'--------------------------------
' Preconditions: Model document is open.
'
' Postconditions: Model is zoomed in and out.
**'--------------------------------**

Option Explicit

Dim swApp As SldWorks.SldWorks
Dim swModel As SldWorks.ModelDoc2
Dim swModelView As SldWorks.ModelView
Dim swMouse As SldWorks.Mouse

Sub main()

    Set swApp = Application.SldWorks
    Set swModel = swApp.**ActiveDoc**
    Set swModelView = swModel.**ActiveView**
    Set swMouse = swModelView.**GetMouse**

    swMouse.**MouseWheelXYZ** 0, 0, 0, 120, swMouse\_RightUp
    swMouse.**MouseWheelXYZ** 0, 0, 0, 120, swMouse\_RightUp
    swMouse.**MouseWheelXYZ** 0, 0, 0, 240, swMouse\_RightUp
    swMouse.**MouseWheelXYZ** 0, 0, 0, -120, swMouse\_RightUp
    swMouse.**MouseWheelXYZ** 0, 0, 0, -240, swMouse\_RightUp

End Sub

# ![](dotnetimages/collapse.gif)Remarks

To use this method and access SOLIDWORKS commands, you must add a reference to SOLIDWORKS *version* Commands type library (substitute the actual SOLIDWORKS version number for *version*) or **SolidWorks.Interop.swcommands.dll**, typically installed in *install\_dir***\api\redist.**

The coordinate system is the model's coordinate system.

# ![](dotnetimages/collapse.gif)See Also

####

[IMouse Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMouse.html)

[IMouse Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMouse_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 FCS, Revision Number 17.0