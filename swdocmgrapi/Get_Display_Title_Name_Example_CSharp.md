<!-- source: swdocmgrapi/Get_Display_Title_Name_Example_CSharp.htm -->

# SOLIDWORKS Document Manager API Help

# Get Display Title Name (C#)

This example shows how to get the display title name of a document.

//
=================================================

// Preconditions:

// 1. Read the SOLIDWORKS Document Manager API Getting
Started

//
   topic
and ensure that the required DLLs are registered.

// 2. Copy and paste this code into a C# console
application

//
   in
Microsoft Visual Studio.

// 3. Add the **SolidWorks.Interop.swdocumentmgr.dll** reference to the project:

//
   a.
Right-click the solution in Solution Explorer.

//
   b.
Select **Add Reference**.

//
   c.
Click **Browse**.

//
   d.
Click *install\_dir***\api\redist\SolidWorks.Interop.swdocumentmgr.dll**.

//
   e.
Click **Add**.

//
   f.
Click **Close**.

//
4.
Ensure that **sLicenseKey** and **sDocFileName** point
to valid strings.

//
5.
Open an Immediate window.

//

// Postconditions: Inspect the Immediate window.

// ===================================================

using System;

using System.Collections.Generic;

using System.Diagnostics;

using System.Globalization;

using System.IO;

using System.Linq;

using System.Reflection;

using System.Runtime.CompilerServices;

using System.Security;

using System.Text;

using System.Threading.Tasks;

using Microsoft.VisualBasic;

using SolidWorks.Interop.sldworks;

using SolidWorks.Interop.swdocumentmgr;

using SolidWorks.Interop.swconst;

using System.Runtime.InteropServices;

partial class SolidWorksMacro

{

public void main()

{

SwDMClassFactory swClassFact;

SwDMApplication swDocMgr;

SwDMDocument25 swDoc;

string sLicenseKey;

sLicenseKey = "your\_license\_key";

string sDocFileName;

sDocFileName = "doc\_file\_name";

int nDocType;

nDocType = SwDmDocumentType.swDmDocumentPart;

swClassFact = new SwDMClassFactory();

swDocMgr = swClassFact.GetApplication(sLicenseKey);

SwDmDocumentOpenError retval;

swDoc = swDocMgr.GetDocument(sDocFileName, nDocType, false, retval);

Debug.Print("File = " + swDoc.FullName);

Debug.Print("DisplayTitleName = " + swDoc.**GetDisplayTitleName**);

swDoc.CloseDoc();

}

/// <summary>

///     ''' The
SldWorks swApp variable is pre-assigned for you.

///     '''
</summary>

public SldWorks swApp;

}