<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IWeldSymbol~SetText.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetText Method (IWeldSymbol) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IWeldSymbol Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IWeldSymbol.html) : SetText Method (IWeldSymbol) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Top*
:   True to set the text in the portion of the symbol above the horizontal line, false to set the text in the portion of the symbol below the horizontal line

*Left*
:   Text to the left of the weld symbol

*Symbol*
:   Text representing the weld symbol (see **Remarks**)

*Right*
:   Text to the right of the weld symbol

*Stagger*
:   Text to the right of the stagger symbol (see **Remarks**)

*Contour*
:   Contour setting as defined in swWeldSymbolContourTypes\_e (see **Remarks**)

Sets the text and symbols in the upper or lower portion of the weld symbol.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetText( _    ByVal Top As System.Boolean, _    ByVal Left As System.String, _    ByVal Symbol As System.String, _    ByVal Right As System.String, _    ByVal Stagger As System.String, _    ByVal Contour As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IWeldSymbol Dim Top As System.Boolean Dim Left As System.String Dim Symbol As System.String Dim Right As System.String Dim Stagger As System.String Dim Contour As System.Integer Dim value As System.Boolean   value = instance.SetText(Top, Left, Symbol, Right, Stagger, Contour) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetText(     System.bool Top,    System.string Left,    System.string Symbol,    System.string Right,    System.string Stagger,    System.int Contour ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetText(  &   System.bool Top, &   System.String^ Left, &   System.String^ Symbol, &   System.String^ Right, &   System.String^ Stagger, &   System.int Contour ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Top*
:   True to set the text in the portion of the symbol above the horizontal line, false to set the text in the portion of the symbol below the horizontal line

*Left*
:   Text to the left of the weld symbol

*Symbol*
:   Text representing the weld symbol (see **Remarks**)

*Right*
:   Text to the right of the weld symbol

*Stagger*
:   Text to the right of the stagger symbol (see **Remarks**)

*Contour*
:   Contour setting as defined in swWeldSymbolContourTypes\_e (see **Remarks**)

#### Return Value

True if the text and symbols are set, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See WeldSymbol::SetText.

# ![](dotnetimages/collapse.gif)Example

See the [IWeldSymbol](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IWeldSymbol.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

To get the individual pieces of text for a weld symbol, use [IWeldSymbol::GetText](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IWeldSymbol~GetText.html). To get the contour setting for a weld symbol, use [IWeldSymbol::GetContour](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IWeldSymbol~GetContour.html).

The stagger text that is specified is only visible if this option is enabled. See [IWeldSymbol::GetStagger](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IWeldSymbol~GetStagger.html) to see the current setting and [IWeldSymbol::SetStagger](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IWeldSymbol~SetStagger.html) to enable or disable that option.

A list of weld symbol names can be found in the text file **gtol.sym**,, typically installed at **C:\ProgramData\SolidWorks\SolidWorks 20***nn*\**lang**\**english**. Specify Symbol with one of the currently supported ISO weld symbols:

* BUTT

  * BUSQ

    * BUSV

      * BUSB

        * BUSVBR

          * BUSBR

            * BUSU

              * BUSJ

                * BACK

                  * FILL

                    * PLUG

                      * SPOT

                        * SEAM

                          * SEAMC

                            * JSPT

                              * JSM

# ![](dotnetimages/collapse.gif)See Also

####

[IWeldSymbol Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IWeldSymbol.html)

[IWeldSymbol Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IWeldSymbol_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 99, datecode 1999207