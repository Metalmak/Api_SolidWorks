<!-- source: sldworksapiprogguide/Overview/Third-party_Data_in_SOLIDWORKS_Files.htm -->

# API Help

# Third-party Data in SOLIDWORKS Files

Starting with SOLIDWORKS 2015, third-party
data stored in SOLIDWORKS files cannot be externally read or written by standard
structured storage or compound file techniques.

To read or
write third-party data, use the methods and events in the SOLIDWORKS API or
SOLIDWORKS Document Manager API.

SOLIDWORKS API:

* IModelDoc2::IGet3rdPartyStorage
* IModelDoc2::IRelease3rdPartyStorage
* IModelDocExtension::IGet3rdPartyStorageStore
* IModelDocExtension::IRelease3rdPartyStorageStore
* DAssemblyDocEvents::AutoSaveToStorageNotifyEventHandler Delegate
* DAssemblyDocEvents::AutoSaveToStorageStoreNotifyEventHandler Delegate
* DAssemblyDocEvents::LoadFromStorageNotifyEventHandler Delegate
* DAssemblyDocEvents::LoadFromStorageStoreNotifyEventHandler Delegate
* DAssemblyDocEvents::SaveToStorageNotifyEventHandler Delegate
* DAssemblyDocEvents::SaveToStorageStoreNotifyEventHandler Delegate
* DDrawingDocEvents::AutoSaveToStorageNotifyEventHandler Delegate
* DDrawingDocEvents::AutoSaveToStorageStoreNotifyEventHandler Delegate
* DDrawingDocEvents::LoadFromStorageNotifyEventHandler Delegate
* DDrawingDocEvents::LoadFromStorageStoreNotifyEventHandler Delegate
* DDrawingDocEvents::SaveToStorageNotifyEventHandler Delegate
* DDrawingDocEvents::SaveToStorageStoreNotifyEventHandler Delegate
* DPartDocEvents::AutoSaveToStorageNotifyEventHandler Delegate
* DPartDocEvents::AutoSaveToStorageStoreNotifyEventHandler Delegate
* DPartDocEvents::LoadFromStorageNotifyEventHandler Delegate
* DPartDocEvents::LoadFromStorageStoreNotifyEventHandler Delegate
* DPartDocEvents::SaveToStorageNotifyEventHandler Delegate
* DPartDocEvents::SaveToStorageStoreNotifyEventHandler Delegate

**SOLIDWORKS Document Manager API:**

* ISwDMDocument20::Delete3rdPartyStorage
* ISwDMDocument20::Delete3rdPartyStorageStore
* ISwDMDocument19::Get3rdPartyStorage
* ISwDMDocument19::Get3rdPartyStorageStore
* ISwDMDocument19::Release3rdPartyStorage
* ISwDMDocument19::Release3rdPartyStorageStore