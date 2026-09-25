<!-- source: emodelapi/GettingStarted-emodelapi.html -->

![](images/collapse.gif)
![](images/expand.gif)
![](images/copycode.gif)
![](images/copycodeHighlight.gif)
![](images/drpdown.gif)
![](images/drpdown_orange.gif)

|  |
| --- |
|  |

|  |  |
| --- | --- |
| eDrawings API Help |  |
| Getting Started |
| Send Feedback | |

Glossary Item Box

#### Using the eDrawings ActiveX control

The eDrawings API is implemented as a Microsoft ActiveX control.

##### Prerequisites

* Microsoft Visual Studio is installed.* eDrawings 20*nn* is installed.

###### Manually generate eDrawings x64 primary interop assembly DLL

You must manually generate the 64-bit primary interop assembly DLL needed by your Microsoft Visual Studio C# Windows Forms Application, because Microsoft Visual Studio is a 32-bit application.

Procedure 1: Generate the 64-bit primary assembly DLL:

1. Install eDrawings 20*nn* x64 Edition, if it is not already installed on your computer.- Locate **tlbimp.exe** on your computer For:
     * .NET Framework 4 and later, which use CLR 4.0, the path is **C:\Program Files (x86)\Microsoft SDKs\Windows\v7.0A\Bin\NETFX 4.0 Tools.*** .NET Framework 3.5 and earlier, which use CLR 2.0, the path is **C:\Program Files (x86)\Microsoft Visual Studio 8\SDK\v2.0\Bin.**- Open a command prompt window in the folder where **tlbimp.exe** resides and type:

       **tlbimp.exe "C:\Program Files\SOLIDWORKS Corp\eDrawings\EModelView.dll"

       NOTE:** If eDrawings 20*nn* x64 Edition is installed elsewhere on your computer, then specify your path to **EModelView.dll**.- Examine the command window to verify that **Type library imported to EModelView.dll** is returned.- Type **exit**.

###### Modify SOLIDWORKS eDrawings x64 C# example

Contact SOLIDWORKS API Support to obtain the **eDrawings Example.zip**, which includes two Microsoft Visual Studio projects written in C# that you will modify in the following two procedures.

Procedure 2: Modify the SOLIDWORKS eDrawings x64 Host Control C# example

