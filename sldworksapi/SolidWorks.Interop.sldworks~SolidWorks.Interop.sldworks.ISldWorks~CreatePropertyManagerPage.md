<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~CreatePropertyManagerPage.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreatePropertyManagerPage Method (ISldWorks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : CreatePropertyManagerPage Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Title*
:   Title of the page

*Options*
:   Options as defined in swPropertyManagerPageOptions\_e

*Handler*
:   Pointer to the event handler for this page (IPropertyManagerPage2Handler5)

*Errors*
:   Status of the creation as defined in swPropertyManagerPageStatus\_e

Creates a PropertyManager page.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreatePropertyManagerPage( _    ByVal Title As System.String, _    ByVal Options As System.Integer, _    ByVal Handler As System.Object, _    ByRef Errors As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim Title As System.String Dim Options As System.Integer Dim Handler As System.Object Dim Errors As System.Integer Dim value As System.Object   value = instance.CreatePropertyManagerPage(Title, Options, Handler, Errors) ``` | |

| C# |  |
| --- | --- |
| ``` System.object CreatePropertyManagerPage(     System.string Title,    System.int Options,    System.object Handler,    out System.int Errors ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ CreatePropertyManagerPage(  &   System.String^ Title, &   System.int Options, &   System.Object^ Handler, &   [Out] System.int Errors ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Title*
:   Title of the page

*Options*
:   Options as defined in swPropertyManagerPageOptions\_e

*Handler*
:   Pointer to the event handler for this page (IPropertyManagerPage2Handler5)

*Errors*
:   Status of the creation as defined in swPropertyManagerPageStatus\_e

#### Return Value

[PropertyManager page](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPropertyManagerPage2.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::CreatePropertyManagerPage.

# ![](dotnetimages/collapse.gif)Example

See the [IPropertyManagerPage2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPage2.html) examples.

# ![](dotnetimages/collapse.gif)Example

[Cut Body In Half Using Macro Feature (VBA)](Cut_Body_in_Half_using_Macro_Feature_Example_VB.htm)

[Create PropertyManager Page (VBA)](Create_PropertyManager_Page_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Specify swPropertyManagerPageOptions\_e.swPropertyManagerOptions\_LockedPage in the Options parameter when you create your PropertyManager page. It is important that when a handler (such as IPropertyManagerPage2Handler5::OnButtonPress or IPropertyManagerPage2Handler5::OnClose) is finished and control returns to SOLIDWORKS that the PropertyManager page is still there. If the PropertyManager page is not there, SOLIDWORKS might crash. Some methods try to close the PropertyManager page, but you can avoid this scenario by creating the PropertyManager page as Locked.

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[ISldWorks::ICreatePropertyManagerPage Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~ICreatePropertyManagerPage.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0