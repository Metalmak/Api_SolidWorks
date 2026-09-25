<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swDrawingNotify_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swDrawingNotify\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swDrawingNotify\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Drawing notifications.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swDrawingNotify_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swDrawingNotify_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swDrawingNotify_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swDrawingNotify_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swDrawingActivateSheetPostNotify** | 53 = ActivateSheetPostNotify |
| **swDrawingActivateSheetPreNotify** | 52 = ActivateSheetPreNotify |
| **swDrawingAddCustomPropertyNotify** | 20 = AddCustomPropertyNotify |
| **swDrawingAddDvePagePreNotify** | 40 = Not used. |
| **swDrawingAddItemNotify** | 15 = AddItemNotify |
| **swDrawingAutoSaveNotify** | 10 = AutoSaveNotify |
| **swDrawingAutoSaveToStorageNotify** | 11 = AutoSaveToStorageNotify |
| **swDrawingAutoSaveToStorageStoreNotify** | 48 = AutoSaveToStorageStoreNotify |
| **swDrawingChangeCustomPropertyNotify** | 21 = ChangeCustomPropertyNotify |
| **swDrawingClearSelectionsNotify** | 37 = ClearSelectionsNotify |
| **swDrawingCommandManagerTabActivatedPreNotify** | 54 = CommandManagerTabActivatedPreNotify |
| **swDrawingConfigChangeNotify** | 12 = ActiveConfigChangeNotify |
| **swDrawingConfigChangePostNotify** | 13 = ActiveConfigChangePostNotify |
| **swDrawingDeleteCustomPropertyNotify** | 22 = DeleteCustomPropertyNotify |
| **swDrawingDeleteItemNotify** | 17 = DeleteItemNotify |
| **swDrawingDeleteItemPreNotify** | 36 = DeleteItemPreNotify |
| **swDrawingDeleteSelectionPreNotify** | 24 = DeleteSelectonPreNotify |
| **swDrawingDestroyNotify** | 2 = Obsolete |
| **swDrawingDestroyNotify2** | 42 = DestroyNotify2 |
| **swDrawingDimensionChangeNotify** | 32 = DimensionChangeNotify |
| **swDrawingDynamicHighlightNotify** | 31 = DynamicHighlightNotify |
| **swDrawingEquationEditorPostNotify** | 39 = EquationEditorPostNotify |
| **swDrawingEquationEditorPreNotify** | 38 = EquationEditorPreNotify |
| **swDrawingFeatureManagerTabActivatedNotify** | 56 = FeatureManagerTabActivatedNotify |
| **swDrawingFeatureManagerTabActivatedPreNotify** | 55 = FeatureManagerTabActivatedPreNotify |
| **swDrawingFeatureManagerTreeRebuildNotify** | 29 = FeatureManagerTreeRebuildNotify |
| **swDrawingFileReloadCancelNotify** | 33 = Not used. |
| **swDrawingFileReloadNotify** | 19 = Not used. |
| **swDrawingFileReloadPreNotify** | 25 = Not used. |
| **swDrawingFileSaveAsNotify** | 7 = Obsolete |
| **swDrawingFileSaveAsNotify2** | 23 = FileSaveAsNotify2 |
| **swDrawingFileSaveNotify** | 6 = FileSaveNotify |
| **swDrawingFileSavePostCancelNotify** | 34 = FileSavePostCancelNotify |
| **swDrawingFileSavePostNotify** | 26 = FileSavePostNotify |
| **swDrawingInsertTableNotify** | 49 = InsertTableNotify |
| **swDrawingLoadFromStorageNotify** | 8 = LoadFromStorageNotify |
| **swDrawingLoadFromStorageStoreNotify** | 27 = LoadFromStorageStoreNotify |
| **swDrawingModifyNotify** | 18 = ModifyNotify |
| **swDrawingModifyTableNotify** | 50 = ModifyTableNotify |
| **swDrawingNewSelectionNotify** | 5 = NewSelectionNotify |
| **swDrawingRedoPostNotify** | 45 = RedoPostNotify |
| **swDrawingRedoPreNotify** | 46 = RedoPreNotify |
| **swDrawingRegenNotify** | 1 = RegenNotify |
| **swDrawingRegenPostNotify** | 3 = RegenPostNotify |
| **swDrawingRenameDisplayTitleNotify** | 57 = RenameDisplayTitleNotify |
| **swDrawingRenameItemNotify** | 16 = RenameItemNotify |
| **swDrawingSaveToStorageNotify** | 9 = SaveToStorageNotify |
| **swDrawingSaveToStorageStoreNotify** | 28 = SaveToStorageStoreNotify |
| **swDrawingSketchSolveNotify** | 35 = SketchSolveNotify |
| **swDrawingUndoPostNotify** | 43 = UndoPostNotify |
| **swDrawingUndoPreNotify** | 47 = UndoPreNotify |
| **swDrawingUnitsChangeNotify** | 41 = UnitsChangeNotify |
| **swDrawingUserSelectionPostNotify** | 51 = UserSelectionPostNotify |
| **swDrawingUserSelectionPreNotify** | 44 = UserSelectionPreNotify |
| **swDrawingViewCreatePreNotify** | 30 = ViewCreatePreNotify |
| **swDrawingViewNewNotify** | 4 = Obsolete |
| **swDrawingViewNewNotify2** | 14 = ViewNewNotify2 |

# ![](dotnetimages/collapse.gif)Remarks

To receive notifications, a DLL application must register for the notifications by object type. This registration must be done for each instance of a particular object.

For example, in the file in the Visual C++ 6.0 wizard-generated add-in that supports drawing events (e.g., Drawing.h), include:

BEGIN\_SINK\_MAP(CSwDrawing)

SINK\_ENTRY\_EX(ID\_DRAWINGDOC\_EVENTS, DIID\_DDrawingDocEvents, swDrawingDestroyNotify, DestroyNotify)

SINK\_ENTRY\_EX(ID\_DRAWINGDOC\_EVENTS, DIID\_DDrawingDocEvents, swDrawingNewSelectionNotify, NewSelectionNotify)

END\_SINK\_MAP()

If developing a C++ application, use the enumerators to register for notifications for IDrawingDoc events.

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)