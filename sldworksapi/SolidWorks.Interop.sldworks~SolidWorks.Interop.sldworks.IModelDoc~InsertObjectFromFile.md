<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc~InsertObjectFromFile.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertObjectFromFile Method (IModelDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html) : InsertObjectFromFile Method (IModelDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FilePath*

*CreateLink*

*Xx*

*Yy*

*Zz*

Obsolete. Superseded by [IModelDoc2::InsertObjectFromFile](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~InsertObjectFromFile.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertObjectFromFile( _    ByVal FilePath As System.String, _    ByVal CreateLink As System.Boolean, _    ByVal Xx As System.Double, _    ByVal Yy As System.Double, _    ByVal Zz As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc Dim FilePath As System.String Dim CreateLink As System.Boolean Dim Xx As System.Double Dim Yy As System.Double Dim Zz As System.Double Dim value As System.Boolean   value = instance.InsertObjectFromFile(FilePath, CreateLink, Xx, Yy, Zz) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool InsertObjectFromFile(     System.string FilePath,    System.bool CreateLink,    System.double Xx,    System.double Yy,    System.double Zz ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool InsertObjectFromFile(  &   System.String^ FilePath, &   System.bool CreateLink, &   System.double Xx, &   System.double Yy, &   System.double Zz ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FilePath*

*CreateLink*

*Xx*

*Yy*

*Zz*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc::InsertObjectFromFile.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html)

[IModelDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc_members.html)