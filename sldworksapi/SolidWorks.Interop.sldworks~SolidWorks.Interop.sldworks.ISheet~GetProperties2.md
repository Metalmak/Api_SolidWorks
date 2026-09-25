<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet~GetProperties2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetProperties2 Method (ISheet) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISheet Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet.html) : GetProperties2 Method (ISheet) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the properties for this sheet.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetProperties2() As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISheet Dim value As System.Object   value = instance.GetProperties2() ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetProperties2() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetProperties2(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

Array of doubles (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Sheet::GetProperties2.

# ![](dotnetimages/collapse.gif)Example

[Set Drawing Sheet Properties (C#)](Set_Drawing_Sheet_Properties_Example_CSharp.htm)

[Set Drawing Sheet Properties (VB.NET)](Set_Drawing_Sheet_Properties_Example_VBNET.htm)

[Set Drawing Sheet Properties (VBA)](Set_Drawing_Sheet_Properties_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

The return value is the following array of eight doubles:

[ paperSize, templateIn, scale1, scale2, firstAngle, width, height, sameCustomProp ]

where:

paperSize = Paper size; this value is a long or integer packed into a double and is represented by the swDwgPaperSizes\_e enumeration

templateIn = Template index; this value is a long or integer packed into a double and is represented by the swDwgTemplates\_e enumeration

scale1 = Scale numerator

scale2 = Scale denominator

firstAngle = Value is a boolean packed into a double and returns true if the sheet is using first angle projection; false if not

width = Paper width

height = Paper height

*sameCustomProp* = Value is a boolean packed into a double and returns true if the **Same as sheet specified in Document Properties** in the Sheet Properties dialog is selected, false if not

NOTES:

* To ensure a correct return value, open the document as read-write or read-only. Insufficient information is available if you open the document as view-only.

  * You can also use [ISheet::GetSize](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISheet~GetSize.html) to get the size of the sheet and the standard sheet size.

# ![](dotnetimages/collapse.gif)See Also

####

[ISheet Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet.html)

[ISheet Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet_members.html)

[ISheet::SetProperties2 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet~SetProperties2.html)

[ISheet::PageSetup Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet~PageSetup.html)

[ISheet::GetSize Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet~GetSize.html)

[ISheet::SetSize Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet~SetSize.html)

[ISheet::GetTemplateName Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet~GetTemplateName.html)

[ISheet::SetTemplateName Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet~SetTemplateName.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2016 FCS, Revision Number 24.0