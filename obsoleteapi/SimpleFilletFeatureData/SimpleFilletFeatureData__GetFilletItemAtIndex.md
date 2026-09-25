<!-- source: obsoleteapi/SimpleFilletFeatureData/SimpleFilletFeatureData__GetFilletItemAtIndex.htm -->

# SimpleFilletFeatureData::GetFilletItemAtIndex

This method is obsolete and has been superseded
by SimpleFilletFeatureData2::GetFilletItemAtIndex.

Description

This method gets the fillet
item at the specified index.

Syntax (OLE Automation)

pFilletItem = SimpleFilletFeatureData.GetFilletItemAtIndex
( index )

|  |  |  |
| --- | --- | --- |
| Input: | (int) index | Index at which fillet item is required |
| Return: | (LPDISPATCH) pFilletItem | Pointer to a dispatch object, the fillet item ( edge, face, loop, or NULL if the operation fails) |

Syntax (COM)

status = SimpleFilletFeatureData->IGetFilletItemAtIndex
( index, &pFilletItem )

|  |  |  |
| --- | --- | --- |
| Input: | (int) index | Index at which fillet item is required |
| Output: | (LPUNKNOWN) pFilletItem | Pointer to a dispatch object, the fillet item ( edge, face, loop, or NULL if the operation fails) |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks