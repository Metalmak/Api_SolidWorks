<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~SendMsgToUser2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SendMsgToUser2 Method (ISldWorks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : SendMsgToUser2 Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Message*
:   Message for user

*Icon*
:   Icon to show in the message box as defined in swMessageBoxIcon\_e

*Buttons*
:   Buttons to show in the message box as defined in swMessageBoxBtn\_e

Displays a message box containing a message to the user, who is required to interact with it before continuing.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SendMsgToUser2( _    ByVal Message As System.String, _    ByVal Icon As System.Integer, _    ByVal Buttons As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim Message As System.String Dim Icon As System.Integer Dim Buttons As System.Integer Dim value As System.Integer   value = instance.SendMsgToUser2(Message, Icon, Buttons) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SendMsgToUser2(     System.string Message,    System.int Icon,    System.int Buttons ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SendMsgToUser2(  &   System.String^ Message, &   System.int Icon, &   System.int Buttons ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Message*
:   Message for user

*Icon*
:   Icon to show in the message box as defined in swMessageBoxIcon\_e

*Buttons*
:   Buttons to show in the message box as defined in swMessageBoxBtn\_e

#### Return Value

Value corresponding to the button the user clicked as defined in swMessageBoxResult\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::SendMsgToUser2.

# ![](dotnetimages/collapse.gif)Example

[Access Assembly (C++)](Access_Assembly_Example_CPlusPlus_COM.htm)

[Detecting In-context Edit (C++)](Get_Edit_In_Context_Example_CPlusPlus_COM.htm)

[Access Selections (VBA)](Access_Selections_Example_VB.htm)

[Save Drawing As DXF (VBA)](Save_Drawing_as_DXF_Example_VB.htm)

[Save Drawing as DXF (VB.NET)](Save_Drawing_as_DXF_Example_VBNET.htm)

[Save Drawing as DXF (C#)](Save_Drawing_as_DXF_Example_CSharp.htm)

[Get Names of Configurations Using Variant (C++)](ConfigurationTraversalCPP.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)