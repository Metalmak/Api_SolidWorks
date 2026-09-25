<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension~SetBrokenLeader2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetBrokenLeader2 Method (IDisplayDimension) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDisplayDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension.html) : SetBrokenLeader2 Method (IDisplayDimension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*UseDoc*
:   True uses the document default setting, false uses the setting specified in the Broken argument

*Broken*
:   Broken leader value as defined in swDisplayDimensionLeaderText\_e if UseDoc is false

Sets the broken leader display characteristic of this display dimension.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetBrokenLeader2( _    ByVal UseDoc As System.Boolean, _    ByVal Broken As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDisplayDimension Dim UseDoc As System.Boolean Dim Broken As System.Integer Dim value As System.Integer   value = instance.SetBrokenLeader2(UseDoc, Broken) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetBrokenLeader2(     System.bool UseDoc,    System.int Broken ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetBrokenLeader2(  &   System.bool UseDoc, &   System.int Broken ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*UseDoc*
:   True uses the document default setting, false uses the setting specified in the Broken argument

*Broken*
:   Broken leader value as defined in swDisplayDimensionLeaderText\_e if UseDoc is false

#### Return Value

Return status:

|  |  |
| --- | --- |
| -1 | Command failed, no broken leader values were set |
| 0 | Command was successful, all precision values were set |
| 1 | Specified broken value is invalid, the display dimension was set to use the document default |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DisplayDimension::SetBrokenLeader2.

# ![](dotnetimages/collapse.gif)Remarks

Dimension text can be displayed above a solid, unbroken leader line, or broken with the text displayed horizontally or aligned with the leader line. This method allows you to determine if this [IDisplayDimension](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDisplayDimension.html) uses the default document setting for this value or if the user has applied a specific setting.

If UseDoc is True, then SOLIDWORKS ignores the broken value.

The return value indicates the success or failure of this method. In general, a value less than 0 indicates that the command failed, and no broken leader values were set. A value of 0 indicates success.

Use [IDisplayDimension::GetUseDocBrokenLeader](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDisplayDimension~GetUseDocBrokenLeader.html) and [IDisplayDimension::GetBrokenLeader2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDisplayDimension~GetBrokenLeader2.html) to get these values.

After using this method, use [IModelDoc2::GraphicsRedraw2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~GraphicsRedraw2.html) to redraw the graphics window to see your changes.

# ![](dotnetimages/collapse.gif)See Also

####

[IDisplayDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension.html)

[IDisplayDimension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension_members.html)

[IDisplayDimension::SetBrokenLeader2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension~SetBrokenLeader2.html)

[IDisplayDimension::GetUseDocBrokenLeader Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension~GetUseDocBrokenLeader.html)

[IDisplayDimension::SolidLeader Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension~SolidLeader.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 99, datecode 1999207