<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICamera~Pitch.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Pitch Property (ICamera) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICamera Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICamera.html) : Pitch Property (ICamera) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the pitch (up or down angle) of a [floating camera](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICamera~Type.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property Pitch As System.Double ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICamera Dim value As System.Double   instance.Pitch = value   value = instance.Pitch ``` | |

| C# |  |
| --- | --- |
| ``` System.double Pitch {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.double Pitch {    System.double get();    void set ( &   System.double value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

Pitch

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Camera::Pitch.

# ![](dotnetimages/collapse.gif)Example

[Insert and Rotate Camera (C#)](Insert_and_Rotate_Camera_Example_CSharp.htm)

[Insert and Rotate Camera (VB.NET)](Insert_and_Rotate_Camera_Example_VBNET.htm)

[Insert and Rotate Camera (VBA)](Insert_and_Rotate_Camera_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ICamera Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICamera.html)

[ICamera Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICamera_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 SP4, Revision Number 17.4