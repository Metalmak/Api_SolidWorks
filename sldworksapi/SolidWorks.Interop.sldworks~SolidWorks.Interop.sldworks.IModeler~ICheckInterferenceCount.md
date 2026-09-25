<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~ICheckInterferenceCount.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ICheckInterferenceCount Method (IModeler) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html) : ICheckInterferenceCount Method (IModeler) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Body1*

*Body2*

*CoincidentInterference*

*Body1InterferedFaceCount*

*Body2InterferedFaceCount*

*IntersectedBodyCount*

Obsolete. Superseded by [IModeler::ICheckInterferenceCount2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModeler~ICheckInterferenceCount2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ICheckInterferenceCount( _    ByVal Body1 As Body, _    ByVal Body2 As Body, _    ByVal CoincidentInterference As System.Boolean, _    ByRef Body1InterferedFaceCount As System.Integer, _    ByRef Body2InterferedFaceCount As System.Integer, _    ByRef IntersectedBodyCount As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModeler Dim Body1 As Body Dim Body2 As Body Dim CoincidentInterference As System.Boolean Dim Body1InterferedFaceCount As System.Integer Dim Body2InterferedFaceCount As System.Integer Dim IntersectedBodyCount As System.Integer Dim value As System.Boolean   value = instance.ICheckInterferenceCount(Body1, Body2, CoincidentInterference, Body1InterferedFaceCount, Body2InterferedFaceCount, IntersectedBodyCount) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ICheckInterferenceCount(     Body Body1,    Body Body2,    System.bool CoincidentInterference,    out System.int Body1InterferedFaceCount,    out System.int Body2InterferedFaceCount,    out System.int IntersectedBodyCount ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ICheckInterferenceCount(  &   Body^ Body1, &   Body^ Body2, &   System.bool CoincidentInterference, &   [Out] System.int Body1InterferedFaceCount, &   [Out] System.int Body2InterferedFaceCount, &   [Out] System.int IntersectedBodyCount ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Body1*

*Body2*

*CoincidentInterference*

*Body1InterferedFaceCount*

*Body2InterferedFaceCount*

*IntersectedBodyCount*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Modeler::ICheckInterferenceCount.

# ![](dotnetimages/collapse.gif)See Also

####

[IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html)

[IModeler Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler_members.html)