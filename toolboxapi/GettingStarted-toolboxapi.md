<!-- source: toolboxapi/GettingStarted-toolboxapi.html -->

![](images/collapse.gif)
![](images/expand.gif)
![](images/copycode.gif)
![](images/copycodeHighlight.gif)
![](images/drpdown.gif)
![](images/drpdown_orange.gif)

|  |
| --- |
|  |

|  |  |
| --- | --- |
| SOLIDWORKS Toolbox Browser API |  |
| Getting Started |
| Send Feedback | |

Glossary Item Box

The SOLIDWORKS Toolbox Browser API is designed specifically to allow third-party PDMs to interact with the SOLIDWORKS Toolbox Browser and the Toolbox Configurator. The SOLIDWORKS Toolbox Browser API includes:

* SOLIDWORKS Toolbox Browser API (**SOLIDWORKS.Interop.swbrowser.dll**):
  + [IApplication](SOLIDWORKS.Interop.swbrowser~SOLIDWORKS.Interop.swbrowser.IApplication.html)+ [IPDMDocManager](SOLIDWORKS.Interop.swbrowser~SOLIDWORKS.Interop.swbrowser.IPDMDocManager.html)* SOLIDWORKS Toolbox Configurator API (**SOLIDWORKS.Interop.sldtoolboxconfigureaddin.dll**):
    + [IToolboxConfiguratorAddin](SOLIDWORKS.Interop.sldtoolboxconfigureaddin~SOLIDWORKS.Interop.sldtoolboxconfigureaddin.IToolboxConfiguratorAddin.html)+ [IToolBoxConfiguratorApplication](SOLIDWORKS.Interop.sldtoolboxconfigureaddin~SOLIDWORKS.Interop.sldtoolboxconfigureaddin.IToolBoxConfiguratorApplication.html)

##### Use the SOLIDWORKS Toolbox Browser API to Access the SOLIDWORKS Toolbox Browser

1. Set up a third-party PDM vault to contain the SOLIDWORKS Toolbox. See the PDM Administration Guide and the SOLIDWORKS Toolbox Help.- Create a SOLIDWORKS add-in using one of the add-in templates in the SOLIDWORKS API SDK.- In the add-in's ConnectToSW():
       1. Call ISldWorks::GetAddInObject, passing in the GUID of the SOLIDWORKS Toolbox Browser add-in type library (**Registry Editor >** **Computer\HKEY\_CLASSES\_ROOT\TypeLib\{ED783340-D5DB-11d4-BD5A-00C04F019809}**), to get a Dispatch pointer to the IApplication object and connect to the SOLIDWORKS Toolbox Browser.

          For example, in COM:

          LPDISPATCH pDisp = NULL;
          HRESULT hres = pSldWorks->GetAddInObject("{ED783340-D5DB-11d4-BD5A-00C04F019809}" , &pDisp);

          - Cast the Dispatch pointer to **SOLIDWORKS.Interop.swbrowser.IApplication** to gain access to the SOLIDWORKS Toolbox Browser API.- Implement and attach to PDMDocManager event handlers that control access to the PDM-managed SOLIDWORKS Toolbox Browser part documents.- Run the add-in. The SOLIDWORKS Toolbox Browser add-in is registered and loaded.- Open a document in SOLIDWORKS.- To open the SOLIDWORKS Toolbox Browser, select **Toolbox** from the SOLIDWORKS menu.- The add-in connects to the SOLIDWORKS Toolbox Browser.

##### Use the SOLIDWORKS Toolbox Browser API to Access the SOLIDWORKS Toolbox Configurator

1. Set up a third-party PDM vault to contain the SOLIDWORKS Toolbox. See the PDM Administration Guide and the SOLIDWORKS Toolbox Help.- Create a SOLIDWORKS add-in using one of the add-in templates in the SOLIDWORKS API SDK.- Use Microsoft Visual Studio 2010 **Tools > Create GUID** to create a GUID.- Add a class of type IToolboxConfiguratorAddin to the add-in, assigning the new GUID to the class.- Implement all of the methods of IToolboxConfiguratorAddin.- Implement and attach to PDMDocManager event handlers that control access to the PDM-managed SOLIDWORKS Toolbox Configurator part documents.- In the add-in's Connect(), cast the return variable, pTbcApplication, to **SOLIDWORKS.Interop.sldtoolboxconfigureaddin.IToolBoxConfiguratorApplication** to gain access to the SOLIDWORKS Toolbox Configurator API.- Debug the add-in. The Toolbox Configurator add-in is registered and loaded.- To open the Toolbox Configurator from SOLIDWORKS, select **Tools > Options > Hole Wizard/Toolbox > Configure**.- The add-in connects to the Toolbox Configurator.- In Visual Studio 2010 select **Debug > Attach to Process > SldToolboxConfigure.exe**.

