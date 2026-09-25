<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserGroup9~SetSettingsVar.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| SetSettingsVar Method (IEdmUserGroup9) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmUserGroup9 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserGroup9.html) : SetSettingsVar Method (IEdmUserGroup9) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*eVar*
:   User group setting as defined by [EdmGroupSetting](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGroupSetting.html)

*pbsVal*
:   Value of eVar

Sets the specified user group setting.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub SetSettingsVar( _    ByVal eVar As EdmGroupSetting, _    ByVal pbsVal As System.String _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void SetSettingsVar(     EdmGroupSetting eVar,    System.string pbsVal ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetSettingsVar(  &   EdmGroupSetting eVar, &   System.String^ pbsVal ) ``` | |

#### Parameters

*eVar*
:   User group setting as defined by [EdmGroupSetting](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGroupSetting.html)

*pbsVal*
:   Value of eVar

# ![](dotnetimages/collapse.gif)Example

//Preconditions:

//1. Create a C# console application in Visual Studio.

//2. Add references EPDM.Interop.epdm and EPDM.Interop.EPDMResultCode to the project.

//3. Copy the code below to Program.cs.

//4. Change the namespace to match your project name.

//5. Open the Admin Tool and add a user “A” and a user group “NewGroup”. Add a user to NewGroup.

//6. Ensure that parameters of Login match your vault.

//

//Postconditions:

//1. Open the Admin Tool.

//2. Inspect the settings of user “A” to verify that reference files are not auto-selected to get latest when user A checks out a file.

//3. Inspect the settings of user group “NewGroup” to verify that reference files are auto-selected to get latest when a user in user group NewGroup checks out a file.

//Program.cs:

using System;

using System.Text;

using EPDM.Interop.epdm;

using EPDM.Interop.EPDMResultCode;

namespace project\_name

{

  class Program

  {

    static string userName = "Admin";

    static string vaultName = "JEB12";

    static string updUser = "A";

    static string updGroup = "NewGroup";

    static void Main(string[] args)

    {

      StringBuilder sb = new StringBuilder();

      try

      {

        sb.AppendFormat("UserName: {0}", userName).AppendLine();

        sb.AppendFormat("VaultName: {0}", vaultName).AppendLine();

        IEdmVault11 vault = (IEdmVault11)(new EdmVault5());

        if (!vault.**IsLoggedIn**)

          vault.**Login**(userName, "password", vaultName);

        IEdmUserMgr9 userMgr = (IEdmUserMgr9)vault.**CreateUtility**(EdmUtility.EdmUtil\_UserMgr);

        var userPos = userMgr.**GetFirstUserPosition**();

        while (!userPos.IsNull)

        {

          IEdmUser11 user = (IEdmUser11)userMgr.**GetNextUser**(userPos);

          if (user.Name == updUser)

          {

            //user.SetSettingsVar(EdmUserSetting.EdmSv\_AutoGetLatest, "1");

            //user.SetSettingsVar(EdmUserSetting.EdmSv\_AutoDelete, "1");

            user.**SetSettingsVar**(EdmUserSetting.EdmUSv\_AutoGetLatestRefs, "0");

            sb.AppendFormat("Settings successfully updated for user {0}", updUser).AppendLine();

            break;

          }

        }

        var groupPos = userMgr.**GetFirstUserGroupPosition**();

        while (!groupPos.IsNull)

        {

          IEdmUserGroup9 group = (IEdmUserGroup9)userMgr.**GetNextUserGroup**(groupPos);

          if (group.Name == updGroup)

          {

            group.**SetSettingsVar**(EdmGroupSetting.EdmGSv\_AutoGetLatestRefs, "1");

            sb.AppendFormat("Settings successfully updated for group {0}", updGroup);

            break;

          }

        }

      }

      catch (System.Runtime.InteropServices.COMException ex)

      {

        var errorType = typeof(EdmResultErrorCodes\_e);

        if (Enum.IsDefined(errorType, ex.ErrorCode))

          sb.AppendFormat("Edm error occurred: {0}", Enum.GetName(errorType, ex.ErrorCode)).AppendLine();

        else

          sb.AppendLine("HRESULT = 0x" + ex.ErrorCode.ToString("X") + " " + ex.Message);

      }

      catch (Exception ex)

      {

        sb.AppendFormat("Error occurred: {0}", ex.Message).AppendLine();

      }

      Console.WriteLine(sb.ToString());

      Console.WriteLine("Please press any key to exit");

      Console.ReadKey();

    }

  }

}

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmUserGroup9 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserGroup9.html)

[IEdmUserGroup9 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserGroup9_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2022