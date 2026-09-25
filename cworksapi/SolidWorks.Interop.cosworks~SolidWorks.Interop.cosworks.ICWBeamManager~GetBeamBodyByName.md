<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamManager~GetBeamBodyByName.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetBeamBodyByName Method (ICWBeamManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWBeamManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamManager.html) : GetBeamBodyByName Method (ICWBeamManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SBeamBodyName*
:   Name of beam body

*ErrorCode*
:   0 if successful, 1 if not

Gets the specified beam body.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetBeamBodyByName( _    ByVal SBeamBodyName As System.String, _    ByRef ErrorCode As System.Integer _ ) As CWBeamBody ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWBeamManager Dim SBeamBodyName As System.String Dim ErrorCode As System.Integer Dim value As CWBeamBody   value = instance.GetBeamBodyByName(SBeamBodyName, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` CWBeamBody GetBeamBodyByName(     System.string SBeamBodyName,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` CWBeamBody^ GetBeamBodyByName(  &   System.String^ SBeamBodyName, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*SBeamBodyName*
:   Name of beam body

*ErrorCode*
:   0 if successful, 1 if not

#### Return Value

[ICWBeamBody](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWBeamManager::GetBeamBodyByName.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWBeamManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamManager.html)

[ICWBeamManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamManager_members.html)

[ICWBeamManager::GetBeamBodyAt Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamManager~GetBeamBodyAt.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2017 SP0