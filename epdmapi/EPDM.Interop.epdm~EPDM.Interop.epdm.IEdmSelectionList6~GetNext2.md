<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSelectionList6~GetNext2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetNext2 Method (IEdmSelectionList6) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmSelectionList6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSelectionList6.html) : GetNext2 Method (IEdmSelectionList6) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poPos*
:   [IEdmPos5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html); position of the item to get (see **Remarks**)

*poSel*
:   [EdmSelectionObject](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSelectionObject.html) structure

Gets the next item in this list.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetNext2( _    ByVal poPos As IEdmPos5, _    ByRef poSel As EdmSelectionObject _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetNext2(     IEdmPos5 poPos,    out EdmSelectionObject poSel ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetNext2(  &   IEdmPos5^ poPos, &   [Out] EdmSelectionObject poSel ) ``` | |

#### Parameters

*poPos*
:   [IEdmPos5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html); position of the item to get (see **Remarks**)

*poSel*
:   [EdmSelectionObject](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSelectionObject.html) structure

# ![](dotnetimages/collapse.gif)Example

See the [IEdmSelectionList5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSelectionList5.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method the first time, you must populate poPos with the interface to the position of the first item, IEdmPos5. Call [IEdmSelectionList5::GetHeadPosition](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSelectionList5~GetHeadPosition.html) to obtain IEdmPos5.

After calling this method the first time, poPos is automatically incremented every time it is called. Call this method repeatedly to obtain the rest of the items.

Be sure to call [IEdmPos5::IsNull](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5~IsNull.html) before you call this method to ensure you have not reached the end of the enumeration.

C++ programmers must free the object returned in poSel.

**Note**: Objects added with the now obsolete [IEdmSelectionList5::AddTail](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSelectionList5~AddTail.html) are not completely defined. If you added an object using IEdmSelectionList5::AddTail, the EdmSelectionObject structure returned by this method contains the following:

* The meType member is always [EdmObjectType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmObjectType.html).EdmObject\_File.* The mbsPath member contains only the file name provided as argument to IEdmSelectionList5::AddTail, not the entire path.* The members mlGetVersion, mlLocalVersion, and mlLatestVersion are all -1.

To add completely defined objects to this list, call [IEdmSelectionList6.AddTail2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSelectionList6~AddTail2.html).

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* E\_EDM\_END\_OF\_LIST: You have gone past the end of the list.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmSelectionList6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSelectionList6.html)

[IEdmSelectionList6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSelectionList6_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010