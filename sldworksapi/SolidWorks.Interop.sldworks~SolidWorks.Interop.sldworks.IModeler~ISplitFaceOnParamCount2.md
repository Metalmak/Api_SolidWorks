<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~ISplitFaceOnParamCount2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ISplitFaceOnParamCount2 Method (IModeler) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html) : ISplitFaceOnParamCount2 Method (IModeler) |

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
:   Position along the parametric axis at which the split will be performed

*Status*
:   True if the operation was successful, false if not

Sets up and counts the number of new faces split on the U or V parameter.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ISplitFaceOnParamCount2( _    ByVal Facedisp As Face2, _    ByVal UVFlag As System.Integer, _    ByVal Parameter As System.Double, _    ByRef Status As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModeler Dim Facedisp As Face2 Dim UVFlag As System.Integer Dim Parameter As System.Double Dim Status As System.Boolean Dim value As System.Integer   value = instance.ISplitFaceOnParamCount2(Facedisp, UVFlag, Parameter, Status) ``` | |

| C# |  |
| --- | --- |
| ``` System.int ISplitFaceOnParamCount2(     Face2 Facedisp,    System.int UVFlag,    System.double Parameter,    out System.bool Status ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int ISplitFaceOnParamCount2(  &   Face2^ Facedisp, &   System.int UVFlag, &   System.double Parameter, &   [Out] System.bool Status ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Facedisp*
:   [Face](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) to split

*UVFlag*
:   Parametric axis; either swSplitFaceOnParamU or swSplitFaceOnParamV

*Parameter*
:   Position along the parametric axis at which the split will be performed

*Status*
:   True if the operation was successful, false if not

#### Return Value

Number of new faces

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Modeler::ISplitFaceOnParamCount2.

# ![](dotnetimages/collapse.gif)Remarks

The split is defined by calling this method. Then, you can retrieve the list of new faces by using [IModeler::ISplitFaceOnParam2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModeler~ISplitFaceOnParam2.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html)

[IModeler Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler_members.html)

[IModeler::SplitFaceOnParam Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~SplitFaceOnParam.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0