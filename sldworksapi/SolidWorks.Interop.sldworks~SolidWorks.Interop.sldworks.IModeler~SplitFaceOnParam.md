<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~SplitFaceOnParam.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SplitFaceOnParam Method (IModeler) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html) : SplitFaceOnParam Method (IModeler) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Facedisp*
:   [Face](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) to split

*UVFlag*
:   Parametric axis; either swSplitFaceOnParamU or swSplitFaceOnParamV

*Parameter*
:   Position along the parametric axis at which the split is performed

*Status*
:   True if the operation was successful, false if

Splits and retrieves the faces on the U or V parameter

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SplitFaceOnParam( _    ByVal Facedisp As System.Object, _    ByVal UVFlag As System.Integer, _    ByVal Parameter As System.Double, _    ByRef Status As System.Boolean _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModeler Dim Facedisp As System.Object Dim UVFlag As System.Integer Dim Parameter As System.Double Dim Status As System.Boolean Dim value As System.Object   value = instance.SplitFaceOnParam(Facedisp, UVFlag, Parameter, Status) ``` | |

| C# |  |
| --- | --- |
| ``` System.object SplitFaceOnParam(     System.object Facedisp,    System.int UVFlag,    System.double Parameter,    out System.bool Status ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ SplitFaceOnParam(  &   System.Object^ Facedisp, &   System.int UVFlag, &   System.double Parameter, &   [Out] System.bool Status ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Facedisp*
:   [Face](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) to split

*UVFlag*
:   Parametric axis; either swSplitFaceOnParamU or swSplitFaceOnParamV

*Parameter*
:   Position along the parametric axis at which the split is performed

*Status*
:   True if the operation was successful, false if

#### Return Value

Array of new [faces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Modeler::SplitFaceOnParam.

# ![](dotnetimages/collapse.gif)See Also

####

[IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html)

[IModeler Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler_members.html)

[IModeler::ISplitFaceOnParam2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~ISplitFaceOnParam2.html)

[IModeler::ISplitFaceOnParamCount2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~ISplitFaceOnParamCount2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001 FCS, Revision Number 9.0