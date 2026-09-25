<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol~SetAllAroundThisSide.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetAllAroundThisSide Method (IGtol) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IGtol Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol.html) : SetAllAroundThisSide Method (IGtol) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*AllAroundTS*
:   True to use an All Around This Side leader, false to not

Sets whether this GTol uses an All Around This Side leader.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetAllAroundThisSide( _    ByVal AllAroundTS As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IGtol Dim AllAroundTS As System.Boolean   instance.SetAllAroundThisSide(AllAroundTS) ``` | |

| C# |  |
| --- | --- |
| ``` void SetAllAroundThisSide(     System.bool AllAroundTS ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetAllAroundThisSide(  &   System.bool AllAroundTS ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*AllAroundTS*
:   True to use an All Around This Side leader, false to not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Gtol::SetAllAroundThisSide.

# ![](dotnetimages/collapse.gif)Example

'VBA Preconditions:

'Open a drawing.

```
Dim swApp As SldWorks
Dim Part As ModelDoc2
Dim myGtol As Gtol
Dim myAnno As Annotation
Dim boolstatus As Boolean
Dim longstatus As Long
Option Explicit
Sub main()
```

```
    Set swApp = Application.SldWorks
    Set Part = swApp.ActiveDoc

    Set myGtol = Part.InsertGtol()
    If Not myGtol Is Nothing Then
       myGtol.SetFrameSymbols2 1, "<IGTOL-SPROF>", False, "", False, "", "", "", ""
       myGtol.SetFrameValues 1, ".031265", "", "", "", ""
       myGtol.SetFrameSymbols2 2, "", False, "", False, "", "", "", ""
       myGtol.SetFrameValues 2, "", "", "", "", ""
       myGtol.SetPTZHeight "", False
       myGtol.SetCompositeFrame False
       myGtol.SetText 4, ""
       myGtol.SetBetweenTwoPoints False, "", ""
       myGtol.SetAllAroundThisSide True
       Set myAnno = myGtol.GetAnnotation()
       If Not myAnno Is Nothing Then
          boolstatus = myAnno.SetPosition(0.801796955941255, 0.800162656875834, 0)
          longstatus = myAnno.SetLeader3(swLeaderStyle_e.swBENT, 0, True, False, False, False)
       End If
    End If
    Part.WindowRedraw

End Sub
```

# ![](dotnetimages/collapse.gif)Remarks

This property is valid only for bent, perpendicular, and multi-jog leaders. To create bent, perpendicular, and multi-jog leaders, use [IAnnotation::SetLeader3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation~SetLeader3.html).

Use:

* [IGtol::IsAttached](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IGtol~IsAttached.html) to determine whether this symbol is currently using a leader.* [IGtol::HasExtraLeader](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IGtol~HasExtraLeader.html) to determine whether this symbol is using a bent leader.* [IGtol::GetLeaderSide](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IGtol~GetLeaderSide.html) to determine where the leader is attached to the symbol.* [IGtol::SetLeader](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IGtol~SetLeader.html) to set the characteristics of the leader on this symbol.

# ![](dotnetimages/collapse.gif)See Also

####

[IGtol Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol.html)

[IGtol Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol_members.html)

[IGtol::GetAllAroundThisSide Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol~GetAllAroundThisSide.html)

[IGtol::SetAllOverThisSide Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol~SetAllOverThisSide.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2018 FCS, Revision Number 26.0