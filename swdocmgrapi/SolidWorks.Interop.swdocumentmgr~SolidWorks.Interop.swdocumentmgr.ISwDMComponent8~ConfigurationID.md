<!-- source: swdocmgrapi/SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMComponent8~ConfigurationID.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Document Manager API Help | Send comments on this topic. |
| ConfigurationID Property (ISwDMComponent8) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdocumentmgr Namespace](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr_namespace.html) > [ISwDMComponent8 Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMComponent8.html) : ConfigurationID Property (ISwDMComponent8) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the ID of the configuration of this component.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` ReadOnly Property ConfigurationID As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwDMComponent8 Dim value As System.Integer   value = instance.ConfigurationID ``` | |

| C# |  |
| --- | --- |
| ``` System.int ConfigurationID {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int ConfigurationID {    System.int get(); } ``` | |

#### Property Value

Configuration ID

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwDMComponent8::ConfigurationID.

# ![](dotnetimages/collapse.gif)Example

[Get Current Name of Configuration of Suppressed Component (VB.NET)](Get_Current_Name_of_Configuration_of_Suppressed_Component_Example_VBNET.htm)

[Get Current Name of Configuration of Suppressed Component (C#)](Get_Current_Name_of_Configuration_of_Suppressed_Component_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

SOLIDWORKS does not update suppressed assembly components with changes that occur in referenced documents. For instance, if a component's configuration is renamed, the suppressed component in the assembly is not updated with the new configuration name.

To find the current configuration name of a suppressed component in an assembly, query the referenced component document for the name of the configuration whose ID matches ISwDMComponent8::ConfigurationID.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwDMComponent8 Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMComponent8.html)

[ISwDMComponent8 Members](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMComponent8_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 SP05, Revision Number 18.5 and SOLIDWORKS 2011 SP01, Revision Number 19.1