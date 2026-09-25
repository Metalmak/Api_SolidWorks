<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInterferenceDetectionMgr~GetComponentsTransformInterferenceCount.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetComponentsTransformInterferenceCount Method (IInterferenceDetectionMgr) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IInterferenceDetectionMgr Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInterferenceDetectionMgr.html) : GetComponentsTransformInterferenceCount Method (IInterferenceDetectionMgr) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NumOfComponent*
:   Number of components in the Component array

*Component*
:   Array of [IComponent2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2.html)s

*Transform*
:   [IMathTransform](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathTransform.html)

Calculates and gets the number of interfering components for the specified components and math transform.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetComponentsTransformInterferenceCount( _    ByVal NumOfComponent As System.Integer, _    ByRef Component As Component2, _    ByRef Transform As MathTransform _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IInterferenceDetectionMgr Dim NumOfComponent As System.Integer Dim Component As Component2 Dim Transform As MathTransform Dim value As System.Integer   value = instance.GetComponentsTransformInterferenceCount(NumOfComponent, Component, Transform) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetComponentsTransformInterferenceCount(     System.int NumOfComponent,    ref Component2 Component,    ref MathTransform Transform ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetComponentsTransformInterferenceCount(  &   System.int NumOfComponent, &   Component2^% Component, &   MathTransform^% Transform ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*NumOfComponent*
:   Number of components in the Component array

*Component*
:   Array of [IComponent2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2.html)s

*Transform*
:   [IMathTransform](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathTransform.html)

#### Return Value

Number of interfering components

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See InterferenceDetectionMgr::GetComponentsTransformInterferenceCount.

# ![](dotnetimages/collapse.gif)Remarks

Call this method before calling [IInterferenceDetectionMgr::IGetComponentsTransformInterference](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IInterferenceDetectionMgr~IGetComponentsTransformInterference.html) to get the size of the array returned by that method.

# ![](dotnetimages/collapse.gif)See Also

####

[IInterferenceDetectionMgr Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInterferenceDetectionMgr.html)

[IInterferenceDetectionMgr Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInterferenceDetectionMgr_members.html)

[IInterferenceDetectionMgr::GetComponentsTransformInterferenceCount Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInterferenceDetectionMgr~GetComponentsTransformInterferenceCount.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2012 FCS, Revision Number 20.0