<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~RunMacro2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| RunMacro2 Method (ISldWorks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : RunMacro2 Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FilePathName*
:   Path and filename of the project file containing the macro

*ModuleName*
:   Name of the module in the macro

*ProcedureName*
:   Name of the procedure in the module

*Options*
:   Option as defined swRunMacroOption\_e (supports VBA macros only)

*Error*
:   Error as defined by swRunMacroError\_e (supports VBA macros only)

Runs a macro from a project file.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function RunMacro2( _    ByVal FilePathName As System.String, _    ByVal ModuleName As System.String, _    ByVal ProcedureName As System.String, _    ByVal Options As System.Integer, _    ByRef Error As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim FilePathName As System.String Dim ModuleName As System.String Dim ProcedureName As System.String Dim Options As System.Integer Dim Error As System.Integer Dim value As System.Boolean   value = instance.RunMacro2(FilePathName, ModuleName, ProcedureName, Options, Error) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool RunMacro2(     System.string FilePathName,    System.string ModuleName,    System.string ProcedureName,    System.int Options,    out System.int Error ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool RunMacro2(  &   System.String^ FilePathName, &   System.String^ ModuleName, &   System.String^ ProcedureName, &   System.int Options, &   [Out] System.int Error ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FilePathName*
:   Path and filename of the project file containing the macro

*ModuleName*
:   Name of the module in the macro

*ProcedureName*
:   Name of the procedure in the module

*Options*
:   Option as defined swRunMacroOption\_e (supports VBA macros only)

*Error*
:   Error as defined by swRunMacroError\_e (supports VBA macros only)

#### Return Value

True if macro runs, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::RunMacro2.

# ![](dotnetimages/collapse.gif)Example

**Visual Basic for Applications (VBA)**

1. Create two VBA macros using the following code samples.- Store **RunMacroSub.swp** in **c:\test**.- Run **RunMacro.swp**.

'----------------------------
' RunMacro.swp
'---------------------------

Option Explicit
Dim swApp As SldWorks.SldWorks
Dim boolstatus As Boolean
Sub main()
   Set swApp = Application.SldWorks
   Dim runMacroError As Long
   boolstatus = swApp.**RunMacro2**("c:\test\RunMacroSub.swp", "RunMacroSub1", "main",   swRunMacroUnloadAfterRun, runMacroError)
End Sub

'---------------------------------------
' RunMacroSub.swp
'---------------------------------------
Option Explicit
Dim swApp As SldWorks.SldWorks
Sub alternate()
   Set swApp = Application.SldWorks
   swApp.SendMsgToUser "RunMacroSub1:alternate() called."
End Sub
Sub main()
   Set swApp = Application.SldWorks
   swApp.SendMsgToUser "RunMacroSub1:main() called."
End Sub

**Running a C# DLL from VBA**

boolstatus = Me.swApp.**RunMacro2**('C:\Test\CSharpMacro\SwMacro\bin\Release\CSharpMacro.dll',

 '', 'Main',  swRunMacroOption\_e.swRunMacroDefault, runMacroError)

# ![](dotnetimages/collapse.gif)Remarks

If you specify swRunMacroUnloadAfterRun for Options, then the macro is unloaded from the VBA IDE after running.

Use the path and filename of the compiled DLL for the FilePathName argument for a .NET macro. By default, the procedure is called **Main** in a C# macro. Because C# is case sensitive, you must specify **Main** for ProcedureName in this method.. See **Running a C# DLL from VBA** in the **Example** section.

Running a macro from an add-in application, standalone .exe, or VBA macro is supported. Running a .NET macro from a .NET macro is also supported, but only if both .NET macros were created using the same VSTA version.

See SOLIDWORKS Macros for details.

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[ISldWorks::GetCurrentMacroPathFolder Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetCurrentMacroPathFolder.html)

[ISldWorks::GetCurrentMacroPathName Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetCurrentMacroPathName.html)

[ISldWorks::GetMacroMethods Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetMacroMethods.html)

[ISldWorks::RunAttachedMacro Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~RunAttachedMacro.html)

[ISldWorks::RecordLine Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~RecordLine.html)

[ISldWorks::RecordLineCSharp Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~RecordLineCSharp.html)

[ISldWorks::RecordLineVBnet Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~RecordLineVBnet.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 FCS, Revision Number 17.0