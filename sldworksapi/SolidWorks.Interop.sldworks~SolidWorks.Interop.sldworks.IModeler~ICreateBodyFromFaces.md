<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~ICreateBodyFromFaces.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ICreateBodyFromFaces Method (IModeler) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html) : ICreateBodyFromFaces Method (IModeler) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NumOfFaces*

*Faces*

*DoLocalCheck*

*LocalCheckResult*

Obsolete. Superseded by [IModeler::ICreateBodyFromFace3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModeler~ICreateBodyFromFaces3.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ICreateBodyFromFaces( _    ByVal NumOfFaces As System.Integer, _    ByRef Faces As Face, _    ByVal DoLocalCheck As System.Boolean, _    ByRef LocalCheckResult As System.Boolean _ ) As Body ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModeler Dim NumOfFaces As System.Integer Dim Faces As Face Dim DoLocalCheck As System.Boolean Dim LocalCheckResult As System.Boolean Dim value As Body   value = instance.ICreateBodyFromFaces(NumOfFaces, Faces, DoLocalCheck, LocalCheckResult) ``` | |

| C# |  |
| --- | --- |
| ``` Body ICreateBodyFromFaces(     System.int NumOfFaces,    ref Face Faces,    System.bool DoLocalCheck,    ref System.bool LocalCheckResult ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Body^ ICreateBodyFromFaces(  &   System.int NumOfFaces, &   Face^% Faces, &   System.bool DoLocalCheck, &   System.bool% LocalCheckResult ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*NumOfFaces*

*Faces*

*DoLocalCheck*

*LocalCheckResult*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Modeler::ICreateBodyFromFaces.

# ![](dotnetimages/collapse.gif)See Also

####

[IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html)

[IModeler Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler_members.html)