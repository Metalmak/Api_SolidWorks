<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~InsertSurfaceFinishSymbol2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertSurfaceFinishSymbol2 Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : InsertSurfaceFinishSymbol2 Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SymType*

*LeaderType*

*LocX*

*LocY*

*LocZ*

*LaySymbol*

*ArrowType*

*MachAllowance*

*OtherVals*

*ProdMethod*

*SampleLen*

*MaxRoughness*

*MinRoughness*

*RoughnessSpacing*

Obsolete. Superseded by [IModelDocExtension::InsertSurfaceFinishSymbol3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~InsertSurfaceFinishSymbol3.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertSurfaceFinishSymbol2( _    ByVal SymType As System.Integer, _    ByVal LeaderType As System.Integer, _    ByVal LocX As System.Double, _    ByVal LocY As System.Double, _    ByVal LocZ As System.Double, _    ByVal LaySymbol As System.Integer, _    ByVal ArrowType As System.Integer, _    ByVal MachAllowance As System.String, _    ByVal OtherVals As System.String, _    ByVal ProdMethod As System.String, _    ByVal SampleLen As System.String, _    ByVal MaxRoughness As System.String, _    ByVal MinRoughness As System.String, _    ByVal RoughnessSpacing As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim SymType As System.Integer Dim LeaderType As System.Integer Dim LocX As System.Double Dim LocY As System.Double Dim LocZ As System.Double Dim LaySymbol As System.Integer Dim ArrowType As System.Integer Dim MachAllowance As System.String Dim OtherVals As System.String Dim ProdMethod As System.String Dim SampleLen As System.String Dim MaxRoughness As System.String Dim MinRoughness As System.String Dim RoughnessSpacing As System.String Dim value As System.Boolean   value = instance.InsertSurfaceFinishSymbol2(SymType, LeaderType, LocX, LocY, LocZ, LaySymbol, ArrowType, MachAllowance, OtherVals, ProdMethod, SampleLen, MaxRoughness, MinRoughness, RoughnessSpacing) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool InsertSurfaceFinishSymbol2(     System.int SymType,    System.int LeaderType,    System.double LocX,    System.double LocY,    System.double LocZ,    System.int LaySymbol,    System.int ArrowType,    System.string MachAllowance,    System.string OtherVals,    System.string ProdMethod,    System.string SampleLen,    System.string MaxRoughness,    System.string MinRoughness,    System.string RoughnessSpacing ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool InsertSurfaceFinishSymbol2(  &   System.int SymType, &   System.int LeaderType, &   System.double LocX, &   System.double LocY, &   System.double LocZ, &   System.int LaySymbol, &   System.int ArrowType, &   System.String^ MachAllowance, &   System.String^ OtherVals, &   System.String^ ProdMethod, &   System.String^ SampleLen, &   System.String^ MaxRoughness, &   System.String^ MinRoughness, &   System.String^ RoughnessSpacing ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*SymType*

*LeaderType*

*LocX*

*LocY*

*LocZ*

*LaySymbol*

*ArrowType*

*MachAllowance*

*OtherVals*

*ProdMethod*

*SampleLen*

*MaxRoughness*

*MinRoughness*

*RoughnessSpacing*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::InsertSurfaceFinishSymbol2.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)