[Back to top](#top)

##### SOLIDWORKS Toolbox Browser API Use Cases

###### Drag and Drop Standard SOLIDWORKS Toolbox Parts

1. After the user releases the mouse button to drop a SOLIDWORKS Toolbox Browser part onto the assembly, SOLIDWORKS fires the FileDropPreNotify event, passing the path name of the dropped file.- In the FileDropPreNotify event handler, the PDM application must call IAssemblyDoc::SetDroppedFileName, passing the path name of the PDM-managed version of the document (if it can be made writable) or a copy of the managed document that can be written to by SOLIDWORKS Toolbox Browser (if it cannot be made writable).- If SOLIDWORKS Toolbox Browser determines that the dropped file needs to be written to, it fires the [BeforeWritingToDocument event](SOLIDWORKS.Interop.swbrowser~SOLIDWORKS.Interop.swbrowser.DPDMDocManagerEvents_BeforeWritingToDocumentEventHandler.html), passing the path name of the PDM-managed version of the dropped file.- In the BeforeWritingToDocument event handler, the PDM application must ensure that the file that was previously passed to IAssemblyDoc::SetDroppedFileName is writable and call [IPDMDocManager::SetDocumentStatus](SOLIDWORKS.Interop.swbrowser~SOLIDWORKS.Interop.swbrowser.IPDMDocManager~SetDocumentStatus.html), passing [swPDMStatus\_e.swPDMStatusKnownAndAvailable](SOLIDWORKS.Interop.swbrowser~SOLIDWORKS.Interop.swbrowser.swPDMStatus_e.html). If the application passes any other status value, SOLIDWORKS Toolbox Browser generates an error and stops the file drop.- After the application updates the document, SOLIDWORKS Toolbox Browser fires the [AfterWritingToDocument event](SOLIDWORKS.Interop.swbrowser~SOLIDWORKS.Interop.swbrowser.DPDMDocManagerEvents_AfterWritingToDocumentEventHandler.html), passing the path name of the PDM-managed version of the document that was written to.- In the AfterWritingToDocument event handler, the PDM application must copy the working document back to the PDM-managed location and change the file attribute of the PDM-managed version to read-only.- SOLIDWORKS continues the file drop as usual.

[Back to top](#top)

###### Insert SmartFastener

1. After the user inserts a SmartFastener, SOLIDWORKS Toolbox Browser fires the [PreInsertDocument event](SOLIDWORKS.Interop.swbrowser~SOLIDWORKS.Interop.swbrowser.DPDMDocManagerEvents_PreInsertDocumentEventHandler.html), passing the path name of the PDM-managed version of the SmartFastener.- In the PreInsertDocument event handler, the PDM application must call [IPDMDocManager::SetManagedDocument](SOLIDWORKS.Interop.swbrowser~SOLIDWORKS.Interop.swbrowser.IPDMDocManager~SetManagedDocument.html), passing the path name of the PDM-managed version of the document (if it can be made writable) or a copy of the managed document that can be written to by SOLIDWORKS Toolbox Browser (if it cannot be made writable).- If it determines that the file needs to be written to, SOLIDWORKS Toolbox Browser fires the [BeforeWritingToDocument event](SOLIDWORKS.Interop.swbrowser~SOLIDWORKS.Interop.swbrowser.DPDMDocManagerEvents_BeforeWritingToDocumentEventHandler.html), passing the path name of the PDM-managed version of the file.- In the BeforeWritingToDocument event handler, the PDM application must ensure that the file that was previously passed to IAssemblyDoc::SetDroppedFileName is writable and call [IPDMDocManager::SetDocumentStatus](SOLIDWORKS.Interop.swbrowser~SOLIDWORKS.Interop.swbrowser.IPDMDocManager~SetDocumentStatus.html), passing [swPDMStatus\_e.swPDMStatusKnownAndAvailable](SOLIDWORKS.Interop.swbrowser~SOLIDWORKS.Interop.swbrowser.swPDMStatus_e.html). If the application passes any other status value, SOLIDWORKS Toolbox Browser generates an error and stops the file drop.- After the document is updated, SOLIDWORKS Toolbox Browser fires the [AfterWritingToDocument event](SOLIDWORKS.Interop.swbrowser~SOLIDWORKS.Interop.swbrowser.DPDMDocManagerEvents_AfterWritingToDocumentEventHandler.html), passing the path name of the PDM-managed version of the file.- In the AfterWritingToDocument event handler, the PDM application must copy the working document back to the PDM-managed location and change the file attribute of the PDM-managed version to read-only.- SOLIDWORKS continues the insert as usual.

[Back to top](#top)

##### SOLIDWORKS Toolbox Configurator API Use Case

###### Welcome to Toolbox Setup - Modify a Toolbox Part

1. After the user clicks the Save button, SOLIDWORKS Toolbox Configurator fires the [BeforeWritingToDocument event](SOLIDWORKS.Interop.swbrowser~SOLIDWORKS.Interop.swbrowser.DPDMDocManagerEvents_BeforeWritingToDocumentEventHandler.html), passing the path name of the PDM-managed version of the SOLIDWORKS Toolbox part being edited.- In the BeforeWritingToDocument event handler, the PDM application must try to unset the read-only attribute of the PDM-managed version of the Toolbox part. (If it can't, it must copy the part to a working file that can be written to and call [IPDMDocManager::SetManagedDocument](SOLIDWORKS.Interop.swbrowser~SOLIDWORKS.Interop.swbrowser.IPDMDocManager~SetManagedDocument.html), passing the path name of the working document.) It must then call [IPDMDocManager::SetDocumentStatus](SOLIDWORKS.Interop.swbrowser~SOLIDWORKS.Interop.swbrowser.IPDMDocManager~SetDocumentStatus.html), passing [swPDMStatus\_e.swPDMStatusKnownAndAvailable](SOLIDWORKS.Interop.swbrowser~SOLIDWORKS.Interop.swbrowser.swPDMStatus_e.html) before returning. If any other status value is passed, the SOLIDWORKS Toolbox Configurator generates an error.- After SOLIDWORKS Toolbox Configurator updates the document, it fires the [AfterWritingToDocument event](SOLIDWORKS.Interop.swbrowser~SOLIDWORKS.Interop.swbrowser.DPDMDocManagerEvents_AfterWritingToDocumentEventHandler.html), passing the path name of the PDM-managed version of the SOLIDWORKS Toolbox part being edited.- In the AfterWritingToDocument event handler, the PDM application must copy the working document back to the PDM-managed location. It must also change the file attribute of the PDM-managed version back to read-only.

[Back to top](#top)