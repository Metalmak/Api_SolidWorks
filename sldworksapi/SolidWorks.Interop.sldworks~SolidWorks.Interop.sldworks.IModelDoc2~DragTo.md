<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~DragTo.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DragTo Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : DragTo Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Flags*
:   Mouse-event flags as defined by the operating system. They can be combined to indicate the selection state.  For example:

    * Left-mouse button is pressed: 0x0001

      * Right-mouse button is pressed:  0x0002

        * Shift key is pressed:  0x0004

          * Ctrl key is pressed: 0x0008

            * Middle-mouse button is pressed:  0x0010

*X*
:   X coordinate of end point

*Y*
:   Y coordinate of end point

*Z*
:   Z coordinate of end point

Drags the specified end point.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub DragTo( _    ByVal Flags As System.Integer, _    ByVal X As System.Double, _    ByVal Y As System.Double, _    ByVal Z As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim Flags As System.Integer Dim X As System.Double Dim Y As System.Double Dim Z As System.Double   instance.DragTo(Flags, X, Y, Z) ``` | |

| C# |  |
| --- | --- |
| ``` void DragTo(     System.int Flags,    System.double X,    System.double Y,    System.double Z ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void DragTo(  &   System.int Flags, &   System.double X, &   System.double Y, &   System.double Z ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Flags*
:   Mouse-event flags as defined by the operating system. They can be combined to indicate the selection state.  For example:

    * Left-mouse button is pressed: 0x0001

      * Right-mouse button is pressed:  0x0002

        * Shift key is pressed:  0x0004

          * Ctrl key is pressed: 0x0008

            * Middle-mouse button is pressed:  0x0010

*X*
:   X coordinate of end point

*Y*
:   Y coordinate of end point

*Z*
:   Z coordinate of end point

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::DragTo.

# ![](dotnetimages/collapse.gif)Remarks

This method is only valid for assemblies.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0