<!-- source: obsoleteapi/ModelDoc2/ModelDoc2__InsertSketchPicture.htm -->

# ModelDoc2::InsertSketchPicture

This method is obsolete and has been superseded
by SketchManager::InsertSketchPicture.

Description

This method inserts a picture into the current
sketch. Supported image types are:

* Windows
  bitmap (\*.bmp)
* Tagged
  Image Format (\*.tif)

Syntax (OLE Automation)

pResult = ModelDoc2.InsertSketchPicture ( filename
)

#

|  |  |  |
| --- | --- | --- |
| Input: | (BSTR) filename | Path to image file including file extension |
| Output: | (VARIANT\_BOOL) pResult | TRUE if successful, FALSE otherwise |

#

Syntax (COM)

status = ModelDoc2->InsertSketchPicture ( filename,
&pResult )

|  |  |  |
| --- | --- | --- |
| Input: | (BSTR) filename | Path to image file including file extension |
| Output: | (VARIANT\_BOOL) pResult | TRUE if successful, FALSE otherwise |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks