<!-- source: obsoleteapi/SimpleHoleFeatureData/SimpleHoleFeatureData__SurfaceOffset.htm -->

# SimpleHoleFeatureData::SurfaceOffset

This
property is obsolete and has been superseded by SimpleHoleFeatureData2::SurfaceOffset.

Description

This property gets or sets the simple hole
feature offset from the surface.

Syntax (OLE Automation)

surfaceOffset = SimpleHoleFeatureData.SurfaceOffset   (VB
Get property)

SimpleHoleFeatureData.SurfaceOffset = surfaceOffset   (VB Set property)

surfaceOffset = SimpleHoleFeatureData.GetSurfaceOffset ( )  (C++
Get property)

SimpleHoleFeatureData.SetSurfaceOffset ( surfaceOffset )  (C++ Set property)

| Property: | (double) surfaceOffset | Offset from the surface of the simple hole feature |

Syntax (COM)

status = SimpleHoleFeatureData ->get\_SurfaceOffset
( &surfaceOffset )

status = SimpleHoleFeatureData ->put\_SurfaceOffset
( surfaceOffset )

| Property: | (double) surfaceOffset | Offset from the surface of the simple hole feature |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks