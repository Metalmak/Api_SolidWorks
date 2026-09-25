<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation~GetArrowHeadSizeAtIndex.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetArrowHeadSizeAtIndex Method (IAnnotation) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation.html) : GetArrowHeadSizeAtIndex Method (IAnnotation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Index*
:   Index of leader on this annotation

*UseDoc*
:   TRUE indicates that the document default setting for arrow head size was used, FALSE
    indicates that the Length, Width, and Height values were specified

*Length*
:   Length of arrow head

*Width*
:   Width of arrow head

*Height*
:   Height of arrow head

Gets the arrow head size of the specified leader on this annotation.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetArrowHeadSizeAtIndex( _    ByVal Index As System.Integer, _    ByRef UseDoc As System.Boolean, _    ByRef Length As System.Double, _    ByRef Width As System.Double, _    ByRef Height As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAnnotation Dim Index As System.Integer Dim UseDoc As System.Boolean Dim Length As System.Double Dim Width As System.Double Dim Height As System.Double Dim value As System.Boolean   value = instance.GetArrowHeadSizeAtIndex(Index, UseDoc, Length, Width, Height) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetArrowHeadSizeAtIndex(     System.int Index,    out System.bool UseDoc,    out System.double Length,    out System.double Width,    out System.double Height ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetArrowHeadSizeAtIndex(  &   System.int Index, &   [Out] System.bool UseDoc, &   [Out] System.double Length, &   [Out] System.double Width, &   [Out] System.double Height ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Index*
:   Index of leader on this annotation

*UseDoc*
:   TRUE indicates that the document default setting for arrow head size was used, FALSE
    indicates that the Length, Width, and Height values were specified

*Length*
:   Length of arrow head

*Width*
:   Width of arrow head

*Height*
:   Height of arrow head

#### Return Value

True if the method succeeds, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Annotation::GetArrowHeadSizeAtIndex.

# ![](dotnetimages/collapse.gif)Remarks

The index value is 0-based. Therefore, a valid index value is greater than or equal to 0, but less than the number of leaders on this annotation. Use [IAnnotation::GetArrowHeadCount](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAnnotation~GetArrowHeadCount.html) to find the number of leaders on this annotation. If the index value is invalid, SOLIDWORKS returns the arrowhead style as -1, and returns an S\_FALSE status (COM interface).

Use [IAnnotation::SetArrowHeadSizeAtIndex](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAnnotation~SetArrowHeadSizeAtIndex.html) to set the arrow head size of a specific leader.

# ![](dotnetimages/collapse.gif)See Also

####

[IAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation.html)

[IAnnotation Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation_members.html)

[IAnnotation::GetArrowHeadStyleAtIndex Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation~GetArrowHeadStyleAtIndex.html)

[IAnnotation::SetArrowHeadStyleAtIndex Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation~SetArrowHeadStyleAtIndex.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 SP1, Revision Number 16.1