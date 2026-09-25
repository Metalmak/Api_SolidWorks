<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference6.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| IEdmReference6 Interface | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference6_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : IEdmReference6 Interface |

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
| ``` Public Interface IEdmReference6     Inherits IEdmReference5  ``` | |

| C# |  |
| --- | --- |
| ``` public interface IEdmReference6 : IEdmReference5  ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IEdmReference6 : public IEdmReference5  ``` | |

# ![](dotnetimages/collapse.gif)Remarks

The interface:

* inherits from [IEdmReference5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5.html).* is extended by [IEdmReference7](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference7.html).

Some file types, such as files from AutoCAD, SOLIDWORKS, Microsoft Word, etc., can contain references to other files. Regardless of file type, you can also set up your own references using SOLIDWORKS PDM Professional's User Defined File References dialog box in file properties. SOLIDWORKS PDM Professional manages all of these references for you and they show up, for example, in the check-in dialog box in the form of a reference tree.

Using IEdmReference5, you can enumerate referenced files and referencing files. You can also set up user-defined references using IEdmReference5.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmReference6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference6_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

[IEdmReference8 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference8.html)

[IEdmReference9 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference9.html)