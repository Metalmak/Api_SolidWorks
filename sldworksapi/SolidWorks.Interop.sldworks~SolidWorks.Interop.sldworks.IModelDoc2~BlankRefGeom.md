<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~BlankRefGeom.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| BlankRefGeom Method (IModelDoc2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : BlankRefGeom Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Hides the selected reference geometry in the graphics window.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub BlankRefGeom() ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2   instance.BlankRefGeom() ``` | |

| C# |  |
| --- | --- |
| ``` void BlankRefGeom() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void BlankRefGeom(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::BlankRefGeom.

# ![](dotnetimages/collapse.gif)Example

[Create Replace Face Feature (C#)](Replace_Face_Example_CSharp.htm)

[Create Replace Face Feature (VB.NET)](Replace_Face_Example_VBNET.htm)

[Create Replace Face Feature (VBA)](Replace_Face_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

If you select a reference plane and then call this method, the plane is invisible in the graphics area. This method has the same effect as right-clicking an item and selecting **Hide** on the shortcut menu.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

[IModelDoc2::UnBlankRefGeom Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~UnBlankRefGeom.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0