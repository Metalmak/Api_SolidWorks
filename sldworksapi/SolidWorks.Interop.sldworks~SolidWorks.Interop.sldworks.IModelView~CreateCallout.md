<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView~CreateCallout.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateCallout Method (IModelView) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView.html) : CreateCallout Method (IModelView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NumberOfRows*
:   Number of rows in the callout

*LpHandler*
:   Pointer to ISwCalloutHandler

Creates a callout on this model view.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateCallout( _    ByVal NumberOfRows As System.Integer, _    ByVal LpHandler As System.Object _ ) As Callout ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelView Dim NumberOfRows As System.Integer Dim LpHandler As System.Object Dim value As Callout   value = instance.CreateCallout(NumberOfRows, LpHandler) ``` | |

| C# |  |
| --- | --- |
| ``` Callout CreateCallout(     System.int NumberOfRows,    System.object LpHandler ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Callout^ CreateCallout(  &   System.int NumberOfRows, &   System.Object^ LpHandler ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*NumberOfRows*
:   Number of rows in the callout

*LpHandler*
:   Pointer to ISwCalloutHandler

#### Return Value

An [ICallout](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICallout.html) object

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelView::CreateCallout.

# ![](dotnetimages/collapse.gif)Example

[Create a Callout in a Model View (VBA)](Create_Model_View_Callouts_Example_VB.htm)

[Create a Callout in a Model View (VB.NET)](Create_Model_View_Callouts_Example_VBNET.htm)

[Create a Callout in a Model View (C#)](Create_Model_View_Callouts_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IModelView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView.html)

[IModelView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0