<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~InsertDatumTargetSymbol2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertDatumTargetSymbol2 Method (IModelDocExtension) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : InsertDatumTargetSymbol2 Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Datum1*
:   Datum reference string 1

*Datum2*
:   Datum reference string 2

*Datum3*
:   Datum reference string 3

*AreaStyle*
:   * 0 = point

      * 1 = circle

        * 2 = rectangle

*AreaOutside*
:   True to display the target area outside, false to not

*Value1*
:   Numeric datum target area diameter or width

*Value2*
:   Numeric datum target area height

*ValueStr1*
:   Value for datum target area diameter or width

*ValueStr2*
:   Value for datum target area height

*ArrowsSmart*
:   True to use smart arrows, false to not

*ArrowStyle*
:   Arrowhead style as defined by swArrowStyle\_e

*LeaderLineStyle*
:   Leaderline style as defined by swLeaderStyle\_e

*LeaderBent*
:   True to create a bent leader line, false to not

*ShowArea*
:   True to show the target area, false to not

*ShowSymbol*
:   True to display the target symbol, false to not

Obsolete. Superseded by [IModelDocExtension::InsertDatumTargetSymbol3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~InsertDatumTargetSymbol3.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertDatumTargetSymbol2( _    ByVal Datum1 As System.String, _    ByVal Datum2 As System.String, _    ByVal Datum3 As System.String, _    ByVal AreaStyle As System.Short, _    ByVal AreaOutside As System.Boolean, _    ByVal Value1 As System.Double, _    ByVal Value2 As System.Double, _    ByVal ValueStr1 As System.String, _    ByVal ValueStr2 As System.String, _    ByVal ArrowsSmart As System.Boolean, _    ByVal ArrowStyle As System.Short, _    ByVal LeaderLineStyle As System.Short, _    ByVal LeaderBent As System.Boolean, _    ByVal ShowArea As System.Boolean, _    ByVal ShowSymbol As System.Boolean _ ) As DatumTargetSym ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim Datum1 As System.String Dim Datum2 As System.String Dim Datum3 As System.String Dim AreaStyle As System.Short Dim AreaOutside As System.Boolean Dim Value1 As System.Double Dim Value2 As System.Double Dim ValueStr1 As System.String Dim ValueStr2 As System.String Dim ArrowsSmart As System.Boolean Dim ArrowStyle As System.Short Dim LeaderLineStyle As System.Short Dim LeaderBent As System.Boolean Dim ShowArea As System.Boolean Dim ShowSymbol As System.Boolean Dim value As DatumTargetSym   value = instance.InsertDatumTargetSymbol2(Datum1, Datum2, Datum3, AreaStyle, AreaOutside, Value1, Value2, ValueStr1, ValueStr2, ArrowsSmart, ArrowStyle, LeaderLineStyle, LeaderBent, ShowArea, ShowSymbol) ``` | |

| C# |  |
| --- | --- |
| ``` DatumTargetSym InsertDatumTargetSymbol2(     System.string Datum1,    System.string Datum2,    System.string Datum3,    System.short AreaStyle,    System.bool AreaOutside,    System.double Value1,    System.double Value2,    System.string ValueStr1,    System.string ValueStr2,    System.bool ArrowsSmart,    System.short ArrowStyle,    System.short LeaderLineStyle,    System.bool LeaderBent,    System.bool ShowArea,    System.bool ShowSymbol ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` DatumTargetSym^ InsertDatumTargetSymbol2(  &   System.String^ Datum1, &   System.String^ Datum2, &   System.String^ Datum3, &   System.short AreaStyle, &   System.bool AreaOutside, &   System.double Value1, &   System.double Value2, &   System.String^ ValueStr1, &   System.String^ ValueStr2, &   System.bool ArrowsSmart, &   System.short ArrowStyle, &   System.short LeaderLineStyle, &   System.bool LeaderBent, &   System.bool ShowArea, &   System.bool ShowSymbol ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Datum1*
:   Datum reference string 1

*Datum2*
:   Datum reference string 2

*Datum3*
:   Datum reference string 3

*AreaStyle*
:   * 0 = point

      * 1 = circle

        * 2 = rectangle

*AreaOutside*
:   True to display the target area outside, false to not

*Value1*
:   Numeric datum target area diameter or width

*Value2*
:   Numeric datum target area height

*ValueStr1*
:   Value for datum target area diameter or width

*ValueStr2*
:   Value for datum target area height

*ArrowsSmart*
:   True to use smart arrows, false to not

*ArrowStyle*
:   Arrowhead style as defined by swArrowStyle\_e

*LeaderLineStyle*
:   Leaderline style as defined by swLeaderStyle\_e

*LeaderBent*
:   True to create a bent leader line, false to not

*ShowArea*
:   True to show the target area, false to not

*ShowSymbol*
:   True to display the target symbol, false to not

#### Return Value

[Datum target symbol](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDatumTargetSym.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::InsertDatumTargetSymbol2.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2005 FCS, Revision Number 13.0