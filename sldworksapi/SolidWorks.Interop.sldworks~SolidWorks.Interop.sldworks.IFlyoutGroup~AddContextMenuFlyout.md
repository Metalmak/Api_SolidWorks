<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFlyoutGroup~AddContextMenuFlyout.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddContextMenuFlyout Method (IFlyoutGroup) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFlyoutGroup Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFlyoutGroup.html) : AddContextMenuFlyout Method (IFlyoutGroup) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DocumentType*
:   Type of document as defined in swDocumentTypes\_e

*SelectionType*
:   Type of object as defined in swSelectType\_e

Adds this flyout to the context menus of the specified documents and selections.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddContextMenuFlyout( _    ByVal DocumentType As System.Integer, _    ByVal SelectionType As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFlyoutGroup Dim DocumentType As System.Integer Dim SelectionType As System.Integer Dim value As System.Boolean   value = instance.AddContextMenuFlyout(DocumentType, SelectionType) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool AddContextMenuFlyout(     System.int DocumentType,    System.int SelectionType ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool AddContextMenuFlyout(  &   System.int DocumentType, &   System.int SelectionType ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*DocumentType*
:   Type of document as defined in swDocumentTypes\_e

*SelectionType*
:   Type of object as defined in swSelectType\_e

#### Return Value

True if successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FlyoutGroup::AddContextMenuFlyout.

# ![](dotnetimages/collapse.gif)Example

[Create Flyouts in the CommandManager (C#)](Create_Flyouts_in_the_CommandManager_Example_CSharp.htm)

[Create Flyouts in the CommandManager (VB.NET)](Create_Flyouts_in_the_CommandManager_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

Call this method once for each set of DocumentType and SelectionType parameters.

Context-sensitive menus support only the standard flyout style (swCommandFlyoutStyle\_e.swCommandFlyoutStyle\_Simple), in which there is no immediate action on the main flyout button.

# ![](dotnetimages/collapse.gif)See Also

####

[IFlyoutGroup Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFlyoutGroup.html)

[IFlyoutGroup Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFlyoutGroup_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0