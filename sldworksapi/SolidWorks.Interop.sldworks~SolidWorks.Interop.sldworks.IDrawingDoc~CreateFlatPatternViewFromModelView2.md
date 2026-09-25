<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~CreateFlatPatternViewFromModelView2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateFlatPatternViewFromModelView2 Method (IDrawingDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html) : CreateFlatPatternViewFromModelView2 Method (IDrawingDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ModelName*
:   Name of model

*ConfigName*
:   Name of configuration

*LocX*
:   X coordinate

*LocY*
:   Y coordinate

*LocZ*
:   Z coordinate

*HideBendLines*
:   True hides bend lines, false does not

Obsolete. Superseded by [IDrawingDoc::CreateFlatPatternViewFromModelView3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDrawingDoc~CreateFlatPatternViewFromModelView3.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateFlatPatternViewFromModelView2( _    ByVal ModelName As System.String, _    ByVal ConfigName As System.String, _    ByVal LocX As System.Double, _    ByVal LocY As System.Double, _    ByVal LocZ As System.Double, _    ByVal HideBendLines As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDrawingDoc Dim ModelName As System.String Dim ConfigName As System.String Dim LocX As System.Double Dim LocY As System.Double Dim LocZ As System.Double Dim HideBendLines As System.Boolean Dim value As System.Boolean   value = instance.CreateFlatPatternViewFromModelView2(ModelName, ConfigName, LocX, LocY, LocZ, HideBendLines) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool CreateFlatPatternViewFromModelView2(     System.string ModelName,    System.string ConfigName,    System.double LocX,    System.double LocY,    System.double LocZ,    System.bool HideBendLines ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool CreateFlatPatternViewFromModelView2(  &   System.String^ ModelName, &   System.String^ ConfigName, &   System.double LocX, &   System.double LocY, &   System.double LocZ, &   System.bool HideBendLines ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ModelName*
:   Name of model

*ConfigName*
:   Name of configuration

*LocX*
:   X coordinate

*LocY*
:   Y coordinate

*LocZ*
:   Z coordinate

*HideBendLines*
:   True hides bend lines, false does not

#### Return Value

True if the flat-pattern view was created successfully, false if it was not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DrawingDoc::CreateFlatPatternViewFromModelView2.

# ![](dotnetimages/collapse.gif)See Also

####

[IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html)

[IDrawingDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc_members.html)

[IDrawingDoc::ChangeRefConfigurationOfFlatPatternView Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~ChangeRefConfigurationOfFlatPatternView.html)

[IDrawingDoc::CreateDrawViewFromModelView3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~CreateDrawViewFromModelView3.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus SP2, Revision Number 10.2