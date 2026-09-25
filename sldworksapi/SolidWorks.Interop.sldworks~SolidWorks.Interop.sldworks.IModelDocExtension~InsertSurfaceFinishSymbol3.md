<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~InsertSurfaceFinishSymbol3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertSurfaceFinishSymbol3 Method (IModelDocExtension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : InsertSurfaceFinishSymbol3 Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SymType*
:   Type of symbol as defined in swSFSymType\_e

*LeaderType*
:   Type of leader as defined in swLeaderStyle\_e

*LocX*
:   x location for symbol

*LocY*
:   y location for symbol

*LocZ*
:   z location for symbol

*LaySymbol*
:   Type of lay direction as defined in swSFLaySym\_e

*ArrowType*
:   Type of arrow head as defined in swArrowStyle\_e

*MachAllowance*
:   Material removal allowance

*OtherVals*
:   Other roughness values

*ProdMethod*
:   Production method and treatment

*SampleLen*
:   Sampling length

*MaxRoughness*
:   Maximum roughness

*MinRoughness*
:   Minimum roughness

*RoughnessSpacing*
:   Roughness spacing

Creates a surface-finish symbol based on the last selection.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertSurfaceFinishSymbol3( _    ByVal SymType As System.Integer, _    ByVal LeaderType As System.Integer, _    ByVal LocX As System.Double, _    ByVal LocY As System.Double, _    ByVal LocZ As System.Double, _    ByVal LaySymbol As System.Integer, _    ByVal ArrowType As System.Integer, _    ByVal MachAllowance As System.String, _    ByVal OtherVals As System.String, _    ByVal ProdMethod As System.String, _    ByVal SampleLen As System.String, _    ByVal MaxRoughness As System.String, _    ByVal MinRoughness As System.String, _    ByVal RoughnessSpacing As System.String _ ) As SFSymbol ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim SymType As System.Integer Dim LeaderType As System.Integer Dim LocX As System.Double Dim LocY As System.Double Dim LocZ As System.Double Dim LaySymbol As System.Integer Dim ArrowType As System.Integer Dim MachAllowance As System.String Dim OtherVals As System.String Dim ProdMethod As System.String Dim SampleLen As System.String Dim MaxRoughness As System.String Dim MinRoughness As System.String Dim RoughnessSpacing As System.String Dim value As SFSymbol   value = instance.InsertSurfaceFinishSymbol3(SymType, LeaderType, LocX, LocY, LocZ, LaySymbol, ArrowType, MachAllowance, OtherVals, ProdMethod, SampleLen, MaxRoughness, MinRoughness, RoughnessSpacing) ``` | |

| C# |  |
| --- | --- |
| ``` SFSymbol InsertSurfaceFinishSymbol3(     System.int SymType,    System.int LeaderType,    System.double LocX,    System.double LocY,    System.double LocZ,    System.int LaySymbol,    System.int ArrowType,    System.string MachAllowance,    System.string OtherVals,    System.string ProdMethod,    System.string SampleLen,    System.string MaxRoughness,    System.string MinRoughness,    System.string RoughnessSpacing ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` SFSymbol^ InsertSurfaceFinishSymbol3(  &   System.int SymType, &   System.int LeaderType, &   System.double LocX, &   System.double LocY, &   System.double LocZ, &   System.int LaySymbol, &   System.int ArrowType, &   System.String^ MachAllowance, &   System.String^ OtherVals, &   System.String^ ProdMethod, &   System.String^ SampleLen, &   System.String^ MaxRoughness, &   System.String^ MinRoughness, &   System.String^ RoughnessSpacing ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*SymType*
:   Type of symbol as defined in swSFSymType\_e

*LeaderType*
:   Type of leader as defined in swLeaderStyle\_e

*LocX*
:   x location for symbol

*LocY*
:   y location for symbol

*LocZ*
:   z location for symbol

*LaySymbol*
:   Type of lay direction as defined in swSFLaySym\_e

*ArrowType*
:   Type of arrow head as defined in swArrowStyle\_e

*MachAllowance*
:   Material removal allowance

*OtherVals*
:   Other roughness values

*ProdMethod*
:   Production method and treatment

*SampleLen*
:   Sampling length

*MaxRoughness*
:   Maximum roughness

*MinRoughness*
:   Minimum roughness

*RoughnessSpacing*
:   Roughness spacing

#### Return Value

Newly inserted [surface finish symbol](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISFSymbol.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::InsertSurfaceFinishSymbol3.

# ![](dotnetimages/collapse.gif)Example

[Get Annotations Arrays (VBA)](Get_Annotations_Array_Example_VB.htm)

[Get Annotations Arrays (VB.NET)](Get_Annotations_Arrays_Example_VBNET.htm)

[Get Annotations Arrays (C#)](Get_Annotations_Arrays_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

The SOLIDWORKS software uses the location parameters for this method only if the surface finish symbol has a leader leaderType != swNO\_LEADER.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2005 FCS, Revision Number 13.0