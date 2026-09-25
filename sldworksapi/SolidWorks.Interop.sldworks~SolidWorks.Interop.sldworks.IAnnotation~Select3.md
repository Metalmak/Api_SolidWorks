<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation~Select3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Select3 Method (IAnnotation) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation.html) : Select3 Method (IAnnotation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Append*
:   True appends this selection to the current selection list, false replaces the current selection list with this selection

*Data*
:   Pointer to the [ISelectData](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISelectData.html) object

Selects this annotation and marks it.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function Select3( _    ByVal Append As System.Boolean, _    ByVal Data As SelectData _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAnnotation Dim Append As System.Boolean Dim Data As SelectData Dim value As System.Boolean   value = instance.Select3(Append, Data) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool Select3(     System.bool Append,    SelectData Data ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool Select3(  &   System.bool Append, &   SelectData^ Data ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Append*
:   True appends this selection to the current selection list, false replaces the current selection list with this selection

*Data*
:   Pointer to the [ISelectData](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISelectData.html) object

#### Return Value

True if the annotation was selected, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Annotation::Select3.

# ![](dotnetimages/collapse.gif)Example

[Get Corresponding Note in Assembly (VBA)](Get_Corresponding_Note_in_Assembly_Example_VB.htm)

[Get Corresponding Note in Part (VBA)](Get_Corresponding_Note_in_Part_Example_VB.htm)

[Insert Model Annotations (C#)](Insert_Model_Annotations_Example_CSharp.htm)

[Insert Model Annotations (VB.NET)](Insert_Model_Annotations_Example_VBNET.htm)

[Insert Model Annotations (VBA)](Insert_Model_Annotations_Example_VB.htm)

[Select All Center Marks (C#)](Select_All_Center_Marks_Example_CSharp.htm)

[Select All Center Marks (VB.NET)](Select_All_Center_Marks_Example_VBNET.htm)

[Select All Center Marks (VBA)](Select_All_Center_Marks_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation.html)

[IAnnotation Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12