<!-- source: sldworksapiprogguide/Overview/ConfigTraversAddinCPP.htm -->

# SOLIDWORKS API Help

# Get Names of Configurations Using BSTR\* C-array Example (C++)

// ConfigTraversAddin.cpp : Implementation of CConfigTraversAddin

// Add-in for getting the names of configurations in an active
model document

// Demonstrates ModelDoc2::IGetConfigurationNames taking
a BSTR\* C-array

#include "stdafx.h"

#include "ConfigTraversAddin.h"

#include "BitmapHandler.h"

// CConfigTraversAddin

// This method adds the CommandManager to the SOLIDWORKS
user-interface

void CConfigTraversAddin::AddCommandManager()

{

CComPtr<ICommandGroup> icmdGroup;

CComObject<CBitmapHandler> \*iBmp;

CComObject<CBitmapHandler>::CreateInstance(&iBmp);

long cmdIndex0, cmdIndex1;

const int array\_size = 2;

HRESULT hres;

int\* docTypes = new int[array\_size];

docTypes[0] = swDocASSEMBLY;

        docTypes[1]
= swDocDRAWING,

        docTypes[2]
= swDocPART;

CComBSTR title;

title.LoadString(IDS\_TOOLBAR\_TITLE);

CComBSTR hint;

hint.LoadString(IDS\_MENU\_HINT);

iCmdMgr->CreateCommandGroup(1,title,title,hint,-1,&icmdGroup);

CComBSTR smallImageFile;

iBmp->CreateBitmapFileFromResource(IDB\_TOOLBAR\_SMALL,
&smallImageFile);

icmdGroup->put\_SmallIconList(smallImageFile);

CComBSTR largeImageFile;

iBmp->CreateBitmapFileFromResource(IDB\_TOOLBAR\_LARGE,
&largeImageFile);

icmdGroup->put\_LargeIconList(largeImageFile);

CComBSTR largeIconFile;

iBmp->CreateBitmapFileFromResource(IDB\_ICON\_LARGE,
&largeIconFile);

icmdGroup->put\_LargeMainIcon(largeIconFile);

CComBSTR smallIconFile;

iBmp->CreateBitmapFileFromResource(IDB\_ICON\_SMALL,
&smallIconFile);

icmdGroup->put\_SmallMainIcon(smallIconFile);

CComBSTR tip;

CComBSTR callback;

CComBSTR enable;

long cmdIndex;

VARIANT\_BOOL cmdActivated;

callback.LoadString(IDS\_TOOLBAR\_CALLBACK0);

enable.LoadString(IDS\_TOOLBAR\_ENABLE0);

tip.LoadString(IDS\_TOOLBAR\_TIP0);

hint.LoadString(IDS\_TOOLBAR\_HINT0);

icmdGroup->AddCommandItem(tip,-1,hint,tip,0,callback,enable,0,&cmdIndex0);

icmdGroup->put\_HasToolbar(true);

icmdGroup->put\_HasMenu(true);

icmdGroup->Activate(&cmdActivated);

for(int i=0; i < array\_size + 1; i++)

{

CComPtr<ICommandTab> pTab = NULL;

long TabCount, docType = docTypes[i];

CComPtr<ICommandTab> AddinTab;

iCmdMgr->GetCommandTabCount(docType,
&TabCount);

  //
Check for tab

    iCmdMgr->GetCommandTab(docType,
title, &pTab);

if(pTab == NULL)

{

  //
If no tab, then add one

  iCmdMgr->AddCommandTab(docType,
title, &pTab);

  CComPtr<ICommandTabBox>
pBox;

  pTab->AddCommandTabBox(&pBox);

  //
Create two commands on this tab

  long
CommandIDCount = 2;

  long\*
CommandIDs = new long[2];

  long\*
TextDisplayStyles = new long[2];

  long
cmdID = 0;

  //
The two command buttons have different text styles

  icmdGroup->get\_CommandID(cmdIndex0,
&cmdID);

  CommandIDs[0]
= cmdID;

  TextDisplayStyles[0]
= swCommandTabButton\_TextHorizontal;

  icmdGroup->get\_ToolbarId(&cmdID);

  CommandIDs[1]
= cmdID;

  TextDisplayStyles[1]
= swCommandTabButton\_TextHorizontal;

  VARIANT\_BOOL
vbResult = VARIANT\_FALSE;

  pBox->IAddCommands(CommandIDCount,
CommandIDs, TextDisplayStyles, &vbResult);

  CommandIDCount
= 1;

  CommandIDs
= new long[1];

  TextDisplayStyles
= new long[1];

  icmdGroup->get\_ToolbarId(&cmdID);

  CommandIDs[0]
= cmdID;

  TextDisplayStyles[0]
= swCommandTabButton\_TextBelow | swCommandTabButton\_ActionFlyout;

  CComPtr<ICommandTabBox>
pBox1;

  pTab->AddCommandTabBox(&pBox1);

  pBox1->IAddCommands(CommandIDCount,
CommandIDs, TextDisplayStyles, &vbResult);

  CComPtr<ICommandTabBox>
pBoxNew1, pBoxNew2;

  pTab->AddSeparator(pBox1,
cmdID, &pBoxNew1);

}

}

// Clean up

iBmp->Dispose();

iBmp->Release();

}

void CConfigTraversAddin::RemoveCommandManager()

{

VARIANT\_BOOL cmdRemoved;

iCmdMgr->RemoveCommandGroup(1,&cmdRemoved);

}

// Event handlers

// Called when the active document in SOLIDWORKS changes

STDMETHODIMP CConfigTraversAddin::OnDocChange(void)

{

// TODO: Add your implementation code here

return S\_OK;

}

// Called when a new document is created or a document
is loaded

STDMETHODIMP CConfigTraversAddin::OnDocLoad(BSTR
docTitle, BSTR docPath)

{

// TODO: Add your implementation code here

return S\_OK;

}

// Called when the active model document changes in
SOLIDWORKS

STDMETHODIMP CConfigTraversAddin::OnModelDocChange(void)

{

// TODO: Add your implementation code here

return S\_OK;

}

// Called when a new file is created

STDMETHODIMP CConfigTraversAddin::OnFileNew(LPDISPATCH
newDoc, long docType, BSTR templateName)

{

// TODO: Add your implementation code here

return S\_OK;

}

// Utility methods

// Set up the add-in to catch SOLIDWORKS events

VARIANT\_BOOL CConfigTraversAddin::AttachEventHandlers()

{

VARIANT\_BOOL attached = VARIANT\_TRUE;

this->m\_libid = LIBID\_SldWorks;

this->m\_wMajorVerNum = GetSldWorksTlbMajor();

this->m\_wMinorVerNum = 0;

CSldWorksEvents::\_tih.m\_wMajor = this->m\_wMajorVerNum;

// Connect to the SldWorks event sink

HRESULT success = this->DispEventAdvise(iSwApp,
&\_\_uuidof(DSldWorksEvents));

if (success != S\_OK)

return VARIANT\_FALSE;

return attached;

}

// Stop listening for SOLIDWORKS events

VARIANT\_BOOL CConfigTraversAddin::DetachEventHandlers()

{

VARIANT\_BOOL detached = VARIANT\_TRUE;

// Disconnect from the SldWorks event sink

HRESULT success = this->DispEventUnadvise(iSwApp,
&\_\_uuidof(DSldWorksEvents));

CSldWorksEvents::\_tih.m\_plibid = &GUID\_NULL;

if (success != S\_OK)

return VARIANT\_FALSE;

return detached;

}

// ISwAddin Methods

// This is the starting point for the add-in

STDMETHODIMP CConfigTraversAddin::ConnectToSW(LPDISPATCH
ThisSW, long Cookie, VARIANT\_BOOL \* IsConnected)

{

ThisSW->QueryInterface(\_\_uuidof(ISldWorks),
(void\*\*)&iSwApp);

addinID = Cookie;

iSwApp->GetCommandManager(Cookie,&iCmdMgr);

VARIANT\_BOOL status = VARIANT\_FALSE;

iSwApp->SetAddinCallbackInfo((long)\_AtlBaseModule.GetModuleInstance(),
static\_cast<IConfigTraversAddin\*>(this), addinID, &status);

// Get the current type library version

{

USES\_CONVERSION;

CComBSTR bstrNum;

std::string strNum;

char \*buffer;

iSwApp->RevisionNumber(&bstrNum);

strNum = W2A(bstrNum);

m\_swMajNum = strtol(strNum.c\_str(), &buffer,
10 );

m\_swMinNum=0;

}

// Create the addin's user-interface

AddCommandManager();

// Listen for events

\*IsConnected = AttachEventHandlers();

\*IsConnected = VARIANT\_TRUE;

return S\_OK;

}

STDMETHODIMP CConfigTraversAddin::DisconnectFromSW(VARIANT\_BOOL
\* IsDisconnected)

{

// Remove the addin's user-interface

RemoveCommandManager();

// Stop listening for events

\*IsDisconnected = DetachEventHandlers();

iCmdMgr.Release();

// Make sure you release the SOLIDWORKS
pointer last

iSwApp.Release();

return E\_NOTIMPL;

}

// IConfigTraversAddin methods

// Menu and toolbar callbacks

STDMETHODIMP CConfigTraversAddin::ToolbarCallback0(void)

{

// Use ATL
smart pointers

CComPtr<ISldWorks>
  swApp;

CComPtr<IModelDoc2>
 swModel;

swApp = iSwApp;

swApp->get\_IActiveDoc2(&swModel);

if (! swModel)
{

return(S\_OK);

}

CComBSTR
 strModelTitle;

long      nDocumentType;
 // swDocumentTypes\_e

swModel->GetTitle(&strModelTitle);

swModel->GetType(&nDocumentType);

long     lNumConfigurations;

swModel->GetConfigurationCount(&lNumConfigurations);

BSTR\*  aConfigurationNames
= new BSTR[lNumConfigurations];

swModel->IGetConfigurationNames(&lNumConfigurations,
aConfigurationNames);

for (int
i = 0; i < lNumConfigurations; i++) {

CComBSTR
 bstrConfigurationName(aConfigurationNames[i]);

}

delete []
aConfigurationNames;

return(S\_OK);

}

STDMETHODIMP CConfigTraversAddin::ToolbarEnable0(long\*
status)

{

// TODO: Add your implementation code here

\*status = 1;

return S\_OK;

}