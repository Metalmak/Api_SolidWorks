<!-- source: swdocmgrapi/SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMExternalReferenceOption2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Document Manager API Help | Send comments on this topic. |
| ISwDMExternalReferenceOption2 Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMExternalReferenceOption2_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdocumentmgr Namespace](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr_namespace.html) : ISwDMExternalReferenceOption2 Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Allows you to access information about external references from a document.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface ISwDMExternalReferenceOption2     Inherits ISwDMExternalReferenceOption  ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwDMExternalReferenceOption2 ``` | |

| C# |  |
| --- | --- |
| ``` public interface ISwDMExternalReferenceOption2 : ISwDMExternalReferenceOption  ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class ISwDMExternalReferenceOption2 : public ISwDMExternalReferenceOption  ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwDMExternalReferenceOption2.

# ![](dotnetimages/collapse.gif)Example

[Get External References for Part (C#)](Get_External_References_for_Part_Example_CSharp.htm)

[Get External References for Part (VB.NET)](Get_External_References_for_Part_Example_VBNET.htm)

[Get Current Name of Configuration of Suppressed Component (C#)](Get_Current_Name_of_Configuration_of_Suppressed_Component_Example_CSharp.htm)

[Get Current Name of Configuration of Suppressed Component (VB.NET)](Get_Current_Name_of_Configuration_of_Suppressed_Component_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

* You can access an SwDMExternalReferenceOption2 object by calling QueryInterface on an [ISwDMExternalReferenceOption](SOLIDWORKS.Interop.swdocumentmgr~SOLIDWORKS.Interop.swdocumentmgr.ISwDMExternalReferenceOption.html) object in C++ or by direct assignment in Visual Basic.

  * The SwDMExternalReferenceOption object can be assigned to a SwDMExternalReferenceOption2 variable, just like the SOLIDWORKS IModelDoc2 object can be assigned to a SOLIDWORKS IPartDoc variable.

# ![](dotnetimages/collapse.gif)Accessors

[ISwDMApplication4::GetExternalReferenceOptionObject2](SOLIDWORKS.Interop.swdocumentmgr~SOLIDWORKS.Interop.swdocumentmgr.ISwDMApplication4~GetExternalReferenceOptionObject2.html)

# ![](dotnetimages/collapse.gif)See Also

####

[ISwDMExternalReferenceOption2 Members](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMExternalReferenceOption2_members.html)

[SolidWorks.Interop.swdocumentmgr Namespace](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr_namespace.html)

[ISwDMDocument18::GetExternalFeatureReferences2 Method ()](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument18~GetExternalFeatureReferences2.html)