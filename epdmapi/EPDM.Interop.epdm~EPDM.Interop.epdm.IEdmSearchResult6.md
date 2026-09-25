<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearchResult6.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| IEdmSearchResult6 Interface | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearchResult6_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : IEdmSearchResult6 Interface |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Allows you to access a search result.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Interface IEdmSearchResult6     Inherits IEdmObject5, IEdmSearchResult5  ``` | |

| C# |  |
| --- | --- |
| ``` public interface IEdmSearchResult6 : IEdmObject5, IEdmSearchResult5  ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IEdmSearchResult6 : public IEdmObject5, IEdmSearchResult5  ``` | |

# ![](dotnetimages/collapse.gif)Example

See the [IEdmSearch10](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch10.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

This interface extends [IEdmSearchResult5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearchResult5.html).

To use this interface:

1. Call [IEdmSearch10::GetFirstFavoriteResult](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch10~GetFirstFavoriteResult.html), specifying a favorite search name and whether to get search result custom column information.- Determine the type of the search result returned in step 1 by inspecting [ObjectType](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmObject5~ObjectType.html). (Becaue IEdmSearchResult5 inherits from IEdmObject5, you can simply call IEdmSearchResult5::ObjectType.)- If the type of this search result is an:
       1. [EdmObjectType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmObjectType.html).EdmObject\_File, cast the search result object to [IEdmFile5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5.html).- EdmObjectType.EdmObject\_Folder, cast the search result object to [IEdmFolder5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5.html).- Cast the search result object obtained in step 1 to an IEdmSearchResult6 object. Call [IEdmSearchResult6::GetCustomColumnsInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearchResult6~GetCustomColumnsInfo.html) and [IEdmSearchResult6::GetCustomColumnValues](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearchResult6~GetCustomColumnValues.html) to obtain custom column information for the search result listing.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmSearchResult6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearchResult6_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)