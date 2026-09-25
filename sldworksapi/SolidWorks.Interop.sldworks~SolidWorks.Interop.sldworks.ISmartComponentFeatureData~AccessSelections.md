<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISmartComponentFeatureData~AccessSelections.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AccessSelections Method (ISmartComponentFeatureData) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISmartComponentFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISmartComponentFeatureData.html) : AccessSelections Method (ISmartComponentFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ShowPMP*
:   True to display the PropertyManager page, false to not (see **Remarks**)

Gains access to the selection lists on the PropertyManager page of a Smart Component.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AccessSelections( _    ByVal ShowPMP As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISmartComponentFeatureData Dim ShowPMP As System.Boolean Dim value As System.Boolean   value = instance.AccessSelections(ShowPMP) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool AccessSelections(     System.bool ShowPMP ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool AccessSelections(  &   System.bool ShowPMP ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ShowPMP*
:   True to display the PropertyManager page, false to not (see **Remarks**)

#### Return Value

True if the selections where successfully accessed, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SmartComponentFeatureData::AccessSelections.

# ![](dotnetimages/collapse.gif)Example

[Delete Smart Feature (C#)](Delete_Smart_Feature_Example_CSharp.htm)

[Delete Smart Feature (VB.NET)](Delete_Smart_Feature_Example_VBNET.htm)

[Delete Smart Feature (VBA)](Delete_Smart_Feature_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

ShowPMP only controls the display of the PropertyManager page. This method allows access to the PropertyManager page selection lists regardless of whether the PropertyManager page is displayed. The selection lists have marks as defined in swSmartComponentSelectionTypes\_e.

This method opens the training assembly in which this Smart Component is defined.

**To delete a feature or component from a Smart Component:**

1. Open the Smart Component in SOLIDWORKS.

   - Call [IFeature::GetDefinition](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~GetDefinition.html) on the "Smart Feature" to get the [ISmartComponentFeatureData](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISmartComponentFeatureData.html) object.

     - Call this method to open the training assembly of the Smart Component.

       - Call [ISldWorks::ActiveDoc](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~ActiveDoc.html) to set an assembly document variable.

         - To get a specific feature or component, call [ISelectionMgr::GetSelectedObject6](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISelectionMgr~GetSelectedObject6.html)(index, mark), where mark is defined in swSmartComponentSelectionTypes\_e and index is the position of the item in the selection list.

           - Select an already selected feature or component to delete it from its selection list. If the object returned by ISelectionMgr::GetSelectedObject6 is a:

             * feature, call [IFeature::Select2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~Select2.html) to delete that feature from the feature selection list.

               * component, call [IComponent2::Select4](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2~Select4.html) to delete that component from the component selection list.

             - Close the training assembly and release access to the selection lists.

**To insert a feature or component into a Smart Component:**

1. Open the Smart Component in SOLIDWORKS.

   - Call [IFeature::GetDefinition](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~GetDefinition.html) on the "Smart Feature" to get the [ISmartComponentFeatureData](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISmartComponentFeatureData.html) object.

     - Call this method to open the training assembly of the Smart Component.

       - Call [ISldWorks::ActiveDoc](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~ActiveDoc.html) to point to the training assembly.

         - Call [IModelDocExtension::SelectByID2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SelectByID2.html) to specify the feature or component you want to insert, setting Mark to an option in swSmartComponentSelectionTypes\_e.- Close the training assembly and release access to the selection lists.

**To close the training assembly and release access to the selection lists on the PropertyManager page:**

* Call [ISmartComponentFeatureData::ReleaseSelectionAccess](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISmartComponentFeatureData~ReleaseSelectionAccess.html) if you did not insert or delete features and components.* Call [IFeature::ModifyDefinition](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~ModifyDefinition.html) or [IFeature::IModifyDefinition2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~IModifyDefinition2.html) to rebuild the Smart Component if you inserted or deleted features and components.

# ![](dotnetimages/collapse.gif)See Also

####

[ISmartComponentFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISmartComponentFeatureData.html)

[ISmartComponentFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISmartComponentFeatureData_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2012 FCS, Revision Number 20.0