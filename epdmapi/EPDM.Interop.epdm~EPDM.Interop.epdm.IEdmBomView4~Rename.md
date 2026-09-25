<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomView4~Rename.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| Rename Method (IEdmBomView4) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBomView4 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomView4.html) : Rename Method (IEdmBomView4) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsFileName*
:   New file name of named BOM

Renames this named BOM.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub Rename( _    ByVal bsFileName As System.String _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void Rename(     System.string bsFileName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void Rename(  &   System.String^ bsFileName ) ``` | |

#### Parameters

*bsFileName*
:   New file name of named BOM

# ![](dotnetimages/collapse.gif)Example

//Preconditions:

//1. Create a C# console application in Visual Studio.

//2. Add references EPDM.Interop.epdm and EPDM.Interop.EPDMResultCode to the project.

//3. Copy the code below to Program.cs.

//4. Change the namespace to match your project name.

//5. Add an assembly with a named BOM to your vault.

//6. Ensure that parameters of Login, and GetFileFromPath match your vault.

//7. Modify the Rename method’s parameter to rename your assembly’s named BOM.

//

//Postconditions:

//1. Refresh your vault view.

//2. Select the assembly with the named BOM in the vault.

//3. Observe the renamed BOM in the BOM dropdown on the Bill of Materials tab.

//Program.cs:

using System;

using EPDM.Interop.epdm;
using EPDM.Interop.EPDMResultCode;

using System.Windows.Forms;

namespace project\_name

{

    class Program

    {

        static IEdmVault5 vault1 = null;

        static IEdmFile7 aFile;

        static string userName = "Admin";

        static void Main(string[] args)

        {

            try

            {

                vault1 = new EdmVault5();

                if (!vault1.**IsLoggedIn**)

                    vault1.**Login**(userName, "password", "JEB12");

                IEdmVault7 vault7 = (IEdmVault7)vault1;

                IEdmFolder5 ppoRetParentFolder;

                aFile = (IEdmFile7)vault1.**GetFileFromPath**("C:\\Users\\J4M\\Desktop\\JEB12\\test3.sldasm", out ppoRetParentFolder);

                EdmBomInfo[] derivedBOMs = null;

                aFile.**GetDerivedBOMs**(out derivedBOMs);

                int bomId = derivedBOMs[0].**mlBomID**;

                IEdmBom bom = (IEdmBom)vault7.**GetObject**(EdmObjectType.EdmObject\_BOM, bomId);

                EdmBomVersion[] ppoVersions = null;

                bom.**GetVersions**(out ppoVersions);

                IEdmBomView4 bomView = (IEdmBomView4)bom.**GetView**(ppoVersions[ppoVersions.Length - 1].**mlVersion**);

                bomView.**Rename**("test3\_renamed.sldasm.1.BOM");

                Console.WriteLine("BOM successfully renamed");

                Console.WriteLine("Press any key to exit");

                Console.ReadKey();

            }

            catch (System.Runtime.InteropServices.COMException ex)

            {

                var errorType = typeof(EdmResultErrorCodes\_e);

                if (Enum.IsDefined(errorType, ex.ErrorCode))

                    MessageBox.Show(String.Format("Error occurred: {0}", Enum.GetName(errorType, ex.ErrorCode)));

                else

                    MessageBox.Show("HRESULT = 0x" + ex.ErrorCode.ToString("X") + " " + ex.Message);

            }

            catch (Exception ex)

            {

                MessageBox.Show(ex.Message);

            }

        }

    }

}

# ![](dotnetimages/collapse.gif)Remarks

Named BOMs are saved as:

*file\_name*.sld*ext*.*version*.BOM

Be sure to use the correct format when specifying bsFileName. For example, if you get **assembly.sldasm**, then to rename its BOM set bsFileName to:

    assembly\_renamed.sldasm.1.BOM

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBomView4 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomView4.html)

[IEdmBomView4 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomView4_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2022