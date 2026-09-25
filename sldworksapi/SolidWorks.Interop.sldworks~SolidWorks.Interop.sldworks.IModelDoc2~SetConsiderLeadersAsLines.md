<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~SetConsiderLeadersAsLines.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetConsiderLeadersAsLines Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : SetConsiderLeadersAsLines Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*LeadersAsLines*
:   True to return leaders as line data, false to not

Sets a flag on the document that indicates whether the display data of a leader should be included as lines when the lines are retrieved from a view or annotation in this document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetConsiderLeadersAsLines( _    ByVal LeadersAsLines As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim LeadersAsLines As System.Boolean Dim value As System.Boolean   value = instance.SetConsiderLeadersAsLines(LeadersAsLines) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetConsiderLeadersAsLines(     System.bool LeadersAsLines ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetConsiderLeadersAsLines(  &   System.bool LeadersAsLines ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*LeadersAsLines*
:   True to return leaders as line data, false to not

#### Return Value

Original value of the flag before calling this method

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::SetConsiderLeadersAsLines.

# ![](dotnetimages/collapse.gif)Remarks

The various GetLeaderCount and GetLeaderAtIndex methods that are found on several different annotations return the information about where the vertices of the leader are located. GetLineCount and GetLinesAtIndex also return the leader information as part of its line information. Depending on what your program is trying to accomplish and which methods it is using, this duplication of information may not be desirable. This method controls this behavior by setting a flag on the document that indicates whether or not the leader information is returned as part of the line information or not.

Initially, when a document is opened, the flag is set to True, so that existing applications work as they have always worked. If you do not want to get back leader information as part of the line information, call this method and set the value to false. The flag is not saved with the document, so you must specifically set it to false whenever you do not want leaders as part of the line information.

The various GetArrowHeadCount and GetArrowHeadAtIndex methods are also affected. When this flag has been set to false so that leaders are not considered as lines, the arrowhead information for the arrowheads on those leaders is not returned. However, GetArrowHeadInfo still returns valid information.

Use [IModelDoc2::GetConsiderLeadersAsLines](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~GetConsiderLeadersAsLines.html) to determine the current behavior.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0