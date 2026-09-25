<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~ComponentReload2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ComponentReload2 Method (IAssemblyDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html) : ComponentReload2 Method (IAssemblyDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Component*
:   [IComponent2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2.html)

*ReadOnly*
:   True to set Component read-only after reload, false to allow write access

*Options*
:   Reload option as defined by swComponentReloadOption\_e

Reloads and/or sets the read-only state of the specified component.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ComponentReload2( _    ByVal Component As System.Object, _    ByVal ReadOnly As System.Boolean, _    ByVal Options As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAssemblyDoc Dim Component As System.Object Dim ReadOnly As System.Boolean Dim Options As System.Integer Dim value As System.Integer   value = instance.ComponentReload2(Component, ReadOnly, Options) ``` | |

| C# |  |
| --- | --- |
| ``` System.int ComponentReload2(     System.object Component,    System.bool ReadOnly,    System.int Options ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int ComponentReload2(  &   System.Object^ Component, &   System.bool ReadOnly, &   System.int Options ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Component*
:   [IComponent2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2.html)

*ReadOnly*
:   True to set Component read-only after reload, false to allow write access

*Options*
:   Reload option as defined by swComponentReloadOption\_e

#### Return Value

Error code as defined by swComponentReloadError\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AssemblyDoc::ComponentReload2.

# ![](dotnetimages/collapse.gif)Example

'VBA

'Preconditions:

'1. Open *public\_documents***\SOLIDWORKS\SOLIDWORKS 2021\samples\tutorial\api\arm2.sldasm**.

'2. Open the Immediate window.

'Postconditions:

' Inspect the Immediate window.

'=============================================

Dim swApp As SldWorks.SldWorks
Dim SWMODEL As SldWorks.ModelDoc2
Dim SWASSY As SldWorks.AssemblyDoc
Dim swcomponent As SldWorks.Component2
Dim Error As swComponentReloadError\_e
Option Explicit
Sub main()
    Set swApp = Application.SldWorks
    Set SWMODEL = swApp.ActiveDoc
    Set SWASSY = SWMODEL
    Set swcomponent = SWASSY.GetComponentByName("secondgrip-1")
    Debug.Print swcomponent.GetPathName
    Error = SWASSY.**ComponentReload2**(swcomponent, True, swComponentReloadOption\_e.swDontReloadOldComponents)
    Debug.Print "Error code: " & Error
End Sub

# ![](dotnetimages/collapse.gif)Remarks

This method is analogous to the Reload dialog that appears when you right-click on an assembly component in the FeatureManager design tree and select **Reload**. For more information, read the **SOLIDWORKS user-interface Help > Fundamentals > Document Basics > Multi-User Environment > Reload** topic.

# ![](dotnetimages/collapse.gif)See Also

####

[IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html)

[IAssemblyDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc_members.html)

[IAssemblyDoc::ReplaceComponents2 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~ReplaceComponents2.html)

[IModelDoc2::ReloadOrReplace Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ReloadOrReplace.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus