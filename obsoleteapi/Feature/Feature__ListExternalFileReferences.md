<!-- source: obsoleteapi/Feature/Feature__ListExternalFileReferences.htm -->

# Feature::ListExternalFileReferences

This method is obsolete and has been superseded
by Feature::ListExternalFileReferences2.

Description

This method gets the names and status of the
external file references on this model.

Syntax (OLE Automation)

void = Feature.ListExternalFileReferences ( modelPathName,
componentPathName, feature, dataType, Status, refEntity, featCom )

| Output: | (VARIANT) \*modelPathName | Array of external model references |
| Output: | (VARIANT) \*componentPathName | Array of external component references |
| Output: | (VARIANT) \*feature | Array of external feature references |
| Output: | (VARIANT) \*dataType | Array of types of data |
| Output: | (VARIANT) \*Status | Status of external reference as defined in swExternalReferenceStatus\_e |
| Output: | (VARIANT) \*refEntity | Array of external entity references |
| Output: | (VARIANT) \*featCom | Array of feature components |

Syntax (COM)

status = Feature->IListExternalFileReferences
( numRefs, modelPathName, compPathName, feature, dataType, Status, refEntity,
featComp )

| Input: | (long) numRefs | Number of external references |
| Output: | (BSTR\*) modelPathName | Array of external model references of size numRefs |
| Output: | (BSTR\*) compPathName | Array of external component references of size numRefs |
| Output: | (BSTR\*) feature | Array of external feature references of size numRefs |
| Output: | (BSTR\*) dataType | Array of types of data of size numRefs |
| Output: | (long\*) Status | Status of external reference as defined in swExternalReferenceStatus\_e |
| Output: | (BSTR\*) refEntity | Array of external entity references of size numRefs |
| Output: | (BSTR\*) featComp | Array of feature components of size numRefs |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks