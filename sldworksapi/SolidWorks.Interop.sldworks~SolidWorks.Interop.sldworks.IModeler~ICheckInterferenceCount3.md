<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~ICheckInterferenceCount3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ICheckInterferenceCount3 Method (IModeler) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html) : ICheckInterferenceCount3 Method (IModeler) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NumOfTargetBodies*
:   Number of target bodies

*TargetBodies*
:   Array of target [bodies](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html)

*NumOfToolBodies*
:   Number of tool bodies

*ToolBodies*
:   Array of tool [bodies](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html)

*Options*
:   Check interference options as defined by swCheckInterferenceOption\_e

*NumBody1InterferedFaceArray*
:   Number of [faces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) that interfered from the first body with the second body

*NumBody2InterferedFaceArray*
:   Number of [faces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) that interfered from the second body with the first body

*NumIntersectedBodyArray*
:   Number of interfering [bodies](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html)

Checks interference among the specified bodies and returns the number of interferences.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ICheckInterferenceCount3( _    ByVal NumOfTargetBodies As System.Integer, _    ByRef TargetBodies As Body2, _    ByVal NumOfToolBodies As System.Integer, _    ByRef ToolBodies As Body2, _    ByVal Options As System.Integer, _    ByRef NumBody1InterferedFaceArray As System.Integer, _    ByRef NumBody2InterferedFaceArray As System.Integer, _    ByRef NumIntersectedBodyArray As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModeler Dim NumOfTargetBodies As System.Integer Dim TargetBodies As Body2 Dim NumOfToolBodies As System.Integer Dim ToolBodies As Body2 Dim Options As System.Integer Dim NumBody1InterferedFaceArray As System.Integer Dim NumBody2InterferedFaceArray As System.Integer Dim NumIntersectedBodyArray As System.Integer Dim value As System.Boolean   value = instance.ICheckInterferenceCount3(NumOfTargetBodies, TargetBodies, NumOfToolBodies, ToolBodies, Options, NumBody1InterferedFaceArray, NumBody2InterferedFaceArray, NumIntersectedBodyArray) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ICheckInterferenceCount3(     System.int NumOfTargetBodies,    ref Body2 TargetBodies,    System.int NumOfToolBodies,    ref Body2 ToolBodies,    System.int Options,    out System.int NumBody1InterferedFaceArray,    out System.int NumBody2InterferedFaceArray,    out System.int NumIntersectedBodyArray ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ICheckInterferenceCount3(  &   System.int NumOfTargetBodies, &   Body2^% TargetBodies, &   System.int NumOfToolBodies, &   Body2^% ToolBodies, &   System.int Options, &   [Out] System.int NumBody1InterferedFaceArray, &   [Out] System.int NumBody2InterferedFaceArray, &   [Out] System.int NumIntersectedBodyArray ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*NumOfTargetBodies*
:   Number of target bodies

*TargetBodies*
:   Array of target [bodies](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html)

*NumOfToolBodies*
:   Number of tool bodies

*ToolBodies*
:   Array of tool [bodies](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html)

*Options*
:   Check interference options as defined by swCheckInterferenceOption\_e

*NumBody1InterferedFaceArray*
:   Number of [faces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) that interfered from the first body with the second body

*NumBody2InterferedFaceArray*
:   Number of [faces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) that interfered from the second body with the first body

*NumIntersectedBodyArray*
:   Number of interfering [bodies](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Modeler::ICheckInterferenceCount3.

# ![](dotnetimages/collapse.gif)Remarks

Call this method before calling [IModeler::ICheckInterference3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModeler~ICheckInterference3.html) to get the size of the arrays for that method.

# ![](dotnetimages/collapse.gif)See Also

####

[IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html)

[IModeler Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler_members.html)

[IModeler::ICheckInterference3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~ICheckInterference3.html)

[IModeler::CheckInterference3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~CheckInterference3.html)

[IAssemblyDoc::IToolsCheckInterference3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~IToolsCheckInterference3.html)

[IAssemblyDoc::ToolsCheckInterference2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~ToolsCheckInterference2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 FCS, Revision Number 17.0