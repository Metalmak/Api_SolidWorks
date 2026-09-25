<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation~SetLeader3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetLeader3 Method (IAnnotation) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation.html) : SetLeader3 Method (IAnnotation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*LeaderStyle*
:   Leader style as defined in swLeaderStyle\_e (see **Remarks**)

*LeaderSide*
:   Leader side as defined in swLeaderSide\_e (see **Remarks**)

*SmartArrowHeadStyle*
:   True to enable smart arrowhead style, false to disable it (see **Remarks**)

*Perpendicular*
:   True to enable perpendicular bent leader display, false to disable it (see **Remarks**)

*AllAround*
:   True to enable all around symbol display, false to disable it (see **Remarks**)

*Dashed*
:   True to enable dashed line leader display; false to enable solid-line leader (see **Remarks**)

Sets the leader characteristics for this annotation.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetLeader3( _    ByVal LeaderStyle As System.Integer, _    ByVal LeaderSide As System.Integer, _    ByVal SmartArrowHeadStyle As System.Boolean, _    ByVal Perpendicular As System.Boolean, _    ByVal AllAround As System.Boolean, _    ByVal Dashed As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAnnotation Dim LeaderStyle As System.Integer Dim LeaderSide As System.Integer Dim SmartArrowHeadStyle As System.Boolean Dim Perpendicular As System.Boolean Dim AllAround As System.Boolean Dim Dashed As System.Boolean Dim value As System.Integer   value = instance.SetLeader3(LeaderStyle, LeaderSide, SmartArrowHeadStyle, Perpendicular, AllAround, Dashed) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetLeader3(     System.int LeaderStyle,    System.int LeaderSide,    System.bool SmartArrowHeadStyle,    System.bool Perpendicular,    System.bool AllAround,    System.bool Dashed ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetLeader3(  &   System.int LeaderStyle, &   System.int LeaderSide, &   System.bool SmartArrowHeadStyle, &   System.bool Perpendicular, &   System.bool AllAround, &   System.bool Dashed ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*LeaderStyle*
:   Leader style as defined in swLeaderStyle\_e (see **Remarks**)

*LeaderSide*
:   Leader side as defined in swLeaderSide\_e (see **Remarks**)

*SmartArrowHeadStyle*
:   True to enable smart arrowhead style, false to disable it (see **Remarks**)

*Perpendicular*
:   True to enable perpendicular bent leader display, false to disable it (see **Remarks**)

*AllAround*
:   True to enable all around symbol display, false to disable it (see **Remarks**)

*Dashed*
:   True to enable dashed line leader display; false to enable solid-line leader (see **Remarks**)

#### Return Value

Indicates whether the operation was successful (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Annotation::SetLeader3.

# ![](dotnetimages/collapse.gif)Example

[Insert GTol (C#)](Insert_GTol_Example_CSharp.htm)

[Insert GTol (VB.NET)](Insert_GTol_Example_VBNET.htm)

[Insert GTol (VBA)](Insert_GTol_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Not all annotations support all styles of leaders or leader characteristics. Only notes, GTols, surface finish symbols, weld symbols, datum target symbols, and block instances support leaders of any kind.

* Weld symbol leaders can be hidden, but are always bent; straight leaders (swSTRAIGHT) are not supported.

  * Datum target symbols can have straight or bent leaders, but cannot be hidden (swNO\_LEADER is not supported).

    * Only notes support underline leaders (swUNDERLINED).

      * GTols are the only type of annotation that supports perpendicular bent leaders.

        * GTols and weld symbols are the only types of annotations that support all around leader symbols.

          * Datum target symbols are the only type of annotation that supports dashed leaders.

This method sets the characteristics of the annotation, not the individual leaders. You can get or set these characteristics whether leaders are displayed.

|  |  |
| --- | --- |
| **Use...** | **To...** |
| [IAnnotation::GetDashedLeader](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAnnotation~GetDashedLeader.html) | Determine whether this leader is a dashed line or a solid line. |
| [IAnnotation::GetLeaderAllARound](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAnnotation~GetLeaderAllAround.html) | Determine whether all around symbol display is enabled or disabled. |
| [IAnnotation::GetLeaderPerpendicular](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAnnotation~GetLeaderPerpendicular.html) | Determine whether perpendicular bent leader display is enabled or disabled. |
| [IAnnotation::GetLeaderSide](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAnnotation~GetLeaderSide.html) | Get the leader attachment side setting. |
| [IAnnotation::GetLeaderStyle](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAnnotation~GetLeaderStyle.html) | Get style of leader (hidden, straight, bent, or underline). |
| [IAnnotation::GetSmartArrowHeadStyle](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAnnotation~GetSmartArrowHeadStyle.html) | Determine whether smart arrowhead style is enabled or disabled. |

You can set the leader side, smart arrowhead style, and bent leader values at any time. However, if leader display is disabled, you cannot affect the display of the annotation by setting these values. You can also set the perpendicular bent leader and all around symbol display at any time, but if bent leaders are disabled, you cannot affect the display of the annotation by setting these values.

The return status of this operation can have the following values:

* 0 = Leader characteristics were successfully set

  * -1 = Leader characteristics were not set because of an unknown error

    * -2 = Leader attachment side setting is invalid

      * -3 = Leaders are not supported on this type of annotation

        * -4 = Leaders cannot be disabled on this type of annotation

          * -5 = Bent leaders cannot be disabled on this type of annotation

            * -6 = Underline style leaders are not allowed on this type of annotation

If leader display is enabled, then this method changes the visible model.

# ![](dotnetimages/collapse.gif)See Also

####

[IAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation.html)

[IAnnotation Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation_members.html)

[IAnnotation::GetLeader Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation~GetLeader.html)

[IAnnotation::GetLeaderCount Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation~GetLeaderCount.html)

[IAnnotation::GetLeaderPointsAtIndex Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation~GetLeaderPointsAtIndex.html)

[IAnnotation::GetMultiJogLeaderCount Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation~GetMultiJogLeaderCount.html)

[IAnnotation::GetMultiJogLeaders Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation~GetMultiJogLeaders.html)

[IAnnotation::BentLeaderLength Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation~BentLeaderLength.html)

[IAnnotation::LeaderLineStyle Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation~LeaderLineStyle.html)

[IAnnotation::LeaderThickness Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation~LeaderThickness.html)

[IAnnotation::LeaderThicknessCustom Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation~LeaderThicknessCustom.html)

[IAnnotation::UseDocDispLeader Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation~UseDocDispLeader.html)

[IAnnotation::SetLeaderAttachmentPointAtIndex Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation~SetLeaderAttachmentPointAtIndex.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 FCS, Revision Number 14.0