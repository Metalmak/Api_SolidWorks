<!-- source: sldworksapi/Create_Toolbars_Example_CPlusPlus_COM.htm -->

# SOLIDWORKS API Help

# Create Toolbars Example (C++ COM)

Toolbars are added automatically by the C++
COM Addin Wizard, so you should examine the code that the wizard generates.
An example is also included in this topic.

ISldWorks::AddToolbar4 takes bitmap filenames as arguments. You can
create those filenames from resources using CreateBitmapFIleFromResource().

//This method adds the user toolbar to the
SOLIDWORKS user interface

void CswSampleAddin::AddToolbar()

{

long docType = swDocTemplateTypePART;

CComBSTR title;

CComBSTR callback;

CComBSTR enable;

CComBSTR tip;

CComBSTR hint;

VARIANT\_BOOL added;

long menuPos = 0; //Not used

title.LoadString(IDS\_TOOLBAR\_TITLE);

CComBSTR smallImageFile, largeImageFile;

bmp->CreateBitmapFileFromResource(IDB\_TOOLBAR\_SMALL,
&smallImageFile);

bmp->CreateBitmapFileFromResource(IDB\_TOOLBAR\_LARGE,
&largeImageFile);

iSwApp->AddToolbar4(addinID,
title, smallImageFile, largeImageFile, menuPos, docType, &toolbarID);

callback.LoadString(IDS\_TOOLBAR\_CALLBACK0);

enable.LoadString(IDS\_TOOLBAR\_ENABLE0);

tip.LoadString(IDS\_TOOLBAR\_TIP0);

hint.LoadString(IDS\_TOOLBAR\_HINT0);

iSwApp->AddToolbarCommand2(addinID,
toolbarID, 0, callback, enable, tip, hint, &added);

iSwApp->AddToolbarCommand2(addinID,
toolbarID, 1, callback, enable, tip, hint, &added);

iSwApp->AddToolbarCommand2(addinID,
toolbarID, 2, callback, enable, tip, hint, &added);