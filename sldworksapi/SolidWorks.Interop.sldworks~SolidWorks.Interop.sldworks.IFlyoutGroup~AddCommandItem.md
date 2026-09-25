<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFlyoutGroup~AddCommandItem.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddCommandItem Method (IFlyoutGroup) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFlyoutGroup Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFlyoutGroup.html) : AddCommandItem Method (IFlyoutGroup) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Name*
:   Name of the item to add to the flyout

*HintString*
:   Text displayed in the SOLIDWORKS status bar when the pointer is on the item

*ImageListIndex*
:   Index of the image in the icon list (see **Remarks**)

*CallbackFunction*
:   Function to call when this item is selected (see **Remarks**)

*UpdateCallbackFunction*
:   Optional function that controls the state of the item; if specified, then SOLIDWORKS calls this function before displaying the item

    |  |  |
    | --- | --- |
    | If UpdateCallbackFunction returns... | Then SOLIDWORKS... |
    | 0 | Deselects and disables the item |
    | 1 | Deselects and enables the item; this is the default state if no update function is specified |
    | 2 | Selects and disables the item |
    | 3 | Selects and enables the item |
    | 4 | Hides the item |

    (see **Remarks**)

Adds an item to a flyout menu.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddCommandItem( _    ByVal Name As System.String, _    ByVal HintString As System.String, _    ByVal ImageListIndex As System.Integer, _    ByVal CallbackFunction As System.String, _    ByVal UpdateCallbackFunction As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFlyoutGroup Dim Name As System.String Dim HintString As System.String Dim ImageListIndex As System.Integer Dim CallbackFunction As System.String Dim UpdateCallbackFunction As System.String Dim value As System.Integer   value = instance.AddCommandItem(Name, HintString, ImageListIndex, CallbackFunction, UpdateCallbackFunction) ``` | |

| C# |  |
| --- | --- |
| ``` System.int AddCommandItem(     System.string Name,    System.string HintString,    System.int ImageListIndex,    System.string CallbackFunction,    System.string UpdateCallbackFunction ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int AddCommandItem(  &   System.String^ Name, &   System.String^ HintString, &   System.int ImageListIndex, &   System.String^ CallbackFunction, &   System.String^ UpdateCallbackFunction ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Name*
:   Name of the item to add to the flyout

*HintString*
:   Text displayed in the SOLIDWORKS status bar when the pointer is on the item

*ImageListIndex*
:   Index of the image in the icon list (see **Remarks**)

*CallbackFunction*
:   Function to call when this item is selected (see **Remarks**)

*UpdateCallbackFunction*
:   Optional function that controls the state of the item; if specified, then SOLIDWORKS calls this function before displaying the item

    |  |  |
    | --- | --- |
    | If UpdateCallbackFunction returns... | Then SOLIDWORKS... |
    | 0 | Deselects and disables the item |
    | 1 | Deselects and enables the item; this is the default state if no update function is specified |
    | 2 | Selects and disables the item |
    | 3 | Selects and enables the item |
    | 4 | Hides the item |

    (see **Remarks**)

#### Return Value

Index of the item within the flyout as assigned by SOLIDWORKS

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FlyoutGroup::AddCommandItem.

# ![](dotnetimages/collapse.gif)Example

[Create Flyouts in the CommandManager (C#)](Create_Flyouts_in_the_CommandManager_Example_CSharp.htm)

[Create Flyouts in the CommandManager (VB.NET)](Create_Flyouts_in_the_CommandManager_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

See Add-in Callback and Enable Methods  to learn how to specify CallbackFunction and UpdateCallbackFunction.

Flyouts are created at runtime. Call this method from the callback method defined in [ICommandManager::CreateFlyoutGroup](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICommandManager~CreateFlyoutGroup.html).

 ImageListIndex is 0-based. The size of the index is equal to the number of images in the large or small graphic file for that flyout. See [IFlyoutGroup::LargeIconList](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFlyoutGroup~LargeIconList.html) and [IFlyoutGroup::SmallIconList](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFlyoutGroup~SmallIconList.html) for details.

# ![](dotnetimages/collapse.gif)See Also

####

[IFlyoutGroup Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFlyoutGroup.html)

[IFlyoutGroup Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFlyoutGroup_members.html)

[IFlyoutGroup::RemoveAllCommandItems Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFlyoutGroup~RemoveAllCommandItems.html)

[IFlyoutGroup::RemoveCommandItem Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFlyoutGroup~RemoveCommandItem.html)

[IFlyoutGroup::ReplaceCommandItem Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFlyoutGroup~ReplaceCommandItem.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0