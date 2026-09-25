<!-- source: obsoleteapi/SimpleFilletFeatureData/SimpleFilletFeatureData__IsMultipleRadius.htm -->

# SimpleFilletFeatureData::IsMultipleRadius

This
property is obsolete and has been superseded by SimpleFilletFeatureData2::IsMultipleRadius.

Description

This property gets or sets the simple fillet
feature in a multiple radius fillet.

Syntax (OLE Automation)

isMultipleRadius = SimpleFilletFeatureData.IsMultipleRadius  (VB
Get property)

SimpleFilletFeatureData.IsMultipleRadius = isMultipleRadius  (VB Set property)

isMultipleRadius = SimpleFilletFeatureData.GetIsMultipleRadius
( )  (C++ Get property)

SimpleFilletFeatureData.SetIsMultipleRadius ( isMultipleRadius )  (C++ Set property)

| Property: | (BOOL) isMultipleRadius | TRUE if simple fillet feature is a multiple radius fillet, FALSE if not |

Syntax (COM)

status = SimpleFilletFeatureData ->get\_IsMultipleRadius
( &isMultipleRadius )

status = SimpleFilletFeatureData ->put\_IsMultipleRadius
( isMultipleRadius )

|  |  |  |
| --- | --- | --- |
| Property: | (VARIANT\_BOOL) isMultipleRadius | TRUE if simple fillet feature is a multiple radius fillet, FALSE if not |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks