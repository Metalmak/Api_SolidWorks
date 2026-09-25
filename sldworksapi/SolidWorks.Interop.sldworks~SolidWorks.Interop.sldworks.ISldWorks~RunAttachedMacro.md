<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~RunAttachedMacro.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| RunAttachedMacro Method (ISldWorks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : RunAttachedMacro Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FileName*
:   Filename of macro to run (do not include a path)

*ModuleName*
:   Module of specified macro to run

*ProcedureName*
:   Procedure of specified macro to run

Runs the specified attached macro, module, and procedure.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function RunAttachedMacro( _    ByVal FileName As System.String, _    ByVal ModuleName As System.String, _    ByVal ProcedureName As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim FileName As System.String Dim ModuleName As System.String Dim ProcedureName As System.String Dim value As System.Boolean   value = instance.RunAttachedMacro(FileName, ModuleName, ProcedureName) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool RunAttachedMacro(     System.string FileName,    System.string ModuleName,    System.string ProcedureName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool RunAttachedMacro(  &   System.String^ FileName, &   System.String^ ModuleName, &   System.String^ ProcedureName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FileName*
:   Filename of macro to run (do not include a path)

*ModuleName*
:   Module of specified macro to run

*ProcedureName*
:   Procedure of specified macro to run

#### Return Value

True if macro runs, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::RunAttachedMacro.

# ![](dotnetimages/collapse.gif)Example

**Visual Basic for Applications (VBA)**

Create two VBA macros using the following code samples. Attach **RunMacroSub.swp** to the active document's Design Binder. Then run **RunAttachedMacro.swp**.

'--------------------------------------
' RunAttachedMacro.swp
'-------------------------------------
Option Explicit
Dim swApp As SldWorks.SldWorks
Dim boolstatus As Boolean

Sub main()
   Set swApp = Application.SldWorks
   Dim RunMacroError As Long
   boolstatus = swApp.**RunAttachedMacro**("RunMacroSub.swp", "RunMacroSub1", "main")
End Sub

'---------------------------------------
' RunMacroSub.swp'
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

# ![](dotnetimages/collapse.gif)Remarks

An example of an attached macro is a macro that is attached to the active document's Design Binder.

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[ISldWorks::RunMacro2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~RunMacro2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 FCS, Revision Number 17.0