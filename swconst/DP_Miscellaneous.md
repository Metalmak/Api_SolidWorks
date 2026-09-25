<!-- source: swconst/DP_Miscellaneous.htm -->

# SOLIDWORKS API Help

# Document Properties > Miscellaneous

Some document-level enumerators exist that do
not correspond to any of the controls shown on the SOLIDWORKS **Tools >
Options > Document Properties** dialogs. Click the links to jump to the tables in this
Help topic or to the Help topics containing these
miscellaneous document-level
enumerators.

See System
Options and Document Properties for details about system options and
document properties.

| Miscellaneous Document-level Enumerators | | |
| **SOLIDWORKS** | | SOLIDWORKS Routing |
| Related to categories on Document Properties tab | Not related to categories on Document Properties tab |
| Annotations    - [Notes](#Notes)  Dimensions    - [Hole Callout](#DimensionsHoleCallout)  [DimXpert](#DimXpert)  [Detailing](#Detailing)  [Grid/Snap](#Grid/Snap)  [Material Properties](#MaterialProperties)  [Plane Display](#Plane)  [Configurations](#Configurations) | [Annotations folder shortcut menu](#Annotations-RMB)  [Dimensions - Drafting Standard](#DimensionsStandard)  [PropertyManager](#PropertyManager)  [View menu](#View) [Bounding Box](#BoundingBox) [Pdf](#Pdf) | Route Properties PropertyManager page  Twisted Pair Parameters |

Annotations folder
shortcut menu

| Enumerator | Get/Set Methods | Return Value or <Value> | Comment |
| swShowAnnotationInAnnotationViews | IModelDocExtension::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swShowAnnotationInAnnotationViews, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swShowAnnotationInAnnotationViews, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Boolean value | Specifies whether to enable annotation view visibility; corresponds to Annotations' folder shortcut menu item, **Enable Annotation View Visibility** |

Detailing

| Enumerator | Get/Set Methods | Return Value or <Value> | Comment |
| swDetailingAngularDimLeaderStyle | IModelDocExtension::GetUserPreferenceInteger(swUserPreferenceInteger\_e.swDetailingAngularDimLeaderStyle, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceInteger(swUserPreferenceInteger\_e.swDetailingAngularDimLeaderStyle, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, swDisplayDimensionLeaderText\_e.<Value>) | See swDisplayDimensionLeaderText\_e for valid options | Specifies the style of text placement for angular leaders |
| swDetailingAngularToleranceStyle | IModelDocExtension::GetUserPreferenceInteger(swUserPreferenceInteger\_e.swDetailingAngularDimLeaderStyle, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceInteger(swUserPreferenceInteger\_e.swDetailingAngularDimLeaderStyle, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, swTolType\_e.<Value>) | See swTolType\_e for valid options | Specifies the angular tolerance style |
| swDetailingChamferDimTextStyle | IModelDocExtension::GetUserPreferenceInteger(swUserPreferenceInteger\_e.swDetailingChamferDimTextStyle, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceInteger(swUserPreferenceInteger\_e.swDetailingChamferDimTextStyle, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, swDetailingChamferDimLeaderTextStyle\_e.<Value>) | See swDetailingChamferDimLeaderTextStyle\_e for valid options | Specifies how to display text relative to the leader |
| swDetailingCenterMarkShowLines | IModelDocExtension::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDetailingCenterMarkShowLines, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDetailingCenterMarkShowLines, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Boolean value | Specifies whether to display center mark lines |
| swDetailingCenterMarkUseCenterline | IModelDocExtension::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDetailingCenterMarkUseCenterline, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDetailingCenterMarkUseCenterline, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Boolean value | Specifies whether lines in center mark use font specified for centerlines |
| swDetailingDimFontHeight | IModelDocExtension::GetUserPreferenceDouble(swUserPreferenceDouble\_e.swDetailingDimFontHeight, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceDouble(swUserPreferenceDouble\_e.swDetailingDimFontHeight, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Double value in meters | Specifies height of dimensions |
| swDetailingDisplayWithBrokenLeaders | IModelDocExtension::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDetailingDisplayWithBrokenLeaders, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDetailingDisplayWithBrokenLeaders, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Boolean value | For ANSI dimensioning standard only; specifies whether to display broken leaders |
| swDetailingLinearDimLeaderStyle | IModelDocExtension::GetUserPreferenceInteger(swUserPreferenceInteger\_e.swDetailingLinearDimLeaderStyle, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceInteger(swUserPreferenceInteger\_e.swDetailingLinearDimLeaderStyle, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, swDisplayDimensionLeaderText\_e.<Value>) | See swDisplayDimensionLeaderText\_e for valid options | Specifies the style of text placement for linear leaders |
| swDetailingLinearToleranceStyle | IModelDocExtension::GetUserPreferenceInteger(swUserPreferenceInteger\_e.swDetailingLinearToleranceStyle, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceInteger(swUserPreferenceInteger\_e.swDetailingLinearToleranceStyle, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, swTolType\_e.<Value>) | See swTolType\_e for valid options | Specifies the linear tolerance style |
| swDetailingMaxAngularToleranceValue | IModelDocExtension::GetUserPreferenceDouble(swUserPreferenceDouble\_e.swDetailingMaxAngularToleranceValue, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceDouble(swUserPreferenceDouble\_e.swDetailingMaxAngularToleranceValue, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Double value | Specifies the maximum variation for the type of angular tolerance selected |
| swDetailingMaxLinearToleranceValue | IModelDocExtension::GetUserPreferenceDouble(swUserPreferenceDouble\_e.swDetailingMaxLinearToleranceValue, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceDouble(swUserPreferenceDouble\_e.swDetailingMaxLinearToleranceValue, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Double value in meters | Specifies maximum variation for type of linear tolerance selected |
| swDetailingMaxWitnessLineLength | IModelDocExtension::GetUserPreferenceDouble(swUserPreferenceDouble\_e.swDetailingMaxWitnessLineLength, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceDouble(swUserPreferenceDouble\_e.swDetailingMaxWitnessLineLength, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Double value in meters | Specifies maximum length for a witness line |
| swDetailingMinAngularToleranceValue | IModelDocExtension::GetUserPreferenceDouble(swUserPreferenceDouble\_e.swDetailingMinAngularToleranceValue, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceDouble(swUserPreferenceDouble\_e.swDetailingMinAngularToleranceValue, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Double value | Specifies minimum variation for type of angular tolerance selected |
| swDetailingMinLinearToleranceValue | IModelDocExtension::GetUserPreferenceDouble(swUserPreferenceDouble\_e.swDetailingMinLinearToleranceValue, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceDouble(swUserPreferenceDouble\_e.swDetailingMinLinearToleranceValue, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Double value in meters | Specifies minimum variation for type of linear tolerance selected |
| swDetailingNoteFontHeight | IModelDocExtension::GetUserPreferenceDouble(swUserPreferenceDouble\_e.swDetailingNoteFontHeight, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceDouble(swUserPreferenceDouble\_e.swDetailingNoteFontHeight, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Double value in meters | Specifies height of notes |
| swDetailingRadialDimLeaderStyle | IModelDocExtension::GetUserPreferenceInteger(swUserPreferenceInteger\_e.swDetailingRadialDimLeaderStyle, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceInteger(swUserPreferenceInteger\_e.swDetailingRadialDimLeaderStyle, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, swDisplayDimensionLeaderText\_e.<Value>) | See swDisplayDimensionLeaderText\_e for valid options | Specifies the style of text placement for radial leaders |
| swDetailingToleranceFitToDisplayAngular | IModelDocExtension::GetUserPreferenceInteger(swUserPreferenceInteger\_e.swDetailingToleranceFitToDisplayAngular, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceInteger(swUserPreferenceInteger\_e.swDetailingToleranceFitToDisplayAngular, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, swFitTolDisplay\_e.<Value>) | If swTolType\_e set to swTolFIT, swTolFITWITHTOL, or swTolFITTOLONLY, then see swFitTolDisplay\_e for valid options |  |
| swDetailingToleranceFitToDisplayLinear | IModelDocExtension::GetUserPreferenceInteger(swUserPreferenceInteger\_e.swDetailingToleranceFitToDisplayLinear, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceInteger(swUserPreferenceInteger\_e.swDetailingToleranceFitToDisplayLinear, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, swFitTolDisplay\_e.<Value>) | If swTolType\_e set to swTolFIT, swTolFITWITHTOL, or swTolFITTOLONLY, then see swFitTolDisplay\_e for valid options |  |

[Back to top](#Top)

Dimensions
- Drafting Standard

| Enumerator | Get/Set Methods | Return Value or <Value> | Comment |
| swDetailingAutoInsertDimsMarkedForDrawing | IModelDocExtension::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDetailingAutoInsertDimsMarkedForDrawing, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDetailingAutoInsertDimsMarkedForDrawing, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Boolean value | Specifies whether to automatically insert dimensions marked for the drawing in new drawing views; see IDisplayDimension::MarkedForDrawing for details about marking dimensions for drawings |
| swDetailingDimensionsAngularToleranceUseParentheses | IModelDocExtension::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDetailingDimensionsAngularToleranceUseParentheses, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDetailingDimensionsAngularToleranceUseParentheses, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Boolean value | For bilateral, symmetric, or fit-with-tolerance types only; specifies whether to show parentheses around angular tolerances |
| swDetailingDimensionStandardName | IModelDocExtension::GetUserPreferenceString(swUserPreferenceString\_e.swDetailingDimensionStandardName, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceString(swUserPreferenceString\_e.swDetailingDimensionStandardName, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Valid string values:   * ANSI * ISO * DIN * JIS * BSI * GOST * GB | Detailing standard |
| swDetailingDimLeaderOverrideStandard | IModelDocExtension::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDetailingDimLeaderOverrideStandard, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDetailingDimLeaderOverrideStandard, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Boolean value | Specifies whether to override standard's leader display |
| swDetailingDimOffsetText | IModelDocExtension::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDetailingDimOffsetText, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDetailingDimOffsetText, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Boolean value | Specifies whether to offset dimension text or not |
| swDetailingDimsFollowDimXpertLayout | IModelDocExtension::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDetailingDimsFollowDimXpertLayout, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDetailingDimsFollowDimXpertLayout, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Boolean value | Specifies whether to follow DimXpert dimension/annotation layout |
| swDetailingDimsSnapTextToGrid | IModelDocExtension::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDetailingDimsSnapTextToGrid, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDetailingDimsSnapTextToGrid, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Boolean value | Specifies whether to snap dimension text to grid in drawings or sketches |
| swDetailingShowHaloAroundAnnotation | IModelDocExtension::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDetailingShowHaloAroundAnnotation, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDetailingShowHaloAroundAnnotation, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Boolean value | Specifies whether to display a halo of space around dimensions or annotations that belong to the drawing view or a sketch and are on top of an area hatch |

[Back to top](#Top)

Dimensions
- Hole Callout

| Enumerator | Get/Set Methods | Return Value or <Value> | Comment |
| swDetailingDualDimPosition | IModelDocExtension::GetUserPreferenceInteger(swUserPreferenceInteger\_e.swDetailingDualDimPosition, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceInteger(swUserPreferenceInteger\_e.swDetailingDualDimPosition, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, swDetailingDualDimPosition\_e.<Value>) | See swDetailingDualDimPosition\_e for valid options | Allows the display of dimensions in two kinds of units |

[Back to top](#Top)

DimXpert

| Enumerator | Get/Set Methods | Return Value or <Value> | Comment |
| swDisplayComponentDimXpertAnnotations | IModelDocExtension::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDisplayComponentDimXpertAnnotations, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDisplayComponentDimXpertAnnotations, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Boolean value |  |

[Back to top](#Top)

Grid/Snap

| Enumerator | Get/Set Methods | Return Value or <Value> | Comment |
| swSnapOnlyIfGridDisplayed | IModelDocExtension::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swSnapOnlyIfGridDisplayed, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swSnapOnlyIfGridDisplayed, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Boolean value | Specifies whether to snap to grid if swGridDisplay is turned on |
| swSnapToAngle | IModelDocExtension::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swSnapToAngle, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swSnapToAngle, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Boolean value | Specifies whether sketched lines snap to predefined angle |
| swSnapToAngleValue | IModelDocExtension::GetUserPreferenceDouble(swUserPreferenceDouble\_e.swSnapToAngleValue, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceDouble(swUserPreferenceDouble\_e.swSnapToAngleValue, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Double value | Specifies angle to which sketched lines should snap |
| swSnapToPoints | IModelDocExtension::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swSnapToPoints, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swSnapToPoints, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Boolean value | Specifies whether points snap to grid |

[Back to top](#Top)

Material Properties

| Enumerator | Get/Set Methods | Return Value or <Value> | Comment |
| swMaterialPropertySolidFill | IModelDocExtension::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swMaterialPropertySolidFill, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swMaterialPropertySolidFill, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Boolean value | For parts only; specifies whether to set the fill for area hatch or solid |

[Back to top](#Top)

Notes

| Enumerator | Get/Set Methods | Return Value or <Value> | Comment |
| swDetailingNotesDisplayWithBentLeader | IModelDocExtension::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDetailingNotesDisplayWithBentLeader, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDetailingNotesDisplayWithBentLeader, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Boolean value | Specifies whether to display notes using bent leaders |

[Back to top](#Top)

Plane Display

| Enumerator | Get/Set Methods | Return Value or <Value> | Comment |
| swPlaneDisplayShowEdges | IModelDocExtension::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swPlaneDisplayShowEdges, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swPlaneDisplayShowEdges, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Boolean value | Edges of planes take the same color as the front and back faces, are not transparent, and are always displayed |

[Back to top](#Top)

Configurations

| Enumerator | Get/Set Methods | Return Value or <Value> | Comment |
| swDefaultConfigSortOrder | IModelDocExtension::GetUserPreferenceInteger(swUserPreferenceInteger\_e.swDefaultConfigSortOrder, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceInteger(swUserPreferenceInteger\_e.swDefaultConfigSortOrder, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, swConfigTreeSortType\_e.<Value>) | Values as defined in swConfigTreeSortType\_e | ConfigurationManager RMB menu |

[Back to top](#Top)

PropertyManager

| Enumerator | Get/Set Methods | Return Value or <Value> | Comment |
| swPropertyManagerColorActiveClosedDivider | IModelDocExtension::GetUserPreferenceInteger(swUserPreferenceInteger\_e.swPropertyManagerColorActiveClosedDivider, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceInteger(swUserPreferenceInteger\_e.swPropertyManagerColorActiveClosedDivider, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Read-only integer value for RGB color in use |  |
| swPropertyManagerColorBackground | IModelDocExtension::GetUserPreferenceInteger(swUserPreferenceInteger\_e.swPropertyManagerColorBackground, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceInteger(swUserPreferenceInteger\_e.swPropertyManagerColorBackground, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Read-only integer value for RGB color in use |  |
| swPropertyManagerColor\_Divider | IModelDocExtension::GetUserPreferenceInteger(swUserPreferenceInteger\_e.swPropertyManagerColor\_Divider, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceInteger(swUserPreferenceInteger\_e.swPropertyManagerColor\_Divider, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Read-only integer value for RGB color in use |  |
| swPropertyManagerColorEditBox | IModelDocExtension::GetUserPreferenceInteger(swUserPreferenceInteger\_e.swPropertyManagerColorEditBox, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceInteger(swUserPreferenceInteger\_e.swPropertyManagerColorEditBox, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Read-only integer value for RGB color in use |  |
| swPropertyManagerColor\_EditText | IModelDocExtension::GetUserPreferenceInteger(swUserPreferenceInteger\_e.swPropertyManagerColor\_EditText, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceInteger(swUserPreferenceInteger\_e.swPropertyManagerColor\_EditText, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Read-only integer value for RGB color in use |  |
| swPropertyManagerColorImportantMessage | IModelDocExtension::GetUserPreferenceInteger(swUserPreferenceInteger\_e.swPropertyManagerColorImportantMessage, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceInteger(swUserPreferenceInteger\_e.swPropertyManagerColorImportantMessage, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Read-only integer value for RGB color in use |  |
| swPropertyManagerColorInnerBorder | IModelDocExtension::GetUserPreferenceInteger(swUserPreferenceInteger\_e.swPropertyManagerColorInnerBorder, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceInteger(swUserPreferenceInteger\_e.swPropertyManagerColorInnerBorder, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Read-only integer value for RGB color in use |  |
| swPropertyManagerColorLabelAndIcon | IModelDocExtension::GetUserPreferenceInteger(swUserPreferenceInteger\_e.swPropertyManagerColorLabelAndIcon, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceInteger(swUserPreferenceInteger\_e.swPropertyManagerColorLabelAndIcon, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Read-only integer value for RGB color in use |  |
| swPropertyManagerColorTitle | IModelDocExtension::GetUserPreferenceInteger(swUserPreferenceInteger\_e.swPropertyManagerColorTitle, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceInteger(swUserPreferenceInteger\_e.swPropertyManagerColorTitle, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Read-only integer value for RGB color in use |  |
| swPropertyManagerColorOuterBorder | IModelDocExtension::GetUserPreferenceInteger(swUserPreferenceInteger\_e.swPropertyManagerColorOuterBorder, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceInteger(swUserPreferenceInteger\_e.swPropertyManagerColorOuterBorder, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Read-only integer value for RGB color in use |  |
| swPropertyManagerColorTopBorder | IModelDocExtension::GetUserPreferenceInteger(swUserPreferenceInteger\_e.swPropertyManagerColorTopBorder, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceInteger(swUserPreferenceInteger\_e.swPropertyManagerColorTopBorder, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Read-only integer value for RGB color in use |  |
| swPropertyManagerColorDivider | IModelDocExtension::GetUserPreferenceInteger(swUserPreferenceInteger\_e.swPropertyManagerColorDivider, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceInteger(swUserPreferenceInteger\_e.swPropertyManagerColorDivider, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Read-only integer value for RGB color in use |  |

[Back to top](#Top)

View menu

| Enumerator | Get/Set Methods | Return Value or <Value> | Comment |
| swDisplayCameraFOVBox | IModelDocExtension::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDisplayCameraFOVBox, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDisplayCameraFOVBox, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Boolean value | Specifies whether to display Field of View (FOV) box in the graphics area when viewing through a camera |

[Back to top](#Top)

Bounding Box

| Enumerator | Get/Set Methods | Return Value or <Value> | Comment |
| swViewDispGlobalBBox | IModelDocExtension::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swViewDispGlobalBBox, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swViewDispGlobalBBox, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Boolean value |  |

[Back to top](#Top)

Pdf

| Enumerator | Get/Set Methods | Return Value or <Value> | Comment |
| swPdfIncludeBookmarks | IModelDocExtension::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swPdfIncludeBookmarks, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swPdfIncludeBookmarks, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Boolean value |  |

[Back to top](#Top)