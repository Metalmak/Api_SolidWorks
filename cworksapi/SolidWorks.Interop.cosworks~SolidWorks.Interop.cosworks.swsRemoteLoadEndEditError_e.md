<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsRemoteLoadEndEditError_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsRemoteLoadEndEditError\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsRemoteLoadEndEditError\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Remote load editing errors

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsRemoteLoadEndEditError_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsRemoteLoadEndEditError_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsRemoteLoadEndEditError_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsRemoteLoadEndEditError_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsRemoteLoadEndEditError\_CheckAtleastOneComp** | 11 = Select at least one load component |
| **swsRemoteLoadEndEditError\_DisplacementMustBe0ForTopology** | 15 = Displacement components in remote loads in topology studies must be zero |
| **swsRemoteLoadEndEditError\_EmptyArray** | 6 = Empty array |
| **swsRemoteLoadEndEditError\_EntityAlreadyAdded** | 7 = Entity already exists |
| **swsRemoteLoadEndEditError\_InvalidArray** | 5 = Invalid array |
| **swsRemoteLoadEndEditError\_InvalidConnectionType** | 16 = Connection type should be 0 or 1 |
| **swsRemoteLoadEndEditError\_InvalidForAnalysis** | 12 = Only linear static and nonlinear static studies support remote loads with distributed connection types |
| **swsRemoteLoadEndEditError\_InvalidForNonSolid** | 13 = You must select entities on solid bodies for remote loads with distributed connection types |
| **swsRemoteLoadEndEditError\_InvalidForRigid** | 14 = The selections are invalid for a remote load with a rigid connection type |
| **swsRemoteLoadEndEditError\_InvalidLoadType** | 3 = Remote load type is invalid |
| **swsRemoteLoadEndEditError\_InvalidMass** | 10 = Mass should be greater than 0 |
| **swsRemoteLoadEndEditError\_InvalidMassArray** | 9 = Invalid mass array |
| **swsRemoteLoadEndEditError\_InvalidStudyType** | 4 = Study type is invalid for the remote load type |
| **swsRemoteLoadEndEditError\_InvalidUnits** | 8 = Incorrect units |
| **swsRemoteLoadEndEditError\_NoError** | 0 = Success |
| **swsRemoteLoadEndEditError\_SelectCoordinateSystem** | 2 = Select a coordinate system |
| **swsRemoteLoadEndEditError\_SelectFaceEdgeOrVertex** | 1 = Select a face, edge, or vertex |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)