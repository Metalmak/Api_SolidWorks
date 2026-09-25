<!-- source: epdmapi/csharpreactor.htm -->

# SOLIDWORKS PDM Professional API Help

# Creating Add-in Hooks (C#)

This topic shows how to program
an add-in to have SOLIDWORKS PDM Professional notify your add-in
whenever a file is added, checked out, or checked in to a vault.

**NOTE:**
Because SOLIDWORKS PDM Professional cannot force a reload of
add-ins if they are written in .NET, all client machines must be restarted to ensure that the latest version of the add-in is used.

1. Follow
   [Creating Menu Commands (C#)](csharpmenuitem.htm) to create a basic add-in.
    - In your add-in's
     [IEdmAddIn5::GetAddInInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5~GetAddInInfo.html) implementation, call
     [IEdmCmdMgr5::AddHook](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCmdMgr5~AddHook.html)
     for each SOLIDWORKS PDM Professional activity that you want your add-in to be
     notified about. Implement IEdmAddIn5::GetAddInInfo as follows:
   > public void GetAddInInfo(ref EdmAddInInfo poInfo, IEdmVault5 poVault, IEdmCmdMgr5 poCmdMgr)
   > {
   >        //Specify information to display
   > in the add-in's Properties dialog box
   >        poInfo.mbsAddInName = "My first add-in";
   >        poInfo.mbsCompany = "The name of my company";
   >        poInfo.mbsDescription = "This is a very nice add-in.";
   >        poInfo.mlAddInVersion = 1;
   >
   >        //Specify the
   > minimum required version of SolidWorks PDM
   > Professional
   >        poInfo.mlRequiredVersionMajor = 5;
   >        poInfo.mlRequiredVersionMinor = 2;
   >
   >        //Register hooks
   >
   >        //Notify the add-in when a file has been added
   >        poCmdMgr.AddHook(EdmCmdType.EdmCmd\_PostAdd);
   >
   >        //Notify the add-in when a file has been checked out
   >        poCmdMgr.AddHook(EdmCmdType.EdmCmd\_PostLock);
   >
   >        //Notify the add-in when a file is about to be checked in
   >        poCmdMgr.AddHook(EdmCmdType.EdmCmd\_PreUnlock);
   >
   >        //Notify the add-in when a file has been checked in
   >        poCmdMgr.AddHook(EdmCmdType.EdmCmd\_PostUnlock);
   > }

   - Implement
     [IEdmAddIn5::](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5~OnCmd.html)[OnCmd](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5~OnCmd.html) as follows:
   > public void OnCmd(ref EdmCmd poCmd, ref EdmCmdData[] ppoData)
   > {
   >        //Handle the hook
   >        string name = null;
   >        switch (poCmd.meCmdType)
   >        {
   >            case EdmCmdType.EdmCmd\_PostAdd:
   >                name = "PostAdd";
   >                break;
   >            case EdmCmdType.EdmCmd\_PostLock:
   >                name = "PostLock";
   >                break;
   >            case EdmCmdType.EdmCmd\_PreUnlock:
   >                name = "PreUnlock";
   >                break;
   >            case EdmCmdType.EdmCmd\_PostUnlock:
   >                name = "PostUnlock";
   >                break;
   >            default:
   >                name = "?";
   >                break;
   >        }
   >
   >        //Check the upper and lower bounds of the array
   >        string message = null;
   >        message = "";
   >        int index = 0;
   >        index = ppoData.GetLowerBound();
   >        int last = 0;
   >        last = ppoData.GetUpperBound();
   >
   >        //Append the paths of all files to a message
   > string
   >        while (index <= last)
   >        {
   >            message = message + ((EdmCmdData)(ppoData.GetValue(index))).mbsStrData1 + "\r\n";
   >            index = index + 1;
   >        }
   >
   >        //Display a message to the user
   >        message = "The following files were affected by a " + name + " hook:" + "\r\n" + message;
   >
   >        EdmVault5 vault = default(EdmVault5);
   >        vault = (EdmVault5)poCmd.mpoVault;
   >        vault.MsgBox(poCmd.mlParentWnd, message);
   > }

   SOLIDWORKS PDM Professional calls OnCmd whenever one of the
   hooks registered in GetAddInInfo triggers an event. You can tell which hook
   triggered the call by inspecting
   [EdmCmd](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd.html).meCmdType
   that is returned in OnCmd's poCmd argument. meCmdType contains an
   [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html) constant
   that indicates which hook triggered the call.

   The second argument to OnCmd,
   ppoData, contains an array of
   [EdmCmdData](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdData.html) structures.
   The array contains one structure for each file that is affected by the hook. The
   contents of the structure members vary, depending on the hook. See EdmCmdData for a complete list
   of members and their descriptions.

   - Click **Build > Build
     Solution** to build the add-in.
   - Install
     the add-in through the SOLIDWORKS PDM Professional
     Administration tool:

     1. Open the SOLIDWORKS
        PDM Professional Administration tool.
     2. Expand the vault where
        you want to install this add-in and log in as Admin.
     3. Right-click **Add-ins** and click **New
        Add-in**.
     4. Browse to

        *project\_path**\**project\_name\project\_name***\bin\Debug**,
        click *project\_name***.dll** and **EPDM.Interop.epdm.dll**.
     5. Click **Open**.
     6. Click **OK**.
     7. Click **OK**.
   - Add, check out, or check in
     one or more vault files. A message box displays with the files
     added, checked out, or checked in.

**NOTE:**
OnCmd is not called during check-in if the
file is not modified. During check-in of unmodified
files, SOLIDWORKS PDM Professional triggers an "undo check-out" event. To handle
this "undo check-out" event, register  [EdmCmdType.EdmCmd\_PreUndoLock](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html) and
[EdmCmdType.EdmCmd\_PostUndoLock](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html)
hooks in your add-in's implementation of IEdmAddIn5::GetAddInInfo.