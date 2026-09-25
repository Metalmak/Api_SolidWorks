<!-- source: sldworksapiprogguide/Overview/Persistent_Reference_IDs.htm -->

# SOLIDWORKS API Help

# Persistent Reference IDs

Selectable objects in a SOLIDWORKS model document are assigned unique
reference IDs. The reference IDs persist for the objects in the model
document across SOLIDWORKS sessions. Other applications can use persistent
reference IDs to locate objects at runtime.

Some methods that support the retrieval of persistent reference IDs are:

* IModelDocExtension::GetPersistReferenceCount3:
  returns the size of the persistent reference ID for the selected object.
  Call this method before calling
  IModelDocExtension::IGetPersistReference3.

NOTE:
See swSelectType\_e
for a list of selectable objects. You can select the objects via the user
interface or programmatically by using IModelDocExtension::SelectByID2.

* IModelDocExtension::GetPersistReference3:
  returns the persistent reference ID for the selected object. Call this
  method before calling
  IModelDocExtension::GetObjectByPersistReference3.
* IModelDocExtension::GetObjectByPersistReference3:
  returns the object by its persistent reference ID.