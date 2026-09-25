<!-- source: sldworksapi/Display_of_Item_in_Feature_Manager_Example_CPlusPlus_COM.htm -->

# SOLIDWORKS API Help

# Display of Item in FeatureManager Design Tree Example (C++ COM)

This example shows how to change the visibility
of features in the FeatureManager design tree. Import
swconst.tlb.

ToggleFeatureManagerItemDisplay()

{

 VARIANT\_BOOL
flag;

 HRESULT
hres;

 LPMODELDOC2
pModelDoc = NULL;

 hres
= m\_pSldWorks->get\_IActiveDoc2(&pModelDoc);

  if
(S\_OK == hres && pModelDoc != NULL)

 {

  //
Get the Selection Manager

  LPSELECTIONMGR
SelectionMgr = NULL;

  hres
= pModelDoc->get\_ISelectionManager(&SelectionMgr);

  if
(S\_OK != hres || SelectionMgr == NULL )

   return;

  long
numSelObjects;

  hres
= SelectionMgr->GetSelectedObjectCount
( &numSelObjects );

   if
(S\_OK != hres || S\_OK== hres && numSelObjects == 0 )

   return;

  LPUNKNOWN
pSelObject;

  long
index;

  long
SelType;

   for
(index=1; index <= numSelObjects; index++)

  {

   if(S\_OK
== SelectionMgr->GetSelectedObjectType2(index,&SelType))

   {

    if(
SelType == swSelBODYFEATURES ||

     SelType
== swSelDATUMAXES  ||

     SelType
== swSelDATUMPLANES  ||

     SelType
== swSelDATUMPOINTS  ||

     SelType
== swSelMATES  ||

     SelType
== swSelREFCURVES  ||

     SelType
== swSelREFERENCECURVES ||

     SelType
== swSelREFSURFACES  ||

     SelType
== swSelSKETCHES )

    {

     if(S\_OK
== SelectionMgr->IGetSelectedObject3(
index,

        &pSelObject
) && pSelObject != NULL)

     {

      LPFEATURE
pFeature;

      if(S\_OK
== pSelObject->QueryInterface(IID\_IFeature,

           (void\*\*)&pFeature))

      {

       //
Determine if the feature is hidden in the

       //
FeatureManager design tree

       if(S\_OK
== pFeature->GetUIState(

         swIsHiddenInFeatureMgr,
&flag))

       {

        //
If feature is hidden in the

        //
FeatureManager design tree, display it,

        //
otherwise, hide it.

        if
(flag)

        {

pFeature->SetUIState(

          swIsHiddenInFeatureMgr,

          FALSE);

        }else{

         pFeature->SetUIState(

          swIsHiddenInFeatureMgr,
TRUE);

        }

       }

      }

     }

    }

   }

  }

  //
Update the Feature Manager Window by performing a Rebuild on the Doc Type

  long
doctype;

  hres
= pModelDoc->GetType(&doctype);

  if
(doctype == swDocPART )

  {

   LPPARTDOC
pPartDoc = NULL;

   //
Retrieve IPartDoc pointer

   hres
= pModelDoc->QueryInterface(IID\_IPartDoc, (LPVOID \*)&pPartDoc);

   ASSERT(
hres == S\_OK );

   hres
= pPartDoc->EditRebuild();

   //
clean up

   pPartDoc->Release();
// Release the IPartDoc pointer

  }

  else
if (doctype == swDocASSEMBLY)

  {

   LPASSEMBLYDOC
pAssemblyDoc = NULL;

   //
Retrieve IAssemblyDoc pointer

   hres
= pModelDoc->QueryInterface(IID\_IAssemblyDoc,

         (LPVOID
\*)&pAssemblyDoc);

   ASSERT(
hres == S\_OK );

   hres
= pAssemblyDoc->EditRebuild();

   //
clean up

  pAssemblyDoc->Release();
// Release the IAssemblyDoc pointer

  }

  else
if (doctype == swDocDRAWING)

  {

   LPDRAWINGDOC
pDrawingDoc = NULL;

   //
Retrieve IDrawingDoc pointer

   hres
= pModelDoc->QueryInterface(IID\_IDrawingDoc,

         (LPVOID
\*)&pDrawingDoc);

   ASSERT(
hres == S\_OK );

   hres
= pDrawingDoc->EditRebuild();

   //
clean up

   pDrawingDoc->Release();
// Release the IDrawingDoc pointer

  }

  pModelDoc->Release();
// Release the IModelDoc pointer

 }

}