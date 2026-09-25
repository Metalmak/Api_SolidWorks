<!-- source: epdmapi/cppreactor.htm -->

# SOLIDWORKS PDM Professional API Help

# Creating Add-in Hooks (C++)

This
topic shows how to implement
 [IEdmAddIn5::GetAddInInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5~GetAddInInfo.html)
and  [IEdmAddIn5::OnCmd](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5~OnCmd.html)
in your add-in to have SOLIDWORKS PDM Professional notify your add-in
whenever a file is added, checked out, or checked in.

1. Call
   [IEdmCmdMgr5::AddHook](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCmdMgr5~AddHook.html) from
   your add-in's GetAddInInfo method
   for each activity you want your add-in to know about. Implement
   IEdmAddIn5::GetAddInInfo in your add-in as follows:
> STDMETHOD(GetAddInInfo)(EdmAddInInfo \* poInfo, IEdmVault5 \* poVault, IEdmCmdMgr5 \* poCmdMgr)
> {
>
> //The AFX\_MANAGE\_STATE macro is needed for MFC applications but should not
>
>    //be used for applications that are MFC-free
>    AFX\_MANAGE\_STATE(AfxGetStaticModuleState());
>
>    if (poInfo == NULL || poCmdMgr == NULL )
>      return E\_POINTER;
>
>    //Return information to the Administrate Add-ins dialog box
>    poInfo->mbsAddInName= SysAllocString( L"My first add-in" );
>    poInfo->mbsCompany = SysAllocString( L"The name of my company" );
>    poInfo->mbsDescription= SysAllocString( L"This is a very nice add-in." );
>    poInfo->mlAddInVersion = 1;
>
>    //SOLIDWORKS PDM Professional 5.2 is
> required to install this add-in
>    poInfo->mlRequiredVersionMajor = 5;
>    poInfo->mlRequiredVersionMinor= 2;
>
>    //Notify when a file has been added
>    poCmdMgr->AddHook( EdmCmd\_PostAdd, NULL );
>
> //Notify when a file has been checked out
>    poCmdMgr->AddHook( EdmCmd\_PostLock, NULL );
>
> //Notify when a file is about to be checked in
>    poCmdMgr->AddHook( EdmCmd\_PreUnlock, NULL );
>
> //Notify when a file has been checked in
>    poCmdMgr->AddHook( EdmCmd\_PostUnlock, NULL );
>
>    return S\_OK;
> }

2. Implement
   IEdmAddIn5::OnCmd in
   your add-in as follows:
> STDMETHOD(OnCmd)(EdmCmd \* poCmd, SAFEARRAY \* \* ppoData)
> {
>
> //The AFX\_MANAGE\_STATE macro is needed for MFC applications but should not
>
>    //be used for applications that are MFC-free
>    AFX\_MANAGE\_STATE(AfxGetStaticModuleState());
>
>    if (poCmd == NULL ||ppoData == NULL)
>      return E\_POINTER;
>
>    //Check the type of hook that triggered
> this call
>    CString oName;
>    switch(poCmd->meCmdType )
>    {
>      case EdmCmd\_PostAdd: oName =
> "PostAdd"; break;
>      case EdmCmd\_PostLock: oName = "PostLock"; break;
>      case EdmCmd\_PreUnlock: oName = "PreUnlock"; break;
>      case EdmCmd\_PostUnlock: oName = "PostUnlock"; break;
>      default: oName = "?"; break;
>    }
>
>    //Obtain a pointer to the array data
>    if( SafeArrayGetDim( \*ppoData ) != 1 )
>      return E\_INVALIDARG;
>
>    EdmCmdData \*poElements = NULL;
>    HRESULT hRes =
> SafeArrayAccessData( \*ppoData, (void\*\*)&poElements );
>    if( FAILED(hRes) )
>      return hRes;
>
>    //Append the paths of all files to a string
>    CString oMessage =
> "The following files were affected by a " + oName + " hook:\n";
>    int iCount=(\*ppoData)->rgsabound->cElements;
>    for( int i =
> 0; i < iCount; ++i )
>    {
>      oMessage += (LPCTSTR)bstr\_t(poElements->mbsStrData1 );
>      oMessage += "\n";
>      ++poElements;
>    }
>
>    //Release the array data and display a message to the user
>    SafeArrayUnaccessData( \*ppoData );
>
>    MessageBox((HWND)poCmd->mlParentWnd, oMessage, "SOLIDWORKS PDM Professional", MB\_OK );
>
>    return S\_OK;
> }
>
>
> OnCmd
> is called for each of the
> hooks registered in GetAddInInfo. You can tell which hook triggered the call by
> inspecting the meCmdType
> member of the [EdmCmd](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd.html) structure
> that is passed as poCmd in OnCmd. meCmdType contains an EdmCmdType constant that
> indicates the triggering hook.
>
> The second argument to OnCmd
> is an array of [EdmCmdData](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdData.html) structures. There is
> one element in the array for each file that is affected by the call. The
> contents of the structure members vary depending on the type of hook that
> triggers the call. See EdmCmdData for a complete list
> of members and their descriptions.

3. Build
   the add-in DLL and
   add it to the file vault
   using the

   [Administration tool](AdminDlg.htm).
4. Try adding, checking out, and checking in
   vault files.

**NOTE:**
OnCmd is not called during check-in if the
file is not modified before it is checked in. During check-in of unmodified
files, SOLIDWORKS PDM Professional triggers an "undo check-out" event. To handle
this "undo check-out" event, add hooks for  [EdmCmdType.EdmCmd\_PreUndoLock](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html) and
[EdmCmdType.EdmCmd\_PostUndoLock](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html)
to your add-in's GetAddInInfo.

## See Also

[Creating Add-ins (C++)](cppaddin.htm)

[Creating Add-in Hooks (VB.NET)](vbreactor.htm)