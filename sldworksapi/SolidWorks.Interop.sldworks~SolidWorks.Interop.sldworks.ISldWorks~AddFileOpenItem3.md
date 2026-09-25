<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~AddFileOpenItem3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddFileOpenItem3 Method (ISldWorks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : AddFileOpenItem3 Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Cookie*
:   Cookie specified in ISwAddin::ConnectToSW

*MethodName*
:   Name of the application function used to open the file (see **Remarks**)

*Description*
:   File description displayed in the **Save as type** list

*Extension*
:   File name extensions separated by semicolons

*OptionLabel*
:   Label for your options button or an empty string

*OptionMethodName*
:   Name of the callback method to display a dialog box, which appears when a user clicks your options button or an empty string

Adds file types to the **File > Open** dialog box.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddFileOpenItem3( _    ByVal Cookie As System.Integer, _    ByVal MethodName As System.String, _    ByVal Description As System.String, _    ByVal Extension As System.String, _    ByVal OptionLabel As System.String, _    ByVal OptionMethodName As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim Cookie As System.Integer Dim MethodName As System.String Dim Description As System.String Dim Extension As System.String Dim OptionLabel As System.String Dim OptionMethodName As System.String Dim value As System.Boolean   value = instance.AddFileOpenItem3(Cookie, MethodName, Description, Extension, OptionLabel, OptionMethodName) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool AddFileOpenItem3(     System.int Cookie,    System.string MethodName,    System.string Description,    System.string Extension,    System.string OptionLabel,    System.string OptionMethodName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool AddFileOpenItem3(  &   System.int Cookie, &   System.String^ MethodName, &   System.String^ Description, &   System.String^ Extension, &   System.String^ OptionLabel, &   System.String^ OptionMethodName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Cookie*
:   Cookie specified in ISwAddin::ConnectToSW

*MethodName*
:   Name of the application function used to open the file (see **Remarks**)

*Description*
:   File description displayed in the **Save as type** list

*Extension*
:   File name extensions separated by semicolons

*OptionLabel*
:   Label for your options button or an empty string

*OptionMethodName*
:   Name of the callback method to display a dialog box, which appears when a user clicks your options button or an empty string

#### Return Value

True if the file types are added to the **Save as type** list, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::AddFileOpenItem3.

# ![](dotnetimages/collapse.gif)Example

[Add and Remove Items to File Save As and Open Menus (VB.NET)](Add_and_Remove_Items_to_File_Save_As_and_Open_Menus_VBNET.htm)

[Add and Remove Items to File Save As and Open Menus (C#)](Add_and_Remove_Items_to_File_Save_As_and_Open_Menus_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Call this method in your add-in's ConnectToSW method.

Implement the function specified by MethodName with a string parameter that is the file name.

If your application is unloaded using an add-in, then you must remove any file types added with this method. See [ISldWorks::RemoveFileOpenItem2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~RemoveFileOpenItem2.html).

The callback is called one time if the user:

* Presses the Shift or Ctrl key and selects multiple files to open in the **File > Open** Dialog.* Drags-and-drops files into SOLIDWORKS from either File Explorer or the File Explorer tab in the TaskPane.

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[ISldWorks::RemoveFileOpenItem2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~RemoveFileOpenItem2.html)

[ISldWorks::RemoveFileSaveAsItem2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~RemoveFileSaveAsItem2.html)

[ISldWorks::AddFileSaveAsItem2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~AddFileSaveAsItem2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0