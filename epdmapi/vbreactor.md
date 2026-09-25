<!-- source: epdmapi/vbreactor.htm -->

# SOLIDWORKS PDM Professional API Help

# Creating Add-in Hooks (VB.NET)

This
topic shows how to implement
 [IEdmAddIn5::GetAddInInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5~GetAddInInfo.html)
and  [IEdmAddIn5::OnCmd](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5~OnCmd.html)
in your add-in to have SOLIDWORKS PDM Professional notify your add-in
whenever a file is added, checked out, or checked in.

**NOTE:**
Because SOLIDWORKS PDM Professional cannot force a reload of
add-ins if they are written in .NET, all client machines must be restarted to ensure that the latest version of the add-in is used.

1. Call
   [IEdmCmdMgr5::AddHook](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCmdMgr5~AddHook.html)
   from your add-in's GetAddInInfo
   method
   for each activity you want your add-in to know about. Implement IEdmAddIn5::GetAddInInfo
   in your add-in as follows:
> Public Sub
> GetAddInInfo(ByRef poInfo As EdmAddInInfo, ByVal poVault As IEdmVault5,
> ByVal poCmdMgr As IEdmCmdMgr5) Implements IEdmAddIn5.GetAddInInfo
>
>
> 'Specify
> add-in information
>
> poInfo.mbsAddInName = "My first add-in"
>
> poInfo.mbsCompany = "The name of my company"
>
>
> poInfo.mbsDescription = "This is a very nice add-in."
>
> poInfo.mlAddInVersion = 1
>
>
> 'Specify
> minimum version of SOLIDWORKS PDM Professional
>
> poInfo.mlRequiredVersionMajor = 5
>
> poInfo.mlRequiredVersionMinor = 2
>
>
>
> 'Notify when a file has been added
>   poCmdMgr.AddHook(EdmCmdType.EdmCmd\_PostAdd)
>
>
> 'Notify when a file has been checked out
>   poCmdMgr.AddHook(EdmCmdType.EdmCmd\_PostLock)
>
>
> 'Notify when a file is about to be checked in
>   poCmdMgr.AddHook(EdmCmdType.EdmCmd\_PreUnlock)
>
>   'Notify when a file has been checked in
>   poCmdMgr.AddHook(EdmCmdType.EdmCmd\_PostUnlock)
>
> End Sub

2. Implement
   IEdmAddIn5::OnCmd in
   your add-in as follows:
> Public Sub OnCmd(ByRef
> poCmd As EdmCmd,
>
> ByRef ppoData As EdmCmdData[]) Implements IEdmAddIn5.OnCmd
>
>   'Check the type of hook that
> triggered this call
>   Dim name As String
>
> Select Case poCmd.meCmdType
>     Case EdmCmdType.EdmCmd\_PostAdd
>       name = "PostAdd"
>     Case EdmCmdType.EdmCmd\_PostLock
>       name = "PostLock"
>     Case EdmCmdType.EdmCmd\_PreUnlock
>       name = "PreUnlock"
>     Case EdmCmdType.EdmCmd\_PostUnlock
>       name = "PostUnlock"
>     Case Else
>       name = "?"
>   End Select
>
>   'Check the upper and lower bounds
> of the array
>   Dim message As String
>   message = ""
>   Dim index As Long
>
> index = LBound(ppoData)
>   Dim last As Long
>
> last = UBound(ppoData)
>
>
>
> 'Append the paths of all files to a string
>   While index <= last
>     message = message + ppoData(index).mbsStrData1 + vbLf
>     index = index + 1
>   End While
>
>   'Display a message to the user
>
> message = "The following files were affected by a " + name + "
> hook:" + vbLf + message
>
>
> Dim vault As EdmVault5
>   vault = poCmd.mpoVault
>   vault.MsgBox(poCmd.mlParentWnd, message)
>
> End Sub

OnCmd
is called for each of the
hooks registered in GetAddInInfo. You can tell which hook triggered the call to
OnCmd by
inspecting the meCmdType
member of the [EdmCmd](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd.html) structure
that is passed as poCmd in OnCmd. meCmdType contains an EdmCmdType constant
that indicates the triggering hook.

The second argument to OnCmd
is an array of [EdmCmdData](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdData.html) structures. There is
one element in the array for each file that is affected by the call. The
contents of the structure members vary depending on the type of hook that
is executed. See EdmCmdData for a complete list
of members and their descriptions.

3. Click **Build > Build
   Solution** to build the add-in.
4. Install
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
5. Try adding, checking out, and checking in
   vault files.

**NOTE:**
OnCmd is not called during check-in if the
file is not modified before it is checked in. During check-in of unmodified
files, SOLIDWORKS PDM Professional triggers an "undo check-out" event. To handle
this "undo check-out" event, add hooks for  [EdmCmdType.EdmCmd\_PreUndoLock](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html) and
[EdmCmdType.EdmCmd\_PostUndoLock](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html)
to your add-in's GetAddInInfo.