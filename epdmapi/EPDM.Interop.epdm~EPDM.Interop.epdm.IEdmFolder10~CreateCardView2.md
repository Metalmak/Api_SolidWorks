<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder10~CreateCardView2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| CreateCardView2 Method (IEdmFolder10) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFolder10 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder10.html) : CreateCardView2 Method (IEdmFolder10) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lFileID*
:   ID of the file for which to create a data card view; 0 to create a view only for this folder

*lParentWindow*
:   Handle of the window in which to create the data card view

*lX*
:   X coordinate where to place the data card view relative to the upper-left corner of the window

*lY*
:   Y coordinate where to place the data card view relative to the upper-left corner of the window

*poCallback*
:   Optional pointer to a class that implements [IEdmCallback](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback.html) to handle notifications from the data card view (see **Remarks**)

*lEdmCardViewFlags*
:   Appearance and functionality of the data card view as defined in [EmdCardViewFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCardViewFlag.html)

Creates a data card view for the specified file or folder.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function CreateCardView2( _    ByVal lFileID As System.Integer, _    ByVal lParentWindow As System.Integer, _    ByVal lX As System.Integer, _    ByVal lY As System.Integer, _    Optional ByVal poCallback As EdmCallback, _    Optional ByVal lEdmCardViewFlags As System.Integer _ ) As IEdmCardView5 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmCardView5 CreateCardView2(     System.int lFileID,    System.int lParentWindow,    System.int lX,    System.int lY,    EdmCallback poCallback,    System.int lEdmCardViewFlags ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmCardView5^ CreateCardView2(  &   System.int lFileID, &   System.int lParentWindow, &   System.int lX, &   System.int lY, &   EdmCallback^ poCallback, &   System.int lEdmCardViewFlags ) ``` | |

#### Parameters

*lFileID*
:   ID of the file for which to create a data card view; 0 to create a view only for this folder

*lParentWindow*
:   Handle of the window in which to create the data card view

*lX*
:   X coordinate where to place the data card view relative to the upper-left corner of the window

*lY*
:   Y coordinate where to place the data card view relative to the upper-left corner of the window

*poCallback*
:   Optional pointer to a class that implements [IEdmCallback](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback.html) to handle notifications from the data card view (see **Remarks**)

*lEdmCardViewFlags*
:   Appearance and functionality of the data card view as defined in [EmdCardViewFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCardViewFlag.html)

#### Return Value

[IEdmCardView5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardView5.html); Nothing or null if the file does not have a data card associated with it

# ![](dotnetimages/collapse.gif)Example

[Create Card View (C#)](Create_Card_View_Example_CSharp.htm)

[Create Card View (VB.NET)](Create_Card_View_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

If the callback is implemented for this card view:

* [IEdmCallback::SetModifiedFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback~SetModifiedFlag.html) is called whenever the user makes a change in the file data card.* [IEdmCallback::SetProgressRange](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback~SetProgressRange.html) is called if the file data card contains a button connected to an add-in, and the add-in returns a combination of [EdmCardFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCardFlag.html) values other than EdmCardFlag.EdmCF\_Nothing. IEdmCallback::SetProgressRange is called with its lMin and lMax set to the EdmCardFlags passed in by the add-in. See [Calling VB.NET Add-ins](vbcardbutton.htm).

C++ users not using smart-pointer wrapper functions must release the returned interface, IEdmCardView5.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: The file does not have a card associated with it.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFolder10 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder10.html)

[IEdmFolder10 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder10_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2017