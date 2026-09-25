<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISelectionMgr~SelectionColor.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SelectionColor Property (ISelectionMgr) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISelectionMgr Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISelectionMgr.html) : SelectionColor Property (ISelectionMgr) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Mark*
:   Mark value (see **Remarks**)

Gets or sets the selection color.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property SelectionColor( _    ByVal Mark As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISelectionMgr Dim Mark As System.Integer Dim value As System.Integer   instance.SelectionColor(Mark) = value   value = instance.SelectionColor(Mark) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SelectionColor(     System.int Mark ) {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int SelectionColor {    System.int get(System.int Mark);    void set (System.int Mark, System.int value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Mark*
:   Mark value (see **Remarks**)

#### Property Value

Value indicating the color to use for a selection as defined by swSystemColors; these values are from swUserPreferenceIntegerValue\_e  (see Remarks)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SelectionMgr::SelectionColor.

# ![](dotnetimages/collapse.gif)Remarks

You should have a set of marks that you want to apply to selected objects. These marks are application specific and should be designed to present to the user a visual collection of like objects.

The values that SOLIDWORKS internal dialogs typically use for selection colors are:

* swSystemColorsSelectedItem1

  * swSystemColorsSelectedItem2

    * swSystemColorsSelectedItem3

You can also specify any of the following values:

* swSystemColorsViewportBackground

  * swSystemColorsTopGradientColor

    * swSystemColorsBottomGradientColor

      * swSystemColorsDynamicHighlight

        * swSystemColorsHighlight

          * swSystemColorsSelectedFaceShaded

            * swSystemColorsDrawingsVisibleModelEdge

              * swSystemColorsDrawingsHiddenModelEdge

# ![](dotnetimages/collapse.gif)See Also

####

[ISelectionMgr Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISelectionMgr.html)

[ISelectionMgr Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISelectionMgr_members.html)

[ISelectionMgr::ClearSelectionColors Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISelectionMgr~ClearSelectionColors.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2005 FCS, Revision Number 13.0