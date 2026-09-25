<!-- source: obsoleteapi/SimpleFilletFeatureData/SimpleFilletFeatureData__DefaultRadius.htm -->

# SimpleFilletFeatureData::DefaultRadius

This
property is obsolete and has been superseded by SimpleFilletFeatureData2::DefaultRadius.

Description

This property gets or sets the simple fillet
feature default fillet radius.

Syntax (OLE Automation)

radius = SimpleFilletFeatureData.DefaultRadius  (VB
Get property)

SimpleFilletFeatureData.DefaultRadius = radius  (VB Set property)

radius
= SimpleFilletFeatureData.GetDefaultRadius ( ) (C++ Get property)

SimpleFilletFeatureData.SetDefaultRadius ( radius )  (C++ Set property)

| Property: | (double) radius | Default fillet radius of the simple fillet feature |

Syntax (COM)

status = SimpleFilletFeatureData ->get\_DefaultRadius
( &radius )

status = SimpleFilletFeatureData ->put\_DefaultRadius
( radius )

| Property: | (double) radius | Default fillet radius of the simple fillet feature |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks