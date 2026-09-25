<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~ISplitFaceOnParamCount.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ISplitFaceOnParamCount Method (IModeler) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html) : ISplitFaceOnParamCount Method (IModeler) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Facedisp*

*UVFlag*

*Parameter*

*Status*

Obsolete. Superseded by [IModeler::ISplitFaceOnParamCount2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModeler~ISplitFaceOnParamCount2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ISplitFaceOnParamCount( _    ByVal Facedisp As Face, _    ByVal UVFlag As System.Integer, _    ByVal Parameter As System.Double, _    ByRef Status As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModeler Dim Facedisp As Face Dim UVFlag As System.Integer Dim Parameter As System.Double Dim Status As System.Boolean Dim value As System.Integer   value = instance.ISplitFaceOnParamCount(Facedisp, UVFlag, Parameter, Status) ``` | |

| C# |  |
| --- | --- |
| ``` System.int ISplitFaceOnParamCount(     Face Facedisp,    System.int UVFlag,    System.double Parameter,    out System.bool Status ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int ISplitFaceOnParamCount(  &   Face^ Facedisp, &   System.int UVFlag, &   System.double Parameter, &   [Out] System.bool Status ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Facedisp*

*UVFlag*

*Parameter*

*Status*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Modeler::ISplitFaceOnParamCount.

# ![](dotnetimages/collapse.gif)See Also

####

[IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html)

[IModeler Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler_members.html)