<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc~CreateLineDB.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateLineDB Method (IModelDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html) : CreateLineDB Method (IModelDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Sx*

*Sy*

*Sz*

*Ex*

*Ey*

*Ez*

Obsolete. Superseded by [IModelDoc2::CreateLineDB](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~CreateLineDB.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateLineDB( _    ByVal Sx As System.Double, _    ByVal Sy As System.Double, _    ByVal Sz As System.Double, _    ByVal Ex As System.Double, _    ByVal Ey As System.Double, _    ByVal Ez As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc Dim Sx As System.Double Dim Sy As System.Double Dim Sz As System.Double Dim Ex As System.Double Dim Ey As System.Double Dim Ez As System.Double Dim value As System.Boolean   value = instance.CreateLineDB(Sx, Sy, Sz, Ex, Ey, Ez) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool CreateLineDB(     System.double Sx,    System.double Sy,    System.double Sz,    System.double Ex,    System.double Ey,    System.double Ez ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool CreateLineDB(  &   System.double Sx, &   System.double Sy, &   System.double Sz, &   System.double Ex, &   System.double Ey, &   System.double Ez ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Sx*

*Sy*

*Sz*

*Ex*

*Ey*

*Ez*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc::CreateLineDB.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html)

[IModelDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc_members.html)