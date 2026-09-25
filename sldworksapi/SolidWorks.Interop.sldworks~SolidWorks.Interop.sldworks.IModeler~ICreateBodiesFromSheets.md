<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~ICreateBodiesFromSheets.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ICreateBodiesFromSheets Method (IModeler) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html) : ICreateBodiesFromSheets Method (IModeler) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NSheets*

*Sheets*

*Options*

*NResults*

*Results*

Obsolete. Superseded by [IModeler::ICreateBodiesFromSheets2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModeler~ICreateBodiesFromSheets2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ICreateBodiesFromSheets( _    ByVal NSheets As System.Integer, _    ByRef Sheets As System.Object, _    ByVal Options As System.Integer, _    ByRef NResults As System.Integer, _    ByRef Results As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModeler Dim NSheets As System.Integer Dim Sheets As System.Object Dim Options As System.Integer Dim NResults As System.Integer Dim Results As System.Object Dim value As System.Integer   value = instance.ICreateBodiesFromSheets(NSheets, Sheets, Options, NResults, Results) ``` | |

| C# |  |
| --- | --- |
| ``` System.int ICreateBodiesFromSheets(     System.int NSheets,    ref System.object Sheets,    System.int Options,    out System.int NResults,    out System.object Results ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int ICreateBodiesFromSheets(  &   System.int NSheets, &   System.Object^% Sheets, &   System.int Options, &   [Out] System.int NResults, &   [Out] System.Object^ Results ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*NSheets*

*Sheets*

*Options*

*NResults*

*Results*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Modeler::ICreateBodiesFromSheets.

# ![](dotnetimages/collapse.gif)See Also

####

[IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html)

[IModeler Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler_members.html)