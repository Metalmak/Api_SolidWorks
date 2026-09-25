<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DPartDocEvents_ConvertToBodiesPostNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DPartDocEvents\_ConvertToBodiesPostNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : DPartDocEvents\_ConvertToBodiesPostNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FileName*
:   File name of the part to convert to a body

*SaveOption*
:   Save option as defined in swFileSaveTypes\_e:

    * swFileSaveAs* swFileSaveAsCopy* swFileSaveAsCopyAndOpen

*PreserveGeometryAndSketches*
:   True to preserve geometry and sketches, false to not

Fired after the Convert to Bodies dialog closes.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DPartDocEvents_ConvertToBodiesPostNotifyEventHandler( _    ByVal FileName As System.String, _    ByVal SaveOption As System.Integer, _    ByVal PreserveGeometryAndSketches As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DPartDocEvents_ConvertToBodiesPostNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DPartDocEvents_ConvertToBodiesPostNotifyEventHandler(     System.string FileName,    System.int SaveOption,    System.bool PreserveGeometryAndSketches ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DPartDocEvents_ConvertToBodiesPostNotifyEventHandler(  &   System.String^ FileName, &   System.int SaveOption, &   System.bool PreserveGeometryAndSketches ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FileName*
:   File name of the part to convert to a body

*SaveOption*
:   Save option as defined in swFileSaveTypes\_e:

    * swFileSaveAs* swFileSaveAsCopy* swFileSaveAsCopyAndOpen

*PreserveGeometryAndSketches*
:   True to preserve geometry and sketches, false to not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ConvertToBodiesPostNotify Event (PartDoc).

# ![](dotnetimages/collapse.gif)Remarks

This event is triggered after the user clicks **OK** or **Cancel** in the Convert to Bodies dialog and before user interface validation. FileName, SaveOption and PreserveGeometryAndSketches contain the values selected in the dialog.

If developing a C++ application, use swPartConvertToBodiesPostNotify to register for this notification.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2018 FCS, Revision Number 26.0