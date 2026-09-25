<!-- source: obsoleteapi/PropertyManagerPage2Handler4/PropertyManagerPage2Handler4__OnPreview.htm -->

# PropertyManagerPage2Handler4::OnPreview

This method is obsolete and has been superseded
by PropertyManagerPage2Handler5::OnPreview.

Description

This method is called when
a user clicks the Preview button on a PropertyManager page.

Syntax (OLE Automation)

retval = PropertyManagerPage2Handler4.OnPreview ()

|  |  |  |
| --- | --- | --- |
| Output: | (VARIANT\_BOOL) retval | TRUE if the operations specified by your add-in executes, FALSE if not (see Remarks) |

#

Syntax (COM)

status = PropertyManagerPage2Handler4->OnPreview
( &retval)

|  |  |  |
| --- | --- | --- |
| Output: | (VARIANT\_BOOL) retval | TRUE if the operations specified by your add-in executes, FALSE if not (see Remarks) |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks

To show a Preview button on
a PropertyManager page, include swPropertyManagerOptions\_PreviewButton
in the Options argument of SldWorks::CreatePropertyManagerPage.

You can do whatever you want
in response to the Preview button being clicked. Your add-in is responsible
for preview handling, including keeping track of the state of the Preview
button. Your add-in controls what happens when the Preview button is clicked;
SolidWorks takes not action when the Preview button is clicked. SolidWorks
ignores the return value because by the time the callback handler is called,
the button has already changed.