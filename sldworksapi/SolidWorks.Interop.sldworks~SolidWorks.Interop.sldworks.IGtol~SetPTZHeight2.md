<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol~SetPTZHeight2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetPTZHeight2 Method (IGtol) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IGtol Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol.html) : SetPTZHeight2 Method (IGtol) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FrameNumber*
:   Frame number

*TolNumber*
:   Tolerance number

*PtzDisplay*
:   True to display the projected zone tolerance, false to not

*PtzHt*
:   Height of the projected tolerance zone

Sets the projected tolerance zone for the specified frame and tolerance in this GTol.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetPTZHeight2( _    ByVal FrameNumber As System.Integer, _    ByVal TolNumber As System.Integer, _    ByVal PtzDisplay As System.Boolean, _    ByVal PtzHt As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IGtol Dim FrameNumber As System.Integer Dim TolNumber As System.Integer Dim PtzDisplay As System.Boolean Dim PtzHt As System.String Dim value As System.Boolean   value = instance.SetPTZHeight2(FrameNumber, TolNumber, PtzDisplay, PtzHt) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetPTZHeight2(     System.int FrameNumber,    System.int TolNumber,    System.bool PtzDisplay,    System.string PtzHt ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetPTZHeight2(  &   System.int FrameNumber, &   System.int TolNumber, &   System.bool PtzDisplay, &   System.String^ PtzHt ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FrameNumber*
:   Frame number

*TolNumber*
:   Tolerance number

*PtzDisplay*
:   True to display the projected zone tolerance, false to not

*PtzHt*
:   Height of the projected tolerance zone

#### Return Value

True if this method executed successfully, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Gtol::SetPTZHeight2.

# ![](dotnetimages/collapse.gif)Example

[Insert GTol (C#)](Insert_GTol_Example_CSharp.htm)

[Insert GTol (VB.NET)](Insert_GTol_Example_VBNET.htm)

[Insert GTol (VBA)](Insert_GTol_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

The projected tolerance zone (PTZ) displays in the first tolerance window of the first control frame of the GTol. If PtzHt is not empty, its value is displayed after the PTZ symbol, which is a P enclosed in a circle.

# ![](dotnetimages/collapse.gif)See Also

####

[IGtol Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol.html)

[IGtol Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol_members.html)

[IGtol::GetPTZHeight2 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol~GetPTZHeight2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2017 FCS, Revision Number 25.0