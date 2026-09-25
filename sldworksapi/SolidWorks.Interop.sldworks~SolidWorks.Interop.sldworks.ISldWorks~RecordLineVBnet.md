<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~RecordLineVBnet.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| RecordLineVBnet Method (ISldWorks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : RecordLineVBnet Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*StringLine*
:   Text to write to a VB.NET macro and the SOLIDWORKS journal file

Adds a line of code to a VB.NET macro and the SOLIDWORKS journal file.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function RecordLineVBnet( _    ByVal StringLine As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim StringLine As System.String Dim value As System.Boolean   value = instance.RecordLineVBnet(StringLine) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool RecordLineVBnet(     System.string StringLine ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool RecordLineVBnet(  &   System.String^ StringLine ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*StringLine*
:   Text to write to a VB.NET macro and the SOLIDWORKS journal file

#### Return Value

True if successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::RecordLineVBnet.

# ![](dotnetimages/collapse.gif)Example

[Record Macros (VBA)](Record_Macros_Example_VB.htm)

[Record Macros (VB.NET)](Record_Macros_Example_VBNET.htm)

[Record Macros (C#)](Record_Macros_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method is useful if you want your add-in application to record and play back SOLIDWORKS macros or write to the SOLIDWORKS journal file.

For example, if your add-in application allows end users to change the material specifications associated with a model, then end users may want to be able to record and play back the operation in a macro. This might allow them to easily assign material specifications to a large number of files by playing back the macro.

Text is only written to macros if macro recording is enabled when the method is called ([ISldWorks::Run Command](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~RunCommand.html) swCommands\_RecordPauseMacro ""). Users are prompted to select the type of macros to create when recording is stopped (ISldWorks::Run Command swCommands\_StopMacro "").

For your add-in functionality to be recorded reliably in all macro formats, you should call all three macro-recording methods:

* [ISldWorks::RecordLine](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~RecordLine.html) to record to a **SW VBA Macro (\*.swp)**.

  * ISldWorks::RecordLineVBne to record to a **SW VSTA VB Macro (\*.vbproj)**.

    * [ISldWorks::RecordLineCSharp](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~RecordLineCSharp.html) to record to a **SW VSTA C# Macro (\*.csproj)**.

Exercise caution when recording lines that include string literals. String literals are parsed when the add-in application is compiled and again when the macro is compiled.

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[DSldWorksEvents\_BeginRecordNotifyEventHandler Delegate](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DSldWorksEvents_BeginRecordNotifyEventHandler.html)

[DSldWorksEvents\_EndRecordNotifyEventHandler Delegate](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DSldWorksEvents_EndRecordNotifyEventHandler.html)

[ISldWorks::RunMacro2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~RunMacro2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0