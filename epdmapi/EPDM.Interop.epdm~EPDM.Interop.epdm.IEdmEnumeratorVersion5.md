<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVersion5.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| IEdmEnumeratorVersion5 Interface | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVersion5_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : IEdmEnumeratorVersion5 Interface |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Allows you to access the versions and revisions of a file.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Interface IEdmEnumeratorVersion5 ``` | |

| C# |  |
| --- | --- |
| ``` public interface IEdmEnumeratorVersion5 ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IEdmEnumeratorVersion5 ``` | |

# ![](dotnetimages/collapse.gif)Example

[Get File Version Information (C#)](Get_File_Version_Information_Example_CSharp.htm)

[Get File Version Information (VB.NET)](Get_File_Version_Information_Example_VBNET.htm)

[Get Revision Names for Local Version of File (C#)](Get_Revision_Names_for_Local_Version_of_File_Example_CSharp.htm)

[Get Revision Names for Local Version of File (VB.NET)](Get_Revision_Names_for_Local_Version_of_File_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

This interface inherits from IDispatch. See [IDispatch Interface (Automation)](http://msdn.microsoft.com/en-us/library/windows/desktop/ms221608%28v%3Dvs.85%29.aspx).

To access this interface, cast an [IEdmFile5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5.html) object to this interface.

A new version of a file is created every time the file has been modified and checked in. Versions are denoted by numbers (1,2,3,..,N). In addition to versions, users can also set up revisions. Revisions are user-friendly names that can be set on versions of files.

This interface is extended by [IEdmEnumeratorVersion6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVersion6.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmEnumeratorVersion5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVersion5_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)