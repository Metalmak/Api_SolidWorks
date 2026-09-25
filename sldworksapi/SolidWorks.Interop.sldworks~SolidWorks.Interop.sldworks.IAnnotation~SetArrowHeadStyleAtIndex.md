<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation~SetArrowHeadStyleAtIndex.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetArrowHeadStyleAtIndex Method (IAnnotation) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation.html) : SetArrowHeadStyleAtIndex Method (IAnnotation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Index*
:   0-based index of leader within this annotation (see **Remarks**)

*ArrowHeadStyle*
:   Arrowhead style as defined in swArrowStyle\_e

Sets the arrow head style of a specific leader on this annotation.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetArrowHeadStyleAtIndex( _    ByVal Index As System.Integer, _    ByVal ArrowHeadStyle As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAnnotation Dim Index As System.Integer Dim ArrowHeadStyle As System.Integer Dim value As System.Integer   value = instance.SetArrowHeadStyleAtIndex(Index, ArrowHeadStyle) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetArrowHeadStyleAtIndex(     System.int Index,    System.int ArrowHeadStyle ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetArrowHeadStyleAtIndex(  &   System.int Index, &   System.int ArrowHeadStyle ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Index*
:   0-based index of leader within this annotation (see **Remarks**)

*ArrowHeadStyle*
:   Arrowhead style as defined in swArrowStyle\_e

#### Return Value

Return status (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Annotation::SetArrowHeadStyleAtIndex.

# ![](dotnetimages/collapse.gif)Remarks

A valid index value is greater than or equal to 0, but less than the number of leaders on this annotation. Use [IAnnotation::GetArrowHeadCount](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAnnotation~GetArrowHeadCount.html) to find out how many leaders are on this annotation. An index value of -1 is also valid, and indicates that this arrowhead style should be applied to all leaders on this annotation. If the index value is
invalid, SOLIDWORKS returns a retval of -2.

If smart arrowhead style is enabled on this annotation, then this method cannot change
the arrowhead style of individual leaders, and retval is -3. Use [IAnnotation::GetSmartArrowHeadStyle](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAnnotation~GetSmartArrowHeadStyle.html) to determine if this flag is enabled or disabled.

The return status of this method can have the following values:

|  |  |
| --- | --- |
| **If value equals...** | **Then the arrowhead style was...** |
| 0 | Successfully set |
| -1 | Not set because of an unknown error |
| -2 | Not set because of an invalid index value |
| -3 | Not set because of smart arrowhead styles being enabled |
| -4 | Not set because of an invalid arrowhead style value |

If leader display is enabled, then this method changes the visible model. To see those
changes, use [IModelDoc2::GraphicsRedraw2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~GraphicsRedraw2.html) to reddraw the graphics window.

Use [IAnnotation::GetArrowHeadStyleAtIndex](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAnnotation~GetArrowHeadStyleAtIndex.html) to get the arrow head style of a specific leader.

# ![](dotnetimages/collapse.gif)See Also

####

[IAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation.html)

[IAnnotation Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation_members.html)

[IAnnotation::SetArrowHeadSizeAtIndex Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation~SetArrowHeadSizeAtIndex.html)

[IAnnotation::GetArrowHeadSizeAtIndex Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation~GetArrowHeadSizeAtIndex.html)

[IAnnotation::GetArrowHeadStyleAtIndex Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation~GetArrowHeadStyleAtIndex.html)

[IAnnotation::GetArrowHeadCount Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation~GetArrowHeadCount.html)