<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorCustomReference5.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| IEdmEnumeratorCustomReference5 Interface | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorCustomReference5_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : IEdmEnumeratorCustomReference5 Interface |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Allows you to access custom file references.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Interface IEdmEnumeratorCustomReference5 ``` | |

| C# |  |
| --- | --- |
| ``` public interface IEdmEnumeratorCustomReference5 ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IEdmEnumeratorCustomReference5 ``` | |

# ![](dotnetimages/collapse.gif)Example

[Access Custom File References (VB.NET)](Access_Custom_File_References_Example_VBNET.htm)

[Access Custom File References (C#)](Access_Custom_File_References_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This interface:

* inherits from IDispatch. See [IDispatch Interface (Automation)](http://msdn.microsoft.com/en-us/library/windows/desktop/ms221608%28v%3Dvs.85%29.aspx).* is extended by [IEdmEnumeratorCustomReference6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorCustomReference6.html) which adds the ability to specify or get the number of times that a file is referenced by this file.

To use this interface:

1. Get the file to which you want to add references from the vault using [IEdmVault5::GetFileFromPath](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~GetFileFromPath.html).- Cast the [IEdmFile5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5.html) object returned in step 1 to IEdmEnumeratorCustomReference5.- Get a pointer to the file reference using IEdmVault5::GetFileFromPath.- Call [IEdmEnumeratorCustomReference::AddReference](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorCustomReference5~AddReference.html) to add the file reference in step 3 to the file in step 1.

In the SOLIDWORKS PDM Professional user interface, you handle file references in the Contains page of the Properties dialog box. Using the API, you can perform the same file reference tasks that you do in the user interface, for example, adding, removing, and viewing file references. File references can be checked in like any other file in SOLIDWORKS PDM Professional.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmEnumeratorCustomReference5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorCustomReference5_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)