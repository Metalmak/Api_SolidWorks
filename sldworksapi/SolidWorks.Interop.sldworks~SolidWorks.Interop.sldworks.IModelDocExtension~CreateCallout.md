<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~CreateCallout.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateCallout Method (IModelDocExtension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : CreateCallout Method (IModelDocExtension) |

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

*Handler*
:   Pointer to the event handler for the callout (ISwCalloutHandler)

Creates a callout independent of a selection.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateCallout( _    ByVal NumberOfRows As System.Integer, _    ByVal Handler As System.Object _ ) As Callout ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim NumberOfRows As System.Integer Dim Handler As System.Object Dim value As Callout   value = instance.CreateCallout(NumberOfRows, Handler) ``` | |

| C# |  |
| --- | --- |
| ``` Callout CreateCallout(     System.int NumberOfRows,    System.object Handler ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Callout^ CreateCallout(  &   System.int NumberOfRows, &   System.Object^ Handler ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*NumberOfRows*
:   Number of rows in the callout

*Handler*
:   Pointer to the event handler for the callout (ISwCalloutHandler)

#### Return Value

[Callout](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICallout.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::CreateCallout.

# ![](dotnetimages/collapse.gif)Example

[Create a Callout Independent of a Selection (VB.NET)](Create_a_Callout_Independent_of_a_Selection_Example_VBNET.htm)

[Create a Callout Independent of a Selection (VBA)](Create_a_Callout_Independent_of_a_Selection_Example_VB.htm)

[Create a Callout Independent of a Selection (C#)](Create_a_Callout_Independent_of_a_Selection_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method allows you to create a callout independently of a selection. You can define the position of the callout using the [ICallout::Position](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICallout~Position.html) and [ICallout::SetTargetPoint](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICallout~SetTargetPoint.html).

To create a callout dependent on a selection, use [ISelectionMgr::CreateCallout2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISelectionMgr~CreateCallout2.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 FCS, Revision Number 17.0