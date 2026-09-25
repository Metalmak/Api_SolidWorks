<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IAnnotation Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IAnnotation Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Allows access to notes, weld symbols, datum tags, display dimensions, blocks, cosmetic threads, center marks, centerlines, and other annotation types.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface IAnnotation ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAnnotation ``` | |

| C# |  |
| --- | --- |
| ``` public interface IAnnotation ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IAnnotation ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Annotation.

# ![](dotnetimages/collapse.gif)Example

[Get Whether Note Contains Rich-embedded Text (VBA)](Get_Whether_Note_Contains_Rich-embedded_Text_Example_VB.htm)

[Get DimXpert Display Dimensions and Feature (C#)](Get_DimXpert_Display_Dimensions_and_Feature_Example_CSharp.htm)

[Get DimXpert Display Dimensions and Feature (VB.NET)](Get_DimXpert_Display_Dimensions_and_Feature_Example_VBNET.htm)

[Get DimXpert Display Dimensions and Feature (VBA)](Get_DimXpert_Display_Dimensions_and_Feature_Example_VB.htm)

[Select Table Cells (C#)](Select_Table_Cells_Example_CSharp.htm)

[Select Table Cells (VB.NET)](Select_Table_Cells_Example_VBNET.htm)

[Select Table Cells (VBA)](Select_Table_Cells_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Because IAnnotation is a high-level representation of all annotation types, it provides functions that are generic to all types of annotations. For example, every annotation has a name and position, so IAnnotation provides functions that access this data.

Although IAnnotation has specific lower-level objects (such as [INote](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.INote.html)), it does not have any derived classes in the SOLIDWORKS API. This means that you cannot use an IAnnotation pointer to call functions in the lower-level objects. You also cannot use QueryInterface to obtain the underlying classes. Instead, SOLIDWORKS provides [IAnnotation::GetSpecificAnnotation](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAnnotation~IGetSpecificAnnotation.html), which accesses underlying objects.

Similarly if you are holding onto a lower-level class, then you can obtain the corresponding IAnnotation object using the GetAnnotation method of that class (see the **Accessors** list in this topic).

# ![](dotnetimages/collapse.gif)Accessors

[IAnnotation::GetNext3 Method](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAnnotation~GetNext3.html)

[IAnnotationView::Annotations](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotationView~Annotations.html)

[IAnnotationView::IGetAnnotations](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotationView~IGetAnnotations.html)

[ICenterLine::GetAnnotation Method](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICenterLine~GetAnnotation.html)

[ICenterMark::GetAnnotation Method](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICenterMark~GetAnnotation.html)

[ICenterOfMass::GetAnnotation](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICenterOfMass~GetAnnotation.html) and [ICenterOfMass::IGetAnnotation](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICenterOfMass~IGetAnnotation.html)

[ICThread::GetAnnotation](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICThread~GetAnnotation.html) and [ICThread::IGetAnnotation Method](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICThread~IGetAnnotation.html)

[IDatumOrigin::GetAnnotation Method](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDatumOrigin~GetAnnotation.html)

[IDatumTag::GetAnnotation](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDatumTag~GetAnnotation.html) and [IDatumTag::IGetAnnotation Method](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDatumTag~IGetAnnotation.html)

[IDatumTargetSym::GetAnnotation](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDatumTargetSym~GetAnnotation.html) and [IDatumTargetSym::IGetAnnotation Method](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDatumTargetSym~IGetAnnotation.html)

[IDisplayDimension::GetAnnotation](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDisplayDimension~GetAnnotation.html) and [IDisplayDimension::IGetAnnotation Method](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDisplayDimension~IGetAnnotation.html)

[IDowelSymbol::GetAnnotation](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDowelSymbol~GetAnnotation.html) and [IDowelSymbol::IGetAnnotation Method](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDowelSymbol~IGetAnnotation.html)

[IGtol::GetAnnotation](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IGtol~GetAnnotation.html)

[ILayer::GetItems](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILayer~GetItems.html)

[IModelDoc2::GetFirstAnnotation2 Method](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~GetFirstAnnotation2.html)

[IModelDocExtension::GetAnnotations Method](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~GetAnnotations.html)

[IModelDocExtension::InsertAnnotationFavorite Method](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~InsertAnnotationFavorite.html)

[IMultiJogLeader::GetAnnotation](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMultiJogLeader~GetAnnotation.html) and [IMultiJogLeader::IGetAnnotation Method](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMultiJogLeader~IGetAnnotation.html)

[INote::GetAnnotation](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.INote~GetAnnotation.html) and [INote::IGetAnnotation Method](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.INote~IGetAnnotation.html)

[IRevisionCloud::GetAnnotation](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IRevisionCloud~GetAnnotation.html) and [IRevisionCloud::IGetAnnotation](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IRevisionCloud~IGetAnnotation.html)

[ISFSymbol::GetAnnotation Method](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISFSymbol~GetAnnotation.html)

[ITableAnnotation::GetAnnotation Method](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ITableAnnotation~GetAnnotation.html)

[IView::GetAnnotations Method](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~GetAnnotations.html)

[IView::GetFirstAnnotation3 Method](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~GetFirstAnnotation3.html)

[IWeldBead::GetAnnotation Method](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IWeldBead~GetAnnotation.html)

[IWeldSymbol::GetAnnotation Method](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IWeldSymbol~GetAnnotation.html) and [IWeldSymbol::IGetAnnotation Method](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IWeldSymbol~IGetAnnotation.html)

# ![](dotnetimages/collapse.gif)Access Diagram

[Annotation](SWObjectModel.pdf#Annotation)

# ![](dotnetimages/collapse.gif)See Also

####

[IAnnotation Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation_members.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)

[IModelDocExtension::GetObjectId Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~GetObjectId.html)