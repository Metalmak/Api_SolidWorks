<!-- source: swdocmgrapi/Open_and_Close_Document_Example_CPlusCPlus_COM.htm -->

# SOLIDWORKS Document Manager API Help

# Open and Close Document Example (C++)

This examples shows how to instantiate a SOLIDWORKS Document Manager
session, open an assembly, get its latest supported SOLIDWORKS version number, list
its external references, and
close it.

#define WIN32\_LEAN\_AND\_MEAN // Exclude rarely used stuff
from Windows headers

#include <stdio.h>

#include <tchar.h>

#define \_ATL\_CSTRING\_EXPLICIT\_CONSTRUCTORS //Some CString
constructors will be explicit

#include <windows.h>

#include <atlbase.h>

#include <iostream>

#include 'safearray.h'

using namespace std;   //Use
the standard C++ libraries for text output

#import 'C:\Program Files\Common Files\SOLIDWORKS Shared\swdocumentmgr.dll'
 raw\_interfaces\_only,
raw\_native\_types, no\_namespace, named\_guids //Change as necessary

int \_tmain(int argc, \_TCHAR\* argv[])

{

> //Initialize COM
>
> CoInitialize(NULL);
>
> CComPtr<ISwDMClassFactory> swClassFact;
>
> CComPtr<ISwDMApplication> swDocMgr;
>
> HRESULT hres = swClassFact.CoCreateInstance(\_\_uuidof(SwDMClassFactory),
> NULL, CLSCTX\_INPROC\_SERVER );
>
> CComBSTR Key = \_T('your\_license\_key');
>  //Specify
> your license key
>
> CComBSTR AsmDoc = \_T('E:\\Assemblies\\Asm\\Assem1.sldasm');
>  //Replace
> with the name of your assembly (assuming it has one or more external references)
>
> swClassFact->GetApplication(Key,
> &swDocMgr);
>
> long ver = -1;
>
> swDocMgr->GetLatestSupportedFileVersion(&ver);
>
> cout <<'The latest supported file version is: '
> << ver << endl;
>
> CComPtr<ISwDMDocument> swDoc;
>
> SwDmDocumentOpenError res;
>
> swDocMgr->GetDocument(AsmDoc,
> swDmDocumentAssembly,VARIANT\_TRUE,  &res,
> &swDoc);
>
> CComPtr<ISwDMSearchOption> pSrcOpt;
>
> VARIANT Files;
>
> swDocMgr->GetSearchOptionObject(&pSrcOpt);
>
> swDoc->GetAllExternalReferences(pSrcOpt,
> &Files);
>
> SafeBSTRArray FilesArray(&Files);
>
> CComBSTR Ref1 = FilesArray[0];  //First
> file reference (no particular order)
>
> swDoc->CloseDoc();
>
> //Release references
>
> pSrcOpt = NULL;
>
> swDoc = NULL;
>
> swDocMgr = NULL;
>
> swClassFact = NULL;
>
> //Uninitialize COM
>
> CoUninitialize();
>
> return 0;

}