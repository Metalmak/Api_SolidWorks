<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidManager~GetComponentAt.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetComponentAt Method (ICWSolidManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWSolidManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidManager.html) : GetComponentAt Method (ICWSolidManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NIndex*
:   0-based index of the solid component to get

*ErrorCode*
:   0 if successful, 1 if no solid component at NIndex

Gets the solid component at the specified index.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetComponentAt( _    ByVal NIndex As System.Integer, _    ByRef ErrorCode As System.Integer _ ) As CWSolidComponent ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWSolidManager Dim NIndex As System.Integer Dim ErrorCode As System.Integer Dim value As CWSolidComponent   value = instance.GetComponentAt(NIndex, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` CWSolidComponent GetComponentAt(     System.int NIndex,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` CWSolidComponent^ GetComponentAt(  &   System.int NIndex, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*NIndex*
:   0-based index of the solid component to get

*ErrorCode*
:   0 if successful, 1 if no solid component at NIndex

#### Return Value

[Solid component](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWSolidComponent.html) or NULL if no solid component at NIndex

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWSolidManager::GetComponentAt.

# ![](dotnetimages/collapse.gif)Example

See the [ICWSolidManager](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidManager.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, call [ICWSolidManager::ComponentCount](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWSolidManager~ComponentCount.html) to get NIndex. Index starts at 0.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWSolidManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidManager.html)

[ICWSolidManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2008 SP1.0