<!-- source: sldworksapi/Dynamic_View_Rotation_Example_CPlusPlus_COM.htm -->

# SOLIDWORKS API Help

# Dynamically Rotate Model View Example (C++ COM)

This example shows how to dynamically rotate
a model view. It also shows you how to speed up the process by using the
StartDynamics and StopDynamics calls.

RotateTheView(ISldWorks\* m\_pSldWorks)

{

 LPMODELDOC2
p\_ModelDoc = NULL;

 LPMODELVIEW
p\_ModelView = NULL;

 HRESULT
res = S\_OK;

 //
Retrieve the model document pointer

 res
= m\_pSldWorks->get\_IActiveDoc2(
&p\_ModelDoc );

 if(
res != S\_OK || p\_ModelDoc == NULL )

  return;

  //
Get the active view pointer

 res
= p\_ModelDoc->get\_IActiveView(&p\_ModelView);

 if(
res != S\_OK || p\_ModelView == NULL )

 {

  p\_ModelDoc->Release();

  return;

 }

 int
i;

 //
Prepare view for rotation

 p\_ModelView->StartDynamics();

 for
(i = 1; i < 100; i++)

 {

   p\_ModelDoc->ViewRotateplusy();

 }

 //
End dynamic rotation mode

 p\_ModelView->StopDynamics();

 //
Repaint the screen

 p\_ModelDoc->GraphicsRedraw2();

 //Clean
up

 p\_ModelView->Release();

 p\_ModelDoc->Release();

}