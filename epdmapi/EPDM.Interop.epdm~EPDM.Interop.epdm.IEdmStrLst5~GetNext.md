<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmStrLst5~GetNext.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetNext Method (IEdmStrLst5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmStrLst5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmStrLst5.html) : GetNext Method (IEdmStrLst5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poPos*
:   [IEdmPos5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html); position of the next string in this list (see **Remarks**)

Gets the next string in this list.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetNext( _    ByVal poPos As IEdmPos5 _ ) As System.String ``` | |

| C# |  |
| --- | --- |
| ``` System.string GetNext(     IEdmPos5 poPos ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.String^ GetNext(  &   IEdmPos5^ poPos ) ``` | |

#### Parameters

*poPos*
:   [IEdmPos5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html); position of the next string in this list (see **Remarks**)

#### Return Value

Next string in this list

# ![](dotnetimages/collapse.gif)Example

See the [IEdmStrLst5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmStrLst5.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method the first time, you must populate poPosition with the interface to the position of the first string, IEdmPos5. Call [IEdmStrLst5::GetHeadPosition](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmStrLst5~GetHeadPosition.html) to start an enumeration and obtain IEdmPos5.

After calling this method the first time, poPos is automatically incremented every time it is called. Call this method repeatedly to obtain the rest of the strings.

Be sure to call [IEdmPos5::IsNull](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5~IsNull.html) before you call this method to ensure you have not reached the end of the enumeration.

C++ programmers must free the returned pointer with a call to SysFreeString.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* E\_EDM\_END\_OF\_LIST: You have gone past the end of the list.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmStrLst5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmStrLst5.html)

[IEdmStrLst5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmStrLst5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2