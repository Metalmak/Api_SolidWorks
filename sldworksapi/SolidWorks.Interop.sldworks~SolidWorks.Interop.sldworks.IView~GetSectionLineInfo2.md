<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetSectionLineInfo2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetSectionLineInfo2 Method (IView) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html) : GetSectionLineInfo2 Method (IView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets all of the information about the section lines in the view.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetSectionLineInfo2() As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IView Dim value As System.Object   value = instance.GetSectionLineInfo2() ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetSectionLineInfo2() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetSectionLineInfo2(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

Array of doubles (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See View::GetSectionLineInfo2.

# ![](dotnetimages/collapse.gif)Remarks

This method gets all of the information on section lines in the view. Before using this method, you can use [IView::GetSectionLineCount2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~GetSectionLineCount2.html) to determine the size of the data being returned.

The return value is the following array of doubles:

[ numSectionLines, layer, [ numSegments, [ lineType, startPt[3], endPt[3] ], arrowStart1[3], arrowEnd1[3], arrowWidth1, arrowHeight1, arrowStyle1, arrowStart2[3], arrowEnd2[3], arrowWidth2, arrowHeight2, arrowStyle2, textPt1[3], textPt2[3], textHeight ] ]

where:

numSectionLines  = number of section lines in this view. See also [IView::GetSectionLineCount2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~GetSectionLineCount2.html).

layer = layer information.

The following set of data repeats itself for each section line in the view. The number of times the information is given is numSectionLines:

numSegments = number of line segments in this section line

The following three variables repeat themselves for each segment in the current section line. The number of times the information is given is numSegments:

lineType  = linetype for this line segment. See swLineTypes\_e.

startPt[3]  = X,Y,Z start point for the current segment of this section line.

endPt[3]  = X,Y,Z end point for the current segment of this section line.

arrowStart1[3]  = X,Y,Z start point for arrow head 1 on this section line.

arrowEnd1[3]  = X,Y,Z end point for arrow head 1 on this section line.

arrowWidth1  = width of arrow 1 on this section line.

arrowHeight1  = height of arrow 1 on this section line.

arrowStyle1  = style of arrow 1 on this section line.

arrowStart2[3]  = X,Y,Z start point for arrow head 2 on this section line.

arrowEnd2[3]  = X,Y,Z end point for arrow head 2 on this section line.

arrowWidth2  = width of arrow 2 on this section line.

arrowHeight2  = height of arrow 2 on this section line.

arrowStyle2  = style of arrow 2 on this section line.

textPt1[3]  = X,Y,Z point for the text location near arrow 1.

textPt2[3]  = X,Y,Z point for the text location near arrow 2.

textHeight  = text height in meters.

To get the actual text value, use [IView::GetSectionLineStrings](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~GetSectionLineStrings.html) or [IView::IGetSectionLineStrings](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~IGetSectionLineStrings.html).

The number of line segments, line segment geometry, and line type returned depend on the drawing's display standard.

# ![](dotnetimages/collapse.gif)See Also

####

[IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html)

[IView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView_members.html)

[IView::IGetSectionLineInfo2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~IGetSectionLineInfo2.html)

[IView::IGetSection Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~IGetSection.html)

[IView::IGetSectionLines Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~IGetSectionLines.html)

[IView::GetSection Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetSection.html)

[IView::GetSectionLines Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetSectionLines.html)

[IView::EnumSectionLines Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~EnumSectionLines.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2003 FCS, Revision Number 11.0