<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageSelectionbox~SetSelectionColor.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetSelectionColor Method (IPropertyManagerPageSelectionbox) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPropertyManagerPageSelectionbox Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageSelectionbox.html) : SetSelectionColor Method (IPropertyManagerPageSelectionbox) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Special*
:   True uses a specific color for selections, false does not

*Color*
:   Color to use for selections as defined by the swSystemColors; values from swUserPreferenceIntegerValue\_e  (see **Remarks**)

Sets the color for selections made in this selection box on the PropertyManager page.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetSelectionColor( _    ByVal Special As System.Boolean, _    ByVal Color As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPropertyManagerPageSelectionbox Dim Special As System.Boolean Dim Color As System.Integer Dim value As System.Boolean   value = instance.SetSelectionColor(Special, Color) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetSelectionColor(     System.bool Special,    System.int Color ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetSelectionColor(  &   System.bool Special, &   System.int Color ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Special*
:   True uses a specific color for selections, false does not

*Color*
:   Color to use for selections as defined by the swSystemColors; values from swUserPreferenceIntegerValue\_e  (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PropertyManagerPageSelectionbox::SetSelectionColor.

# ![](dotnetimages/collapse.gif)Remarks

You can only use this method to set properties on the PropertyManager page before it is displayed or while it is closed. See [IPropertyManagerPage2::Show2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPropertyManagerPage2~Show2.html) and [IPropertyManagerPage2::Close](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPropertyManagerPage2~Close.html).

By default, the selection box created uses the default selection color. You can use this method to override that default behavior. When you specify a specific selection color by setting the Special argument to True and specifying a color in the Color argument, the resulting selection box has a narrow color bar next to the selection box that is the same color as any faces selected in the graphics area.

The colors that SOLIDWORKS internal dialogs typically use for selection colors are:

* swSystemColorsSelectedItem1

  * swSystemColorsSelectedItem2

    * swSystemColorsSelectedItem3

Although you should use the typical selection colors for a consistent look-and-feel among your PropertyManager and SOLIDWORKS PropertyManager pages, you can specify any of the following values:

* swSystemColorsViewportBackground

  * swSystemColorsTopGradientColor

    * swSystemColorsBottomGradientColor

      * swSystemColorsDynamicHighlight

        * swSystemColorsHighlight

          * swSystemColorsSelectedFaceShaded

            * swSystemColorsDrawingsVisibleModelEdge

              * swSystemColorsDrawingsHiddenModelEdge

                * swSystemColorsDrawingsPaperBorder

                  * swSystemColorsDrawingsPaperShadow

                    * swSystemColorsImportedDrivingAnnotation

                      * swSystemColorsImportedDrivenAnnotation

                        * swSystemColorsSketchOverDefined

                          * swSystemColorsSketchFullyDefined

                            * swSystemColorsSketchUnderDefined

                              * swSystemColorsSketchInvalidGeometry

                                * swSystemColorsSketchNotSolved

                                  * swSystemColorsGridLinesMinor

                                    * swSystemColorsGridLinesMajor

                                      * swSystemColorsConstructionGeometry

                                        * swSystemColorsDanglingDimension

                                          * swSystemColorsText

                                            * swSystemColorsAssemblyEditPart

                                              * swSystemColorsAssemblyEditPartHiddenLines

                                                * swSystemColorsAssemblyNonEditPart

                                                  * swSystemColorsInactiveEntity

                                                    * swSystemColorsTemporaryGraphics

                                                      * swSystemColorsTemporaryGraphicsShaded

                                                        * swSystemColorsActiveSelectionListBox

                                                          * swSystemColorsSurfacesOpenEdge

                                                            * swSystemColorsTreeViewBackground

                                                              * swSystemColorsShadedEdge

# ![](dotnetimages/collapse.gif)See Also

####

[IPropertyManagerPageSelectionbox Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageSelectionbox.html)

[IPropertyManagerPageSelectionbox Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageSelectionbox_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus SP4, Revision Number 10.4