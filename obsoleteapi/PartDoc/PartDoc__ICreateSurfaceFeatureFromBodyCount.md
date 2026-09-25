<!-- source: obsoleteapi/PartDoc/PartDoc__ICreateSurfaceFeatureFromBodyCount.htm -->

# PartDoc::ICreateSurfaceFeatureFromBodyCount

This
method is obsolete and has been superseded by  PartDoc::ICreateSurfaceFeatureFromBodyCount2.

Description

This method gets the number
of surface features that will be created from a body.

Syntax (OLE Automation)

Not available.

Syntax (COM)

status = PartDoc->ICreateSurfaceFeatureFromBodyCount
( body, options, &count )

|  |  |  |
| --- | --- | --- |
| Input: | (LPBODY) body | Body from wihc to create surface features |
| Input: | (long) options | Options as defined in swCreateFeatureBodyOpts\_e |
| Output: | (long) count | Number of surface features to create from a body |
| Return: | (HRESULT) status | S\_OK if successful. |

Remarks