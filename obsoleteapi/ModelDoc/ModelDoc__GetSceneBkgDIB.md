<!-- source: obsoleteapi/ModelDoc/ModelDoc__GetSceneBkgDIB.htm -->

# ModelDoc::GetSceneBkgDIB

This
method is obsolete and has been superseded by ModelDoc2::GetSceneBkgDIB.

Description

This method gets background image as a LPDIBSECTION.

Syntax (OLE Automation)

l\_dib = ModelDoc.GetSceneBkgDIB
( )

|  |  |  |
| --- | --- | --- |
| Return: | (long) l\_dib | Background image as DIBSECTION |

Syntax (COM)

status = ModelDoc->GetSceneBkgDIB
( &l\_dib )

|  |  |  |
| --- | --- | --- |
| Output: | (long)l\_dib | Background image as DIBSECTION |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

For more information, see Bitmap structures, DIBSECTION
in MicroSoft Help.

The memory for the image bits ( DIBSECTION.dsBm.bmBits)
and this structure are allocated by SolidWorks and must be deleted by
the caller.