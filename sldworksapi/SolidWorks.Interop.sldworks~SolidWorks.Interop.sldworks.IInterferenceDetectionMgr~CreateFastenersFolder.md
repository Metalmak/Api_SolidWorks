<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInterferenceDetectionMgr~CreateFastenersFolder.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateFastenersFolder Property (IInterferenceDetectionMgr) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IInterferenceDetectionMgr Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInterferenceDetectionMgr.html) : CreateFastenersFolder Property (IInterferenceDetectionMgr) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets whether to create the Fasteners folders to segregate interferences involving fasteners.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property CreateFastenersFolder As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IInterferenceDetectionMgr Dim value As System.Boolean   instance.CreateFastenersFolder = value   value = instance.CreateFastenersFolder ``` | |

| C# |  |
| --- | --- |
| ``` System.bool CreateFastenersFolder {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool CreateFastenersFolder {    System.bool get();    void set ( &   System.bool value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

True to create fasteners folder, false to not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See InterferenceDetectionMgr::CreateFastenersFolder.

# ![](dotnetimages/collapse.gif)Example

[Run Interference Detection (C#)](Run_Interference_Detection_Example_CSharp.htm)

[Run Interference Detection (VB.NET)](Run_Interference_Detection_Example_VBNET.htm)

[Run Interference Detection (VBA)](Run_Interference_Detection_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Currently, the value set for this property:

* exists only while the InterferenceDetectionMgr object is in scope; i.e., setting this property is temporary.* does not persist across SOLIDWORKS sessions.* does not persist into the next invocation of interference detection in the user interface.

# ![](dotnetimages/collapse.gif)See Also

####

[IInterferenceDetectionMgr Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInterferenceDetectionMgr.html)

[IInterferenceDetectionMgr Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInterferenceDetectionMgr_members.html)

[IInterference::IsFastener Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInterference~IsFastener.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0