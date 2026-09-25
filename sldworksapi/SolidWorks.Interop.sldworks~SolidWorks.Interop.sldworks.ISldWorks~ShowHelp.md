<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~ShowHelp.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ShowHelp Method (ISldWorks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : ShowHelp Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*HelpFile*
:   Name of the Help file that contains the Help topic

*HelpTopic*
:   ID of Help topic to display

Displays the specified Help topic.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub ShowHelp( _    ByVal HelpFile As System.String, _    ByVal HelpTopic As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim HelpFile As System.String Dim HelpTopic As System.Integer   instance.ShowHelp(HelpFile, HelpTopic) ``` | |

| C# |  |
| --- | --- |
| ``` void ShowHelp(     System.string HelpFile,    System.int HelpTopic ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void ShowHelp(  &   System.String^ HelpFile, &   System.int HelpTopic ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*HelpFile*
:   Name of the Help file that contains the Help topic

*HelpTopic*
:   ID of Help topic to display

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::ShowHelp.

# ![](dotnetimages/collapse.gif)Example

STDMETHODIMP CFuncFeatApp::appCallbackFunction(int cmd,int data,LPDISPATCH dsp, BOOL \*retval)

{

            switch (cmd)

            {

            case     swAppIsNewCmd:

                        \*retval = VARIANT\_True; //Set to True if data is new

                        break;

            case     swAppWhatsNewDescription:

                            m\_iSldWorks->ShowHelp(\_T("name\_of\_your\_Help\_system.chm"), cmd);

                        break;

            case     swAppHelpContext:

                        break;

            }

            return S\_OK;

}

# ![](dotnetimages/collapse.gif)Example

[Call Compiled HTML Help File (C#)](Call_Compiled_HTML_Help_File_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

You can use this method with [ISldWorks::AddCallback](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~AddCallback.html) to implement Interactive What's New for your add-in.

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[ISldWorks::CallBack Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~CallBack.html)

[ISldWorks::RemoveCallback Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~RemoveCallback.html)

[ISldWorks::SetAddinCallbackInfo Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~SetAddinCallbackInfo.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 FCS, Revision Number 14.0