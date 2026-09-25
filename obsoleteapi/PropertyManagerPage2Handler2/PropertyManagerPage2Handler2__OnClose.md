<!-- source: obsoleteapi/PropertyManagerPage2Handler2/PropertyManagerPage2Handler2__OnClose.htm -->

# PropertyManagerPage2Handler2::OnClose

This method is obsolete and has been superseded
by [PropertyManagerPage2Handler3::OnClose](../PropertyManagerPage2Handler3/PropertyManagerPage2Handler3__OnClose.htm).

Description

This method is called when
this PropertyManager is closing.

Syntax (OLE Automation)

void = PropertyManagerPage2Handler2.OnClose ( Reason
)

#

|  |  |  |
| --- | --- | --- |
| Input: | (long) Reason | Reason this method is called as defined in swPropertyManagerPageCloseReasons\_e |

#

Syntax (COM)

status = PropertyManagerPage2Handler2->OnClose
( Reason )

|  |  |  |
| --- | --- | --- |
| Input: | (long) Reason | Reason this method is called as defined in swPropertyManagerPageCloseReasons\_e |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks

This handler method is called
when the page is about to close.

| If you implemented the handler in... | Then you... |
| C++ | Can prevent the page from closing by setting the HRESULT return value to S\_FALSE |
| VB | Should use the Err.Raise method with a value of 1 to prevent the page from closing |
| NOTE:  When control returns to SolidWorks:   * These   values are recognized. * The   page remains displayed on the screen. * The   PropertyManagerPage2Handler2::AfterClose handler is not called. | |