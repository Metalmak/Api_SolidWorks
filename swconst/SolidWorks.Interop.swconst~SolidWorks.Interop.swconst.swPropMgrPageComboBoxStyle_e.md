<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swPropMgrPageComboBoxStyle_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swPropMgrPageComboBoxStyle\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swPropMgrPageComboBoxStyle\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

PropertyManager page combobox styles.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swPropMgrPageComboBoxStyle_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swPropMgrPageComboBoxStyle_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swPropMgrPageComboBoxStyle_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swPropMgrPageComboBoxStyle_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swPropMgrPageComboBoxStyle\_AvoidSelectionText** | 8 or 0x8; The item the user selects in the attached drop-down list does not appear in the combo box. Instead, the user's selection causes the add-in to get a callback via IPropertyManagerPage2Handler4::OnComboboxSelectionChanged. The Id argument is the combo box |
| **swPropMgrPageComboBoxStyle\_EditableText** | 2 or 0x2; Allows editing of the text in the combo box |
| **swPropMgrPageComboBoxStyle\_EditBoxReadOnly** | 4 or 0x4; User can only select a value from the attached drop-down list for the combo box  NOTE: You can set swPropMgrPageComboBoxStyle\_EditBoxReadOnly either before or after the PropertyManager page is displayed. If set after the PropertyManager page is displayed and the box contains editable text, then that text cannot be edited by the user. However, you can use IPropertyManagerPageCombobox::EditText to edit the text in the combo box. |
| **swPropMgrPageComboBoxStyle\_Sorted** | 1 or 0x1; Sort the items in the attached drop-down list of the combo box in alphabetical order |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)