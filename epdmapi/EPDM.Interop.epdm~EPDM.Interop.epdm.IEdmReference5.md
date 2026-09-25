<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| IEdmReference5 Interface | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : IEdmReference5 Interface |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Allows you to enumerate referenced and referencing files and set up user-defined references.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Interface IEdmReference5 ``` | |

| C# |  |
| --- | --- |
| ``` public interface IEdmReference5 ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IEdmReference5 ``` | |

# ![](dotnetimages/collapse.gif)Example

[Get File References for a File (C#)](Get_File_References_for_File_Example_CSharp.htm)

[Get File References for a File (VB.NET)](Get_File_References_for_File_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

The interface:

* inherits from IDispatch. See [IDispatch Interface (Automation)](http://msdn.microsoft.com/en-us/library/windows/desktop/ms221608%28v%3Dvs.85%29.aspx).* is extended by [IEdmReference6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference6.html).

Some file types, such as files from AutoCAD, SOLIDWORKS, Microsoft Word, etc., can contain references to other files. Regardless of file type, you can also set up your own references using SOLIDWORKS PDM Professional's User Defined File References dialog box in file properties. SOLIDWORKS PDM Professional manages all of these references for you and they show up, for example, in the check-in dialog box in the form of a reference tree.

Using IEdmReference5, you can enumerate referenced files and referencing files. You can also set up user-defined references using IEdmReference5.

# ![](dotnetimages/collapse.gif)Accessors

[IEdmFile5::GetReferenceTree](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~GetReferenceTree.html)

[IEdmReference5::GetNextChild](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5~GetNextChild.html)

[IEdmReference5::GetNextParent](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5~GetNextParent.html)

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmReference5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

[IEdmReference7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference7.html)

[IEdmReference8 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference8.html)

[IEdmReference9 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference9.html)