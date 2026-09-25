<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension~SetPrecision.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetPrecision Method (IDisplayDimension) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDisplayDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension.html) : SetPrecision Method (IDisplayDimension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*UseDoc*

*Primary*

*Alternate*

*PrimaryTol*

*AlternateTol*

Obsolete. Superseded by [IDisplayDimension::SetPrecision2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDisplayDimension~SetPrecision2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetPrecision( _    ByVal UseDoc As System.Boolean, _    ByVal Primary As System.Integer, _    ByVal Alternate As System.Integer, _    ByVal PrimaryTol As System.Integer, _    ByVal AlternateTol As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDisplayDimension Dim UseDoc As System.Boolean Dim Primary As System.Integer Dim Alternate As System.Integer Dim PrimaryTol As System.Integer Dim AlternateTol As System.Integer Dim value As System.Integer   value = instance.SetPrecision(UseDoc, Primary, Alternate, PrimaryTol, AlternateTol) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetPrecision(     System.bool UseDoc,    System.int Primary,    System.int Alternate,    System.int PrimaryTol,    System.int AlternateTol ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetPrecision(  &   System.bool UseDoc, &   System.int Primary, &   System.int Alternate, &   System.int PrimaryTol, &   System.int AlternateTol ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*UseDoc*

*Primary*

*Alternate*

*PrimaryTol*

*AlternateTol*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DisplayDimension::SetPrecision.

# ![](dotnetimages/collapse.gif)See Also

####

[IDisplayDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension.html)

[IDisplayDimension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension_members.html)