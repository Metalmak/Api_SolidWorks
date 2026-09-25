<!-- source: obsoleteapi/SketchBlockInstance/SketchBlockInstance__Scale.htm -->

# SketchBlockInstance::Scale

This property is obsolete and has been superseded
by SketchBlockInstance::Scale2.

Description

This property gets or
sets the scale for this block instance.

Syntax (OLE Automation)

DScale = SketchBlockInstance.Scale (VB
Get property)

SketchBlockInstance.Scale = DScale
(VB Set property)

DScale = SketchBlockInstance.GetScale
( ) (C++ Get property)

SketchBlockInstance.SetScale ( DScale
) (C++ Set property)

|  |  |  |
| --- | --- | --- |
| Output: | (double) DScale | Scale: 0.0000001 to 500000 |

#

Syntax (COM)

status = SketchBlockInstance->get\_Scale
( &DScale )

status = SketchBlockInstance->put\_Scale
( DScale )

|  |  |  |
| --- | --- | --- |
| Output: | (double) DScale | Scale: 0.0000001 to 500000 |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks