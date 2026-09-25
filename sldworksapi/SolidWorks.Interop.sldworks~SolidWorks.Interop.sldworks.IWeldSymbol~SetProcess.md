<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IWeldSymbol~SetProcess.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetProcess Method (IWeldSymbol) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IWeldSymbol Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IWeldSymbol.html) : SetProcess Method (IWeldSymbol) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Process*
:   True to set the indication of welding process flag, false to not

*Text*
:   Text related to the indication of welding process

*Reference*
:   True to place a reference box around the process text, false to not

Sets the values related to the indication of welding process for this weld symbol.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetProcess( _    ByVal Process As System.Boolean, _    ByVal Text As System.String, _    ByVal Reference As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IWeldSymbol Dim Process As System.Boolean Dim Text As System.String Dim Reference As System.Boolean Dim value As System.Boolean   value = instance.SetProcess(Process, Text, Reference) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetProcess(     System.bool Process,    System.string Text,    System.bool Reference ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetProcess(  &   System.bool Process, &   System.String^ Text, &   System.bool Reference ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Process*
:   True to set the indication of welding process flag, false to not

*Text*
:   Text related to the indication of welding process

*Reference*
:   True to place a reference box around the process text, false to not

#### Return Value

True if the indication of welding process is set, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See WeldSymbol::SetProcess.

# ![](dotnetimages/collapse.gif)Example

See the [IWeldSymbol](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IWeldSymbol.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

Get:

* Flag that indicates whether the indication of welding process flag is set on this weld symbol using [IWeldSymbol::GetProcess](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IWeldSymbol~GetProcess.html).

* Text related to the indication of welding process using [IWeldSymbol::GetText](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IWeldSymbol~GetText.html).

  * Flag that indicates whether a reference box exists around this text using [IWeldSymbol::GetProcessReference](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IWeldSymbol~GetProcessReference.html).

The text and reference box are visible if Process is true.

# ![](dotnetimages/collapse.gif)See Also

####

[IWeldSymbol Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IWeldSymbol.html)

[IWeldSymbol Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IWeldSymbol_members.html)

[IWeldSymbol::SetText Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IWeldSymbol~SetText.html)

# ![](dotnetimages/collapse.gif)Availability