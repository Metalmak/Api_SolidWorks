<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMouse~Move.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Move Method (IMouse) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IMouse Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMouse.html) : Move Method (IMouse) |

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
:   y coordinate where to move the pointer

*Flags*
:   Mouse command as defined in swMouse\_e (see **Remarks**)

Moves the mouse pointer in the window space.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function Move( _    ByVal X As System.Integer, _    ByVal Y As System.Integer, _    ByVal Flags As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMouse Dim X As System.Integer Dim Y As System.Integer Dim Flags As System.Integer Dim value As System.Boolean   value = instance.Move(X, Y, Flags) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool Move(     System.int X,    System.int Y,    System.int Flags ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool Move(  &   System.int X, &   System.int Y, &   System.int Flags ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*X*
:   x coordinate where to move the pointer

*Y*
:   y coordinate where to move the pointer

*Flags*
:   Mouse command as defined in swMouse\_e (see **Remarks**)

#### Return Value

True if the pointer moves to the specified position, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Mouse::Move.

# ![](dotnetimages/collapse.gif)Example

[Run SOLIDWORKS Commands and Synthesize Mouse Events (VBA)](Run_SOLIDWORKS_Commands_and_Synthesize_Mouse_Events_Example_VB.htm)

[Run SOLIDWORKS Commands and Synthesize Mouse Events (C#)](Run_SolidWorks_Commands_and_Synthesize_Mouse_Events_Example_CSharp.htm)

[Run SOLIDWORKS Commands and Synthesize Mouse Events (VB.NET)](Run_SolidWorks_Commands_and_Synthesize_Mouse_Events_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

To use this method and access SOLIDWORKS commands, you must add a reference to SOLIDWORKS *version* Commands type library (substitute the actual SOLIDWORKS version number for *version*) or **SolidWorks.Interop.swcommands.dll**, typically installed in *install\_dir***\api\redist.**

In window space, the origin of the coordinate system is the upper-left corner of the window. Positive x is to the right; positive y is down.

# ![](dotnetimages/collapse.gif)See Also

####

[IMouse Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMouse.html)

[IMouse Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMouse_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0