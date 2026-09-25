<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~Command.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Command Method (ISldWorks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : Command Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Command*
:   Command as defined by swCommand\_e

*Args*
:   See Remarks

Opens the specified dialog or file.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function Command( _    ByVal Command As System.Integer, _    ByVal Args As System.Object _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim Command As System.Integer Dim Args As System.Object Dim value As System.Object   value = instance.Command(Command, Args) ``` | |

| C# |  |
| --- | --- |
| ``` System.object Command(     System.int Command,    System.object Args ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ Command(  &   System.int Command, &   System.Object^ Args ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Command*
:   Command as defined by swCommand\_e

*Args*
:   See Remarks

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::Command.

# ![](dotnetimages/collapse.gif)Remarks

|  |  |
| --- | --- |
| **If command specified is...** | **Then pass...** |
| swOpenHTMLHelp | Path and filename for the compiled HTML file (has .chm filename extension) |
| * swFileOpen * swFileNew * swOpenRecentFile | Empty VARIANT; for example:   VARIANT args;   V\_VT(&args) = VT\_EMPTY;   // Call Command API and open the File, Open dialog   swApp->Command(0, args, &retval); |

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12.0