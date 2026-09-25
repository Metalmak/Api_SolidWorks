<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBom.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| IEdmBom Interface | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBom_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : IEdmBom Interface |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Allows you to access a Bill of Materials (BOM).

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Interface IEdmBom     Inherits IEdmObject5  ``` | |

| C# |  |
| --- | --- |
| ``` public interface IEdmBom : IEdmObject5  ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IEdmBom : public IEdmObject5  ``` | |

# ![](dotnetimages/collapse.gif)Example

[Access Bill of Materials (VB.NET)](Access_Bill_of_Materials_Example_VBNET.htm)

[Access Bill of Materials (C#)](Access_Bill_of_Materials_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This interface inherits from [IEdmObject5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmObject5.html).

To access this interface:

1. Call IEdmVault5::GetObject with eType = [EdmObjectType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmObjectType.html).EdmObject\_BOM.

      - or -

1. Create an [EdmObjectInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmObjectInfo.html) structure with meType = EdmObjectType.EdmObject\_BOM.- Call IEdmVault9::GetObjects with ppoObjects set to the EdmObjectInfo structure created in step 1.

# ![](dotnetimages/collapse.gif)Accessors

[IEdmVault5::GetObject](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~GetObject.html)

[IEdmVault9::GetObjects](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault9~GetObjects.html)

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBom Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBom_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

[IEdmFile7::GetDerivedBOMs Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile7~GetDerivedBOMs.html)