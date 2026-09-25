<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetButtonPosition.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetButtonPosition Method (ISldWorks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : GetButtonPosition Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*PointAt*
:   Command ID for SOLIDWORKS toolbar button as defined in swCommands\_e

*LocX*
:   x coordinate of the center of the specified SOLIDWORKS toolbar button

*LocY*
:   y coordinate of the center of the specified SOLIDWORKS toolbar button

Gets the center coordinates of the specified SOLIDWORKS toolbar button.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetButtonPosition( _    ByVal PointAt As System.Integer, _    ByRef LocX As System.Integer, _    ByRef LocY As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim PointAt As System.Integer Dim LocX As System.Integer Dim LocY As System.Integer Dim value As System.Boolean   value = instance.GetButtonPosition(PointAt, LocX, LocY) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetButtonPosition(     System.int PointAt,    out System.int LocX,    out System.int LocY ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetButtonPosition(  &   System.int PointAt, &   [Out] System.int LocX, &   [Out] System.int LocY ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*PointAt*
:   Command ID for SOLIDWORKS toolbar button as defined in swCommands\_e

*LocX*
:   x coordinate of the center of the specified SOLIDWORKS toolbar button

*LocY*
:   y coordinate of the center of the specified SOLIDWORKS toolbar button

#### Return Value

True if method call is successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::GetButtonPosition.

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[ISldWorks::AddToolbar5 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~AddToolbar5.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0