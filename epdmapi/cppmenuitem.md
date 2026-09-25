<!-- source: epdmapi/cppmenuitem.htm -->

# SOLIDWORKS PDM Professional API Help

# Creating Menu Commands (C++)

This topic shows how to create a
C++ add-in in Microsoft Visual Studio that adds menu commands to the
context-sensitive and Tools menus of vaults in File
Explorer.

1. Create
   an add-in as described in the [basic framework sample](cppaddin.htm).

3. Replace your add-in's implementation of
    [IEdmAddIn5::GetAddInInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5~GetAddInInfo.html)
   with the following code:

> STDMETHOD(GetAddInInfo)(EdmAddInInfo
> \* poInfo, IEdmVault5 \* poVault, IEdmCmdMgr5 \* poCmdMgr)
> {
>   //The AFX\_MANAGE\_STATE macro is needed for MFC
> applications but should not
>   //be used for applications that are MFC-free.
>   AFX\_MANAGE\_STATE(AfxGetStaticModuleState());
>
>   if (poInfo == NULL || poCmdMgr == NULL )
>     return E\_POINTER;
>
>   //Return some information for the
> Administrate Add-ins dialog box
>  poInfo->mbsAddInName = SysAllocString( L"Menu command
> sample" );
>  poInfo->mbsCompany = SysAllocString( L"SOLIDWORKS Corporation"
> );
>   poInfo->mbsDescription= SysAllocString( L"Adds menu items" );
>  poInfo->mlAddInVersion = 1;
>
>   //SOLIDWORKS PDM Professional
> 5.2 or later is required to
> install this add-in
>  poInfo->mlRequiredVersionMajor = 5;
>  poInfo->mlRequiredVersionMinor = 2;
>
>   //Add a command for each of the buttons
> (the command ID numbers 1000 and 1001 are
>   //arbitrary; SOLIDWORKS PDM Professional
> does not use them; instead, it only passes them to
> your
>   //implementation of OnCmd so that it knows which command was selected)
>   poCmdMgr->AddCmd( 1000, bstr\_t("First command"),
> EdmMenu\_Nothing,
>
>                     bstr\_t("This
> is the first command"),
>
>
> bstr\_t("First command"), -1, 0 );
>
>   poCmdMgr->AddCmd( 1001, bstr\_t("Second command"),
> EdmMenu\_MustHaveSelection,
>
>                     bstr\_t("This
> is the second command"),
>
>
> bstr\_t("Second command"), -1, 0 );
>
>   return S\_OK;
> }
>
> The flag
>  [EdmMenuFlags.EdmMenu\_MustHaveSelection](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmMenuFlags.html)
> indicates that only the second command is available to the user if the user
> selects one or more files or folders.

4. Replace your add-in's implementation of

    [IEdmAdd5::OnCmd](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5~OnCmd.html)
   with the following code:

   > STDMETHOD(OnCmd)(EdmCmd \*
   > poCmd, SAFEARRAY \* \* ppoData)
   > {
   >   //The AFX\_MANAGE\_STATE macro is needed for MFC
   > applications but should not
   >   //be used for applications that are MFC-free
   >   AFX\_MANAGE\_STATE(AfxGetStaticModuleState());
   >
   >   if (poCmd == NULL ||ppoData == NULL)
   >     return E\_POINTER;
   >
   >   //Check the command ID to see which
   > command was selected
   >   //(this only affects the caption of the message box below)
   >   CString oName;
   >   if( poCmd->mlCmdID = = 1000 )
   >     oName = "The first command";
   >   else
   >     oName = "The second command";
   >
   >   if( SafeArrayGetDim( \*ppoData ) != 1 )
   >     return E\_INVALIDARG;
   >
   >   //Get a pointer to the actual array
   > elements
   >   EdmCmdData \*poElements = NULL;
   >   HRESULT hRes = SafeArrayAccessData( \*ppoData, (void\*\*)&poElements
   > );
   >   if( FAILED(hRes) )
   >     return hRes;
   >
   >   //Create a message showing the names and
   > IDs of all selected files and folders
   >   CString oRow;
   >   CString oMessage = "You have selected the following files and
   > folders:\n";
   >   int iCount=(\*ppoData)->rgsabound->cElements;
   >   for( int i = 0; i < iCount; ++i )
   >   {
   >
   >     if(poElements->mlObjectID1 == 0 )
   >     {
   >       oRow.Format( "Folder: (ID= %d)
   > ",poElements->mlObjectID2 );
   >     }
   >     else
   >     {
   >       oRow.Format( "File: (ID= %d)
   > ",poElements->mlObjectID1 );
   >     }
   >     oMessage += oRow + (LPCTSTR)bstr\_t(poElements->mbsStrData1
   > );
   >     oMessage += "\n";
   >     ++poElements;
   >   }
   >
   >   //Release the array data and display the
   > message
   >   SafeArrayUnaccessData( \*ppoData );
   >   MessageBox((HWND)poCmd->mlParentWnd, oMessage, oName, MB\_OK );
   >
   >   return S\_OK;
   > }
5. Save and compile the project.
6. Add the add-in DLL to the
   file vault using the

   [Administration tool](AdminDlg.htm).
7. The first menu command appears in
   the
   context-sensitive and Tools menus of vaults in File Explorer. The second menu command appears in the context-sensitive menus
   only when one or
   more files or folders are selected.
   Right-click a file in the vault
   and select **Second command**. A dialog
   similar to the following is displayed:

   ![](advancedmenu.gif)