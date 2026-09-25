<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomMgr3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| IEdmBomMgr3 Interface | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomMgr3_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : IEdmBomMgr3 Interface |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Allows you to add a SOLIDWORKS Bill of Materials (BOM) to a non-SOLIDWORKS document.
**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Interface IEdmBomMgr3     Inherits IEdmBomMgr, IEdmBomMgr2  ``` | |

| C# |  |
| --- | --- |
| ``` public interface IEdmBomMgr3 : IEdmBomMgr, IEdmBomMgr2  ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IEdmBomMgr3 : public IEdmBomMgr, IEdmBomMgr2  ``` | |

# ![](dotnetimages/collapse.gif)Example

//C# console application:

//----------------------------------------------------------------------------

// Preconditions:

// 1. Start Microsoft Visual Studio.

//    a. Click **File > New > Project > Visual C# > Console Applicat**ion.

//    b. Type Search in Name.

//    c. Click **Browse** and navigate to the folder where to create the project.

//    d. Click **OK**.

//    e. Click **Show All Files** in the Solution Explorer toolbar and expand

//       **Program.cs** in the Solution Explorer.

//    f. Replace the code in **Program.cs** with the code below.

//    g. Change the namespace to match your setup.

// 2. Add **EPDM.Interop.epdm.dll** and **EPDM.Interop.EPDMResultCode** as references
//    (right-click the project name in the Solution Explorer, click **Add Reference**, click

//    **Assemblies > Framework** in the left-side panel, browse to the top folder of

//    your SOLIDWORKS PDM Professional installation, locate and select

//    **EPDM.Interop.epdm.dll**, click **Open**, click **Add**, and click **Close**).

// 3. Change the userName, vaultName, swBom.RefDocID, swBom.RefCfgs, swBom.SheetName,
//    AddSWBom method parameters, and swRow property assignments in the code
//    to match your vault and the document to which you want to add this BOM.

// 4. Click **Debug > Start Debugging** or press F5.

//

// Postconditions: Press a key when prompted in the console.

//----------------------------------------------------------------------------

//Program.cs

using System;

using System.Collections.Generic;

using System.Linq;

using System.Text;

using System.Threading.Tasks;

using EPDM.Interop.epdm;

using EPDM.Interop.EPDMResultCode;

using System.Windows.Forms;

namespace SPR\_1207428

{

  class Program

  {

    const int LVCFMT\_CENTER = 2;

    const int LVCFMT\_RIGHT = 1;

    static string userName = "Admin";

    static string vaultName = "2022\_A1\_B291";

    static void Main(string[] args)

    {

      StringBuilder sb = new StringBuilder();

      try

      {

        sb.AppendFormat("UserName: {0}", userName).AppendLine();

        sb.AppendFormat("VaultName: {0}", vaultName).AppendLine();

        IEdmVault11 vault = (IEdmVault11)(new EdmVault5());

        if (!vault.IsLoggedIn)

          vault.Login(userName, "", vaultName);

        IEdmBomMgr3 bomMgr = (IEdmBomMgr3)vault.**CreateUtility**(EdmUtility.EdmUtil\_BomMgr);

        IEdmSWBom swBom = bomMgr.**CreateEmptySWBom**();

        swBom.**Name** = "Custom SWBom 7";

        swBom.**TableType** = 0;

        swBom.**StartNumber** = 1;

        swBom.**IncrementNumber** = 1;

        swBom.**RefCfgs** = "Default";

        swBom.**RefDocID** = 1553;

        swBom.**SheetName** = "Sheet1";

        IEdmSWBomColumn swColTmp;

        swColTmp = swBom.**InsertColumn**(0, "PART NUMBER");

        swColTmp.**Flags** = LVCFMT\_CENTER;

        swColTmp.**Width** = 120;

        swColTmp.**Type** = 8;

        swColTmp = swBom.**InsertColumn**(1, "DESCRIPTION");

        swColTmp.**Flags** = LVCFMT\_CENTER;

        swColTmp.**Width** = 231;

        swColTmp.**CustomPropName** = "Description";

        swColTmp = swBom.**InsertColumn**(2, "WEIGHT");

        swColTmp.**Flags** = LVCFMT\_CENTER;

        swColTmp.Width = 71;

        swColTmp.**CustomPropName** = "Weight";

        swColTmp = swBom.**InsertColumn**(3, "VENDOR");

        swColTmp.**Flags** = LVCFMT\_CENTER;

        swColTmp.**Width** = 132;

        swColTmp.**CustomPropName** = "Vendor";

        swColTmp = swBom.**InsertColumn**(4, "QTY.");

        swColTmp.**Flags** = LVCFMT\_RIGHT;

        swColTmp.**Width** = 71;

        swColTmp.**Type** = 6;

        swColTmp = swBom.**InsertColumn**(0, "ITEM NO."); // insert at first position; reorders previous indexing

        swColTmp.**Flags** = LVCFMT\_CENTER;

        swColTmp.**Width** = 71;

        swColTmp.**Type** = 7;

        IEdmSWBomRow swRow = swBom.**InsertRow**(0);

        swRow.**DocID** = 1556;

        swRow.**Configuration** = "Default";

        swRow.**Version** = 1;

        swRow.**ProjectID** = 7;

        //swRow.ComponentRep = "SW-100200-2<Default>@Bill of Materials1/SW-100217-1<Default>@SW-100200/SW-201831-1<Default>@SW-100217";

        swBom.**GetCell**(0, 0).Text = "1";  //Item number

        swBom.**GetCell**(0, 1).Text = "SW-201831";  //Part number

        swBom.**GetCell**(0, 2).Text = "BASE"; //Description

        swBom.**GetCell**(0, 3).Text = "3696.33"; //Weight

        swBom.**GetCell**(0, 5).Text = "1"; //Quantity

        //Add the new SOLIDWORKS BOM to document with ID=1553 and Version=9

        bomMgr.**AddSWBom**(1553, 7, 9, (EdmSWBom)swBom);

        sb.AppendFormat("{0} sucessfully added.", swBom.**Name**).AppendLine();

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

# ![](dotnetimages/collapse.gif)Remarks

This interface extends [IEdmBomMgr2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomMgr2.html) by providing the ability to:

* create a SOLIDWORKS BOM with rows and columns not tied to a fixed layout.* add a SOLIDWORKS BOM to a non-SOLIDWORKS document in the vault.

To access this interface, call IEdmVault7::CreateUtility with eType = [EdmUtility](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUtility.html).EdmUtil\_BomMgr and then cast the returned object to IEdmBomMgr3.

# ![](dotnetimages/collapse.gif)Accessors

[IEdmVault7::CreateUtility](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault7~CreateUtility.html)

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBomMgr3 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomMgr3_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)