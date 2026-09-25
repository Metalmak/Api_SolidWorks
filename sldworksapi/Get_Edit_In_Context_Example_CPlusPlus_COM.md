<!-- source: sldworksapi/Get_Edit_In_Context_Example_CPlusPlus_COM.htm -->

# SOLIDWORKS API Help

# Detect In-Context Edit Example (C++ COM)

This example shows how to trap an swAssemblyBeginInContextEditNotify
event and examine the document being edited in an assembly.

1. Create a new C++ COM add-in with the Visual Studio.NET COM AppWizard.
2. Select Assembly
   Events on the SwOptions
   page.
3. After the wizard finishes generating code, add
   this code to the specified files.

1. swDocument.h:

SINK\_ENTRY\_EX(ID\_ASSEMBLY\_EVENTS, \_\_uuidof(DAssemblyDocEvents),
swAssemblyBeginInContextEditNotify,OnAssemblyBeginInContextEditNotify)

STDMETHOD(OnAssemblyBeginInContextEditNotify)(LPDISPATCH
newDoc, long docType); //

next to
the other SINK\_ENTRY\_EX and STDMETHOD Declarations

2. swDocument.cpp:

STDMETHODIMP CSwDocument::OnAssemblyBeginInContextEditNotify(LPDISPATCH
newDoc, long docType)

{

ATLTRACE("\tCCSwDocument::OnAssemblyBeginInContextEditNotify
called\n");

CComPtr<IModelDoc2> swModel;

iSwApp->get\_IActiveDoc2(&swModel);

CComPtr<IModelDoc2> swNewModel;

newDoc->QueryInterface(\_\_uuidof(IModelDoc2),
reinterpret\_cast<void\*\*>(&swNewModel));

CComBSTR ContextName;

CComBSTR MainName;

swNewModel->GetTitle(&ContextName);

swModel->GetTitle(&MainName);

CComBSTR message;

message.Append(OLESTR("Main Assembly:
"));

message.Append(MainName);

message.Append(OLESTR("     Component:
"));

message.Append(ContextName);

long res;

iSwApp->SendMsgToUser2(message,0,0,&res);

return S\_OK;

}

4. After loading the add-in, open an assembly, right-click
   a component, and select Edit Part
   or Edit Subassembly. The new method
   OnAssemblyBeginInContextEditNotify that you implemented should be called.