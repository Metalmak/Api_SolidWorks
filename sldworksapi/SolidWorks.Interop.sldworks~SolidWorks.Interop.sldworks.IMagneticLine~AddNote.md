<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMagneticLine~AddNote.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddNote Method (IMagneticLine) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IMagneticLine Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMagneticLine.html) : AddNote Method (IMagneticLine) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Note*
:   [INote](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.INote.html) to attach to this magnetic line

*Position*
:   0.0 <= Attachment position on magnetic line <= 1.0; valid only if [IMagneticLine::EqualSpacing](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMagneticLine~EqualSpacing.html) is false

Attaches to this magnetic line the specified note at the specified position.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddNote( _    ByVal Note As Note, _    ByVal Position As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMagneticLine Dim Note As Note Dim Position As System.Double Dim value As System.Boolean   value = instance.AddNote(Note, Position) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool AddNote(     Note Note,    System.double Position ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool AddNote(  &   Note^ Note, &   System.double Position ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Note*
:   [INote](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.INote.html) to attach to this magnetic line

*Position*
:   0.0 <= Attachment position on magnetic line <= 1.0; valid only if [IMagneticLine::EqualSpacing](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMagneticLine~EqualSpacing.html) is false

#### Return Value

True if successful, false if not (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See MagneticLine::AddNote.

# ![](dotnetimages/collapse.gif)Example

[Insert Magnetic Line (C#)](Insert_Magnetic_Line_Example_CSharp.htm)

[Insert Magnetic Line (VB.NET)](Insert_Magnetic_Line_Example_VBNET.htm)

[Insert Magnetic Line (VBA)](Insert_Magnetic_Line_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

All notes attached to a magnetic line must be from the same view.

# ![](dotnetimages/collapse.gif)See Also

####

[IMagneticLine Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMagneticLine.html)

[IMagneticLine Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMagneticLine_members.html)

[IMagneticLine::RemoveNote Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMagneticLine~RemoveNote.html)

[IMagneticLine::GetNotes Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMagneticLine~GetNotes.html)

[IMagneticLine::IGetNotes Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMagneticLine~IGetNotes.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2012 FCS, Revision Number 20.0