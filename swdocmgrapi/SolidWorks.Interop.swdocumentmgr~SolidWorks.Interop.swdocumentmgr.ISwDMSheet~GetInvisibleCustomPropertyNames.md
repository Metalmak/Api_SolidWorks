<!-- source: swdocmgrapi/SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMSheet~GetInvisibleCustomPropertyNames.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Document Manager API Help | Send comments on this topic. |
| GetInvisibleCustomPropertyNames Method (ISwDMSheet) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdocumentmgr Namespace](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr_namespace.html) > [ISwDMSheet Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMSheet.html) : GetInvisibleCustomPropertyNames Method (ISwDMSheet) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the names of this sheet's invisible custom properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetInvisibleCustomPropertyNames() As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwDMSheet Dim value As System.Object   value = instance.GetInvisibleCustomPropertyNames() ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetInvisibleCustomPropertyNames() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetInvisibleCustomPropertyNames(); ``` | |

#### Return Value

Array of strings of the names of the invisible custom properties for this sheet

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwDMSheet::GetInvisibleCustomPropertyNames.

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, call [ISwDMSheet::GetInvisibleCustomPropertyCount](SOLIDWORKS.Interop.swdocumentmgr~SOLIDWORKS.Interop.swdocumentmgr.ISwDMSheet~GetInvisibleCustomPropertyCount.html) to determine the size of the array.

Call this method before calling [ISwDMSheet::GetInvisibleCustomProperty](SOLIDWORKS.Interop.swdocumentmgr~SOLIDWORKS.Interop.swdocumentmgr.ISwDMSheet~GetInvisibleCustomProperty.html) to determine the name of the invisible custom property you want to use with that method.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwDMSheet Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMSheet.html)

[ISwDMSheet Members](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMSheet_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Document Manager API 2009 SP0