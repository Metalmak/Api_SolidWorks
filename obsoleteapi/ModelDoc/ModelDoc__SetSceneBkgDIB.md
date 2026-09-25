<!-- source: obsoleteapi/ModelDoc/ModelDoc__SetSceneBkgDIB.htm -->

# ModelDoc::SetSceneBkgDIB

This method is obsolete
and has been superseded by ModelDoc2::SetSceneBkgDIB.

Description

This sets background image described by DIBSECTION data.

Syntax (OLE Automation)

(void) ModelDoc.SetSceneBkgDIB ( l\_dib
)

|  |  |  |
| --- | --- | --- |
| Input: | (long) l\_dib | Pointer to DIBSECTION |

Syntax (COM)

status = ModelDoc->SetSceneBkgDIB
( l\_dib )

|  |  |  |
| --- | --- | --- |
| Input: | (long) l\_dib | Pointer to DIBSECTION |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

For more information, see the description of bitmap structures in MicroSoft
Help.

Old background images are deleted automatically.