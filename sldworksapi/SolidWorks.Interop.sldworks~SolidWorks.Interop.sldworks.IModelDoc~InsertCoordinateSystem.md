<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc~InsertCoordinateSystem.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertCoordinateSystem Method (IModelDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html) : InsertCoordinateSystem Method (IModelDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*XFlippedIn*

*YFlippedIn*

*ZFlippedIn*

Obsolete. Superseded by [IModelDoc2::InsertCoordinateSystem](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~InsertCoordinateSystem.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertCoordinateSystem( _    ByVal XFlippedIn As System.Boolean, _    ByVal YFlippedIn As System.Boolean, _    ByVal ZFlippedIn As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc Dim XFlippedIn As System.Boolean Dim YFlippedIn As System.Boolean Dim ZFlippedIn As System.Boolean Dim value As System.Boolean   value = instance.InsertCoordinateSystem(XFlippedIn, YFlippedIn, ZFlippedIn) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool InsertCoordinateSystem(     System.bool XFlippedIn,    System.bool YFlippedIn,    System.bool ZFlippedIn ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool InsertCoordinateSystem(  &   System.bool XFlippedIn, &   System.bool YFlippedIn, &   System.bool ZFlippedIn ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*XFlippedIn*

*YFlippedIn*

*ZFlippedIn*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc::InsertCoordinateSystem.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html)

[IModelDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc_members.html)