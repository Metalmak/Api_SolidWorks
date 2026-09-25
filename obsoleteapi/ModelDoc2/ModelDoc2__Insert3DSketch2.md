<!-- source: obsoleteapi/ModelDoc2/ModelDoc2__Insert3DSketch2.htm -->

# ModelDoc2::Insert3DSketch2

This method is obsolete and has been superseded
by SketchManager::Insert3DSketch.

Description

This method inserts a new 3D sketch in a model
or closes the active sketch.

Syntax (OLE Automation)

ModelDoc2.Insert3DSketch2 (updateEditRebuild  )

| Input: | (VARIANT BOOL )updateEditRebuild | TRUE if you want to edit and rebuild, FALSE otherwise |

Syntax (COM)

status = ModelDoc2->Insert3DSketch2 (updateEditRebuild
)

| Input: | (VARIANT\_BOOL) status | TRUE if you want to edit and rebuild, FALSE otherwise |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks