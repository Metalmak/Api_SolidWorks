<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~LBDownAt.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| LBDownAt Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : LBDownAt Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Flags*
:   Any combination of:

    * MK\_CONTROL

      * MK\_LBUTTON

        * MK\_MBUTTON

          * MK\_RBUTTON

            * MK\_SHIFT

*X*
:   X coordinate of position of cursor

*Y*
:   Y coordinate of position of cursor

*Z*
:   Z coordinate of position of cursor

Generates a left mouse button press (down) event.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub LBDownAt( _    ByVal Flags As System.Integer, _    ByVal X As System.Double, _    ByVal Y As System.Double, _    ByVal Z As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim Flags As System.Integer Dim X As System.Double Dim Y As System.Double Dim Z As System.Double   instance.LBDownAt(Flags, X, Y, Z) ``` | |

| C# |  |
| --- | --- |
| ``` void LBDownAt(     System.int Flags,    System.double X,    System.double Y,    System.double Z ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void LBDownAt(  &   System.int Flags, &   System.double X, &   System.double Y, &   System.double Z ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Flags*
:   Any combination of:

    * MK\_CONTROL

      * MK\_LBUTTON

        * MK\_MBUTTON

          * MK\_RBUTTON

            * MK\_SHIFT

*X*
:   X coordinate of position of cursor

*Y*
:   Y coordinate of position of cursor

*Z*
:   Z coordinate of position of cursor

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::LBDownAt.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

[IModelDoc2::LBUpAt Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~LBUpAt.html)

[IModelDoc2::DragTo Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~DragTo.html)

[IMouse Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMouse.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0