<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~SetComponentIdentifiers.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetComponentIdentifiers Method (IFeatureManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : SetComponentIdentifiers Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Primary*
:   Component identifier as defined by swComponentIdentifier\_e

*Secondary*
:   Component identifier(s) as defined by swComponentIdentifier\_e

*Tertiary*
:   Component identifier(s) as defined by swComponentIdentifier\_e

Allows you to specify the primary, ( secondary ), and < tertiary > elements to display for the components in the FeatureManager design tree.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetComponentIdentifiers( _    ByVal Primary As System.Integer, _    ByVal Secondary As System.Integer, _    ByVal Tertiary As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Primary As System.Integer Dim Secondary As System.Integer Dim Tertiary As System.Integer Dim value As System.Integer   value = instance.SetComponentIdentifiers(Primary, Secondary, Tertiary) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetComponentIdentifiers(     System.int Primary,    System.int Secondary,    System.int Tertiary ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetComponentIdentifiers(  &   System.int Primary, &   System.int Secondary, &   System.int Tertiary ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Primary*
:   Component identifier as defined by swComponentIdentifier\_e

*Secondary*
:   Component identifier(s) as defined by swComponentIdentifier\_e

*Tertiary*
:   Component identifier(s) as defined by swComponentIdentifier\_e

#### Return Value

Result code as defined by swSetComponentIdentifierResult\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::SetComponentIdentifiers.

# ![](dotnetimages/collapse.gif)Example

'VBA

'-------------------------------------------------------
' Preconditions:
' 1. Open *public\_documents***\SOLIDWORKS\SOLIDWORKS 2022\samples\tutorial\smartcomponents\pillow\_block.sldasm**.
' 2. Widen the FeatureManager design tree.
'
' Postconditions: Inspect the FeatureManager design tree and press F5 after each Stop.
'
' Notes: Because the model is used elsewhere, do not save changes.
'-------------------------------------------------------
Option Explicit
Dim swApp As SldWorks.SldWorks
Dim Part As SldWorks.ModelDoc2
Dim swFeatMgr As SldWorks.FeatureManager
Dim compIdentifierRet As Long

Sub main()
    Set swApp = Application.SldWorks
    Set Part = swApp.ActiveDoc
    Set swFeatMgr = Part.FeatureManager

    ' Do show configuration or display state name if only one exists
    swFeatMgr.**HideComponentSingleConfigurationOrDisplayStateNames** = False

    ' Set primary identifier
    compIdentifierRet = swFeatMgr.**SetComponentIdentifiers**(swComponentIdentifier\_ComponentName, 0, 0)
    Stop

    compIdentifierRet = swFeatMgr.**SetComponentIdentifiers**(swComponentIdentifier\_ComponentDescription, 0, 0)
    Stop

    ' Set primary and secondary identifiers
    compIdentifierRet = swFeatMgr.**SetComponentIdentifiers**(swComponentIdentifier\_ComponentName, swComponentIdentifier\_ConfigurationName, 0)
    Stop

    compIdentifierRet = swFeatMgr.**SetComponentIdentifiers**(swComponentIdentifier\_ComponentName, swComponentIdentifier\_ConfigurationDescription, 0)
    Stop

    compIdentifierRet = swFeatMgr.**SetComponentIdentifiers**(swComponentIdentifier\_ComponentName, swComponentIdentifier\_ComponentDescription, 0)
    Stop

    'Set primary, secondary, and tertiary identifiers
    compIdentifierRet = swFeatMgr.**SetComponentIdentifiers**(swComponentIdentifier\_ComponentName, swComponentIdentifier\_ConfigurationName + swComponentIdentifier\_ConfigurationDescription + swComponentIdentifier\_ComponentDescription, swComponentIdentifier\_DisplayStateName)
    Stop

End Sub

# ![](dotnetimages/collapse.gif)Remarks

This method:

* Works in both SOLIDWORKS Desktop and SOLIDWORKS Connected.* Is analogous to right-clicking on the top-level component in the FeatureManager design tree and selecting **Tree Display > Component Name and Description**.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IFeatureManager::ComponentPrimaryIdentifier Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~ComponentPrimaryIdentifier.html)

[IFeatureManager::ComponentSecondaryIdentifier Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~ComponentSecondaryIdentifier.html)

[IFeatureManager::ComponentTertiaryIdentifier Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~ComponentTertiaryIdentifier.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2022 SP01, Revision Number 30.1