<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~AddComponent2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddComponent2 Method (IAssemblyDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html) : AddComponent2 Method (IAssemblyDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*CompName*

*X*

*Y*

*Z*

Obsolete. Superseded by [IAssemblyDoc::AddComponent4](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAssemblyDoc~AddComponent4.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddComponent2( _    ByVal CompName As System.String, _    ByVal X As System.Double, _    ByVal Y As System.Double, _    ByVal Z As System.Double _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAssemblyDoc Dim CompName As System.String Dim X As System.Double Dim Y As System.Double Dim Z As System.Double Dim value As System.Object   value = instance.AddComponent2(CompName, X, Y, Z) ``` | |

| C# |  |
| --- | --- |
| ``` System.object AddComponent2(     System.string CompName,    System.double X,    System.double Y,    System.double Z ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ AddComponent2(  &   System.String^ CompName, &   System.double X, &   System.double Y, &   System.double Z ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*CompName*

*X*

*Y*

*Z*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AssemblyDoc::AddComponent2.

# ![](dotnetimages/collapse.gif)See Also

####

[IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html)

[IAssemblyDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc_members.html)