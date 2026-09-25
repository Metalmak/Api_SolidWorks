<!-- source: obsoleteapi/MacroFeatureData/MacroFeatureData__EditBody.htm -->

# MacroFeatureData::EditBody

This property is obsolete and
has been superseded by MacroFeatureData::EditBodies,
MacroFeatureData::IGetEditBodies,
and MacroFeatureData::ISetEditBodies.

Description

This property gets or sets the body to be modified
by this feature.

Syntax (OLE Automation)

editBody = MacroFeatureData.EditBody (VB Get property)

MacroFeatureData.EditBody = editBody (VB Set property)

editBody = MacroFeatureData.GetEditBody ( ) (C++
Get property)

MacroFeatureData.SetEditBody ( editBody ) (C++ Set
property)

|  |  |  |
| --- | --- | --- |
| Property: | (LPBODY2) editBody | Pointer to the body to edit |

Syntax (COM)

status = MacroFeatureData->get\_EditBody ( \*editBody
)

status = MacroFeatureData->put\_EditBody ( editBody
)

|  |  |  |
| --- | --- | --- |
| Property: | (LPBODY2) editBody | Pointer to the body to edit |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

See Accessing Selections that Define Features
for details on using this property.