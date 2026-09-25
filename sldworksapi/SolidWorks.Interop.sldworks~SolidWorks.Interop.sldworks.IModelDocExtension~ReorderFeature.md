<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~ReorderFeature.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ReorderFeature Method (IModelDocExtension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : ReorderFeature Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FeatureToMove*
:   Name of feature to move

*TargetFeature*
:   Name of feature before or after which to move FeatureToMove; valid only if MoveLocation is swMoveLocation\_e.swMoveAfter

    - or -

    Name of folder; valid only if MoveLocation is swMoveLocation\_e.swMoveToFolder

*MoveLocation*
:   Move type as defined by swMoveLocation\_e

Moves the specified feature to another location in the FeatureManager design tree of this part or assembly.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ReorderFeature( _    ByVal FeatureToMove As System.String, _    ByVal TargetFeature As System.String, _    ByVal MoveLocation As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim FeatureToMove As System.String Dim TargetFeature As System.String Dim MoveLocation As System.Integer Dim value As System.Boolean   value = instance.ReorderFeature(FeatureToMove, TargetFeature, MoveLocation) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ReorderFeature(     System.string FeatureToMove,    System.string TargetFeature,    System.int MoveLocation ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ReorderFeature(  &   System.String^ FeatureToMove, &   System.String^ TargetFeature, &   System.int MoveLocation ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FeatureToMove*
:   Name of feature to move

*TargetFeature*
:   Name of feature before or after which to move FeatureToMove; valid only if MoveLocation is swMoveLocation\_e.swMoveAfter

    - or -

    Name of folder; valid only if MoveLocation is swMoveLocation\_e.swMoveToFolder

*MoveLocation*
:   Move type as defined by swMoveLocation\_e

#### Return Value

True if feature moved successfully, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::ReorderFeature.

# ![](dotnetimages/collapse.gif)Example

[Reorder Features (VBA)](Reorder_Features_Example_VB.htm)

[Reorder Features (VB.NET)](Reorder_Features_Example_VBNET.htm)

[Reorder Features (C#)](Reorder_Features_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

[IPartDoc::ReorderFeature Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc~ReorderFeature.html)

[IAssemblyDoc::ReorderComponents Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~ReorderComponents.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2015 FCS, Revision Number 23.0