1. Unzip and extract **eDrawingHostControl source project.zip**, located in the **HostControl** folder.- Open **eDrawingHostControl.csproj** in Microsoft Visual Studio and convert the project.- Click the **Show All Files** button in the Solution Explorer and expand **References**.- Remove the existing reference to **EModelView** and add a reference to **EModelView.dll**, which you created in the [first procedure](#first) and which resides in the same folder as **tlbimp.exe**.- Click **Project > eDrawingHostControl Properties**.
           1. Click **Build** and change **Platform target** to **x64.**- If you created **EModelView.dll** using .NET Framework 4 or later, click **Application,**change **Target framework** to .**NET Framework 4.***n,* and click **Yes.**- Start debugging.- Click **Yes** when informed of different versions.- Click **Close** on the form.- Save and exit the project.

Procedure 3: Modify the SOLIDWORKS eDrawings x64 C# example

1. Open **eDrawingsExample.csproj** in Microsoft Visual Studio and convert the project.

   **NOTE**: This project is located in the **eDrawingsExample** folder.
   - Click **Project > eDrawingsExample Properties > Build**  and change **Platform target** to **x64**.- Click the **Show All Files** button in the Solution Explorer and expand **References**.- Remove the existing **eDrawingHostControl** reference and add a reference to **\bin\Debug\eDrawingHostControl.dll**, which you created in the [second procedure](#second). Check the date on the file to ensure that you are adding the DLL that you created.- Remove the reference to **Interop.EModelView** and add a reference to **EModelView.dll**, which youcreated in the [first procedure](#first).- Change the name of the SOLIDWORKS or eDrawings file to open in **Form1.cs** to a file that exists on your computer.- Start debugging.- Click **Yes** when informed of different versions.- Click **Open** to open the file.- Click **OK** to close the message box.- Close the form, save, and exit the project.

###### Create a C# eDrawings x64 project

1. Create an eDrawings x64 **EModelView.dll**. See the [first procedure](#first).- Modify the SOLIDWORKS eDrawings x64 Host Control example's Host Control project. See the [second procedure](#second).- Open Microsoft Visual Studio.- Create a C# **Windows Forms Application** project and name it **WindowsFormsApplication1**.- Click **Project > **WindowsFormsApplication1** Properties**.
           1. Click **Build** and change **Platform target** to **x64.**- If you created **EModelView.dll** using .NET Framework 4 or later, click **Application**, change **Target framework** to .**NET Framework 4.***n,* and click **Yes.**- Click the **Show All Files** button in the Solution Explorer and expand **References**.- Add a reference to **EModelView.dll**, which youcreated in step 1.- Add a reference to **\bin\Debug\eDrawingHostControl.dll**, which you created in step 2. Check the date on the file to ensure that you are adding the DLL that you created.- Double-click **Form1.cs** in the Solution Explorer to show the form.- Click **View > Toolbox**, expand **All Windows Forms**, and drag a button onto the form.- Double-click the button.- Replace the code in **Form1.cs** with this code:

                         ```
                         using System.Data;
                         using System.Drawing;
                         using System.Linq;
                         using System.Text;
                         using System.Threading.Tasks;
                         using System.Windows.Forms;
                         using eDrawingHostControl;
                         ```

                         ```
                         namespace WindowsFormsApplication1
                         {
                             public partial class Form1 : Form
                             {
                                 eDrawingHostControl.eDrawingControl ctrl = null;
                         ```

                         ```
                                 public Form1()
                         ```

                         ```
                                 {
                                     InitializeComponent();
                                     if (null == ctrl)
                                     {
                                         ctrl = new eDrawingControl();
                                     }
                         ```

                         ```
                                     this.Controls.Add(ctrl);
                         ```

                         ```
                                 }
                         ```

                         ```
                                 private void Form1_Load(object sender, System.EventArgs e)
                                 {
                                 }
                         ```

                         ```
                                 private void button1_Click(object sender, System.EventArgs e)
                                 {
                                     if(ctrl != null)
                                     {
                                     ctrl.Location = new Point(0,0);
                                     ctrl.Size = new System.Drawing.Size(this.Size.Width,this.Size.Height);
                                     ctrl.eDrawingControlWrapper.OpenDoc("C:\\Users\\Public\\Documents\\SOLIDWORKS\\SOLIDWORKS 2020\\samples\\tutorial\\EDraw\\claw\\claw.sldprt", false, false, false, "");
                                     }
                                 }
                             }
                         }
                         ```

                         - Start debugging to display the form.- Click **button1**.
                             If the file specified in **button1\_Click** exists on your computer, it is displayed. If that file does not exist on your computer, then close the form, edit the file's path and file name in **Form1.cs** to specify a SOLIDWORKS or eDrawings file on your computer, and repeat steps 13 and 14.- Close the form and save the project.

You can also ask SOLIDWORKS API Support to give you the sample, **Add eModelViewControl to a Windows.Forms Application at runtime (eDrawings ActiveX Control)**, which shows how to add instances of the eDrawings ActiveX control IEModelViewControl to a Window.Forms application at runtime. This technique allows Microsoft Visual Studio users to overcome the architecture mismatch that prevents the 32-bit Visual Studio Forms Editor from loading the 64-bit eDrawings library eModelView.dll.

[Back to top](GettingStarted-emodelapi.html#top)

###### Instantiating the eDrawings Control

You can instantiate the eDrawings control using version-specific or version-independent class IDs (CLSIDs).

To get your version-specific eDrawings control's CLSIDs:

1. Run the Windows Registry editor, regedit.- Expand **HKEY\_CLASSES\_ROOT**.- Locate and double-click **EModelView.EModelViewControl**.*nn*, where *nn* is the 2-digit release year of the version of eDrawings installed on your computer. For example, if eDrawings 2017 is installed on your computer, then nn is 17.- Click **CLSID**. Make note of the CLSID.- Locate and double-click EModelViewMarkup.EModelMarkupControl.nn.- Click **CLSID**. Make note of the CLSID.- Exit regedit.

The version-independent eDrawings CLSIDs are:

* EModelNonVersionSpecificViewControl = 22945A69-1191-4DCF-9E6F-409BDE94D101

  * EModelNonVersionSpecificMarkupControl = 5BBBC05A-BD4D-4e3b-AD5B-51A79DFC522F

SOLIDWORKS recommends that you use version-specific CLSIDs, because Microsoft Visual Studio selects them by default. However, because CLSIDs are version specific, with each new release of eDrawings you must edit:

* your application.

  * any HTML pages that reference version-specific CLSIDs.

Although you do not need to edit your application when working with multiple versions of eDrawings when using the version-independent CLSID, if your application uses a newer API than present in an older version of eDrawings installed by your user, your application will not work properly. This scenario can be difficult to debug remotely, especially with HTML applications.

[Back to top](GettingStarted-emodelapi.html#top)