<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~SetVisibleBox.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetVisibleBox Method (IModelDocExtension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : SetVisibleBox Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*UpperLeft*
:   Upper-left [point](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathPoint.html) of the visible bounding box

*LowerRight*
:   Lower-right [point](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathPoint.html) of the visible bounding box

Sets the visible bounding box for Zoom to Fit for a part or an assembly.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetVisibleBox( _    ByVal UpperLeft As MathPoint, _    ByVal LowerRight As MathPoint _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim UpperLeft As MathPoint Dim LowerRight As MathPoint   instance.SetVisibleBox(UpperLeft, LowerRight) ``` | |

| C# |  |
| --- | --- |
| ``` void SetVisibleBox(     MathPoint UpperLeft,    MathPoint LowerRight ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetVisibleBox(  &   MathPoint^ UpperLeft, &   MathPoint^ LowerRight ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*UpperLeft*
:   Upper-left [point](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathPoint.html) of the visible bounding box

*LowerRight*
:   Lower-right [point](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathPoint.html) of the visible bounding box

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::SetVisibleBox.

# ![](dotnetimages/collapse.gif)Example

[Set Visible Bounding Box for Zoom to Fit (C#)](Set_Visible_Bounding_Box_for_Zoom_to_Fit_Example_CSharp.htm)

[Set Visible Bounding Box for Zoom to Fit (C#)](Set_Visible_Bounding_Box_for_Zoom_to_Fit_Example_VBNET.htm)

[Set Visible Bounding Box for Zoom to Fit (VBA)](Set_Visible_Bounding_Box_for_Zoom_to_Fit_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Use:

* [IModelDocExtension::GetVisibleBox](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~GetVisibleBox.html) to get the visible bounding box for a Zoom to Fit operation.

  * [IModelDocExtension::RemoveVisibleBox](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~RemoveVisibleBox.html) to remove the visible bounding box  for a Zoom to Fit operation and to return the size of the bounding box to the size calculated by SOLIDWORKS.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0