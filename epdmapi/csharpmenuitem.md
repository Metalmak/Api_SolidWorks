<!-- source: epdmapi/csharpmenuitem.htm -->

# SOLIDWORKS PDM Professional API Help

# Creating Menu Commands (C#)

This topic shows how to create a C#
add-in that adds menu commands to the context-sensitive menus of
File Explorer vault views.

**NOTE:**
Because SOLIDWORKS PDM Professional cannot force a reload of
add-ins if they are written in .NET, all client machines must be restarted to ensure that the latest version of the add-in is used.

1. Start Microsoft Visual Studio.
2. Click **File >** **New >**
   **Project > Visual C# > Windows
   Desktop > Class Library (.NET Framework)**.
3. In the **.NET Framework** dropdown at the top of the
   New Project dialog, keep the default version (recommended) or select another
   version. See [Using .NET
   Framework for Add-in Applications](Using_NET_Framework_in_Addins.htm) for more information.
4. Type a project name in **Name.**
5. Click **Browse** and navigate to the folder where to
   create the project.
6. Click **OK**.
7. Right-click the project name in the Solution Explorer
   and click **Add Reference**.

   1. Click **Browse** in
      the left-side panel, navigate to and select
      **EPDM.Interop.epdm.dll**, and click
      **OK**.
   2. Right-click **E****pdm.Interop.epdm** in the Solution Explorer,
      select **Properties**, and set **Embed Interop Types** to **False**
      to handle methods that pass arrays of structures.
   3. Click **Assemblies > Framework** in the left-hand panel,
      select
      **System.Windows.Forms**, and click **OK**.
   4. Click **Close**.
8. Right-click the project name in the Solution Explorer
   and click **Properties**.

   1. On the Application tab, click **Assembly Information**.
   2. De-select
      **Make assembly COM-Visible****.**
   3. #### On the Build tab, select **Any CPU** for Platform target, de-select **Prefer 32-bit**, and select Register for COM interop.- Save the project.
9. Double-click **Class1.cs** in the Solution Explorer
   to open the code window.
10. At the top of the code window, type:

    using EPDM.Interop.epdm;
    using System.Runtime.InteropServices;
    using System.Windows.Forms;
11. Replace**:**

    ```
    public class Class1
    ```

    with:

    [Guid(""),
    ComVisible(true)]

    public class Class1 : IEdmAddIn5
12. To populate the GUID
    attribute above, click **Tools > Create GUID** in the IDE, select GUID
    Format 5, click **Copy**, and click **Exit**. Populate [Guid(""),
    ...] with the copied string.
13. Implement
    [IEdmAddIn5::GetAddInInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5~GetAddInInfo.html)
    by adding the following code to Class1:
> public void GetAddInInfo(ref EdmAddInInfo poInfo, IEdmVault5 poVault, IEdmCmdMgr5 poCmdMgr)
> {
>        //Specify
> information to
> display in the add-in's Properties dialog box
>        poInfo.mbsAddInName = "Menu command sample";
>        poInfo.mbsCompany = "SOLIDWORKS Corporation";
>        poInfo.mbsDescription = "Adds menu command items";
>        poInfo.mlAddInVersion = 1;
>
>
> //Specify the
> minimum required version of SOLIDWORKS PDM
> Professional
>        poInfo.mlRequiredVersionMajor = 5;
>        poInfo.mlRequiredVersionMinor = 2;
>
>        //Register
> menu commands; SOLIDWORKS PDM Professional passes command IDs, 1000 and 1001,
>        //to IEdmAddIn5::OnCmd to indicate which command the
> user selects
>        poCmdMgr.AddCmd(1000, "First command", (int)EdmMenuFlags.EdmMenu\_Nothing, "This is the first command", "First command", 0, 99);
>        poCmdMgr.AddCmd(1001, "Second command", (int)EdmMenuFlags.EdmMenu\_MustHaveSelection, "This is the second command", "Second command", 1, 99);
> }
>
> The flag
>
>
> [EdmMenuFlags.EdmMenu\_MustHaveSelection](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmMenuFlags.html)
> means that
> the second command is only available if the user has selected one or more
> files or folders.

14. [IEdmAddIn5::OnCmd](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5~OnCmd.html)
    is called when a menu command is selected by the user.

    Implement

    IEdmAddIn5::OnCmd

    by adding
    the following code to Class1:

public void OnCmd(ref EdmCmd poCmd, ref EdmCmdData[] ppoData)
      {
        //Handle
the menu command
        {
                string CommandName = null;
                if (poCmd.mlCmdID == 1000)
                {
                    CommandName = "The first command.";
                }
                else
                {
                    CommandName = "The second command.";
                }
                //Retrieve the bounds of the array containing the selected files and folders
                int index = 0;
                int last = 0;
                index = ppoData.GetLowerBound();
                last = ppoData.GetUpperBound();
                string StrID = null;

                //Create a message showing the names and IDs of all selected files and folders
                string message = null;
                message = "You have selected the following files and folders: " + "\r\n";
                while (index <= last)
                {
                    if (((EdmCmdData)ppoData.GetValue(index)).mlObjectID1 == 0)
                    {
                        message = message + "Folder: (ID=";
                        StrID = ((EdmCmdData)ppoData.GetValue(index)).mlObjectID2.ToString();
                        message = message + StrID + ") ";
                    }
                    else
                    {
                        message = message + "File: (ID=";
                        StrID = ((EdmCmdData)ppoData.GetValue(index)).mlObjectID1.ToString();
                        message = message + StrID + ") ";
                    }

                    message = message + ((EdmCmdData)ppoData.GetValue(index)).mbsStrData1 + "\r\n";
                    index = index + 1;
                }

                //Display the message
                EdmVault5 v = default(EdmVault5);
                v = (EdmVault5)poCmd.mpoVault;
                v.MsgBox(poCmd.mlParentWnd, message, EdmMBoxType.EdmMbt\_OKOnly, CommandName);
        }
      }

15. Click **Build > Build
    Solution** to build the add-in.
16. Install
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
       click *project\_name***.dll** and **EPDM.Interop.**e**pdm.dll**.
    5. Click **Open**.
    6. Click **OK**.
    7. Click **OK**.
17. Right-click inside a vault view in
    File Explorer. **First command** appears in the context-sensitive
    menu.
18. Right-click a file in
    the vault view and click **Second
    command**. The add-in displays a dialog similar to the following:

>  ![](SecondCommand.gif)
>
>
>
> ## **Complete Source Code**
>
> > #### // Class1.cs
> >
> > using System;
> > using System.Collections.Generic;
> > using System.Text;
> > using EPDM.Interop.epdm;
> >
> > using System.Runtime.InteropServices;
> >
> >
> > namespace CreateMenuCommand\_CSharp
> > {
> >
> >     [Guid(""),
> > ComVisible(true)]
> > // See step 13 above to create the GUID
> >     public class Class1 : IEdmAddIn5
> >     {
> >         #region IEdmAddIn5 Members
> >
> >         public void GetAddInInfo(ref EdmAddInInfo poInfo, IEdmVault5 poVault, IEdmCmdMgr5 poCmdMgr)
> >         {
> >
> >             poInfo.mbsAddInName = "Menu command sample";
> >             poInfo.mbsCompany = "SOLIDWORKS Corporation";
> >             poInfo.mbsDescription = "Adds menu command items";
> >             poInfo.mlAddInVersion = 1;
> >             poInfo.mlRequiredVersionMajor = 5;
> >             poInfo.mlRequiredVersionMinor = 2;
> >
> >
> >             poCmdMgr.AddCmd(1000, "First command", (int)EdmMenuFlags.EdmMenu\_Nothing, "This is the first command", "First command", 0, 99);
> >             poCmdMgr.AddCmd(1001, "Second command", (int)EdmMenuFlags.EdmMenu\_MustHaveSelection, "This is the second command", "Second command", 1, 99);
> >         }
> >
> >         public void OnCmd(ref EdmCmd poCmd, ref EdmCmdData[] ppoData)
> >         {
> >
> >             {
> >                 string CommandName = null;
> >                 if (poCmd.mlCmdID == 1000)
> >                 {
> >                     CommandName = "The first command.";
> >                 }
> >                 else
> >                 {
> >                     CommandName = "The second command.";
> >                 }
> >
> >                 int index = 0;
> >                 int last = 0;
> >                 index = Information.LBound(ppoData);
> >                 last = Information.UBound(ppoData);
> >                 string StrID = null;
> >
> >
> >                 string message = null;
> >                 message = "You have selected the following files and folders: " + "\r\n";
> >                 while (index <= last)
> >                 {
> >                     if (((EdmCmdData)ppoData.GetValue(index)).mlObjectID1 == 0)
> >                     {
> >                         message = message + "Folder: (ID=";
> >                         StrID = ((EdmCmdData)ppoData.GetValue(index)).mlObjectID2.ToString();
> >                         message = message + StrID + ") ";
> >                     }
> >                     else
> >                     {
> >                         message = message + "File: (ID=";
> >                         StrID = ((EdmCmdData)ppoData.GetValue(index)).mlObjectID1.ToString();
> >                         message = message + StrID + ") ";
> >                     }
> >
> >                     message = message + ((EdmCmdData)ppoData.GetValue(index)).mbsStrData1 + "\r\n";
> >                     index = index + 1;
> >                 }
> >
> >
> >                 EdmVault5 v = default(EdmVault5);
> >                 v = (EdmVault5)poCmd.mpoVault;
> >                 v.MsgBox(poCmd.mlParentWnd, message, EdmMBoxType.EdmMbt\_OKOnly, CommandName);
> >             }
> >         }
> >
> >         #endregion
> >     }
> > }