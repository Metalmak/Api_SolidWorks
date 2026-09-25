<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~GetSelections3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetSelections3 Method (IMacroFeatureData) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IMacroFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData.html) : GetSelections3 Method (IMacroFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Objects*
:   Array of selected objects

*ObjectTypes*
:   Array of selected object types as defined in swSelectType\_e

*SelMarks*
:   Array of marks for the selected objects

*DrViews*
:   Array of [drawing views](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView.html)

*ComponentXForms*
:   Array of [transforms](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathTransform.html) for the selections' components

Gets the selected objects for the macro feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetSelections3( _    ByRef Objects As System.Object, _    ByRef ObjectTypes As System.Object, _    ByRef SelMarks As System.Object, _    ByRef DrViews As System.Object, _    ByRef ComponentXForms As System.Object _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMacroFeatureData Dim Objects As System.Object Dim ObjectTypes As System.Object Dim SelMarks As System.Object Dim DrViews As System.Object Dim ComponentXForms As System.Object   instance.GetSelections3(Objects, ObjectTypes, SelMarks, DrViews, ComponentXForms) ``` | |

| C# |  |
| --- | --- |
| ``` void GetSelections3(     out System.object Objects,    out System.object ObjectTypes,    out System.object SelMarks,    out System.object DrViews,    out System.object ComponentXForms ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetSelections3(  &   [Out] System.Object^ Objects, &   [Out] System.Object^ ObjectTypes, &   [Out] System.Object^ SelMarks, &   [Out] System.Object^ DrViews, &   [Out] System.Object^ ComponentXForms ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Objects*
:   Array of selected objects

*ObjectTypes*
:   Array of selected object types as defined in swSelectType\_e

*SelMarks*
:   Array of marks for the selected objects

*DrViews*
:   Array of [drawing views](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView.html)

*ComponentXForms*
:   Array of [transforms](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathTransform.html) for the selections' components

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See MacroFeatureData::GetSelections3.

# ![](dotnetimages/collapse.gif)Example

[Cut Body in Half Using Macro Feature (VBA)](Cut_Body_in_Half_using_Macro_Feature_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

When a macro feature is inserted in-context and an entity on a different component is selected, you may need to know that component's transform.

If the assembly is the active document, then you can use [IEntity::GetComponent](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEntity~GetComponent.html) or [IComponent2::Transform2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2~Transform2.html) to get the component's transform.

However, if the part for the component is open for editing and a macro feature is being edited, then you must use IMacroFeatureData::GetSelections3 to get the component's transform. This method returns the transform and the selection. If the selection belongs to the same part as the macro feature, then NULL is returned. See also Macro Features and Component Transforms.

See Accessing Selections that Define Features for additional details on using this method.

# ![](dotnetimages/collapse.gif)See Also

####

[IMacroFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData.html)

[IMacroFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData_members.html)

[IMacroFeatureData::GetSelectionCount Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~GetSelectionCount.html)

[IMacroFeatureData::IGetSelections3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~IGetSelections3.html)

[IMacroFeatureData::ISetSelections2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~ISetSelections2.html)

[IMacroFeatureData::SetSelections2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~SetSelections2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 FCS, Revision Number 14.0