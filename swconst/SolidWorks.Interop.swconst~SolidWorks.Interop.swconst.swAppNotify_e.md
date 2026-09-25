<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swAppNotify_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swAppNotify\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swAppNotify\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Application notifications.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swAppNotify_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swAppNotify_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swAppNotify_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swAppNotify_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swAppActiveDocChangeNotify** | 4 = ActiveDocChangeNotify |
| **swAppActiveModelDocChangeNotify** | 5 = ActiveModelDocChangeNotify |
| **swAppBackgroundProcessingEndNotify** | 34 = BackgroundProcessingEndNotify |
| **swAppBackgroundProcessingStartNotify** | 33 = BackgroundProcessingStartNotify |
| **swAppBegin3DInterconnectTranslationNotify** | 37 = Begin3DInterconnectTranslationNotify |
| **swAppBeginRecordNotify** | 24 = Not used. |
| **swAppBeginTranslationNotify** | 16 = BeginTranslationNotify |
| **swAppCommandCloseNotify** | 29 = CommandCloseNotify |
| **swAppCommandOpenPreNotify** | 31 = CommandOpenPreNotify |
| **swAppDestroyNotify** | 3 = DestroyNotify |
| **swAppDocumentConversionNotify** | 9 = DocumentConversionNotify |
| **swAppDocumentLoadNotify** | 27 = Obsolete |
| **swAppDocumentLoadNotify2** | 28 = DocumentLoadNotify2 |
| **swAppEnd3DInterconnectTranslationNotify** | 38 = End3DInterconnectTranslationNotify |
| **swAppEndRecordNotify** | 25 = Not used. |
| **swAppEndTranslationNotify** | 16 = EndTranslationNotify |
| **swAppFileCloseNotify** | 32 = FileCloseNotify |
| **swAppFileNewNotify** | 2 = Obsolete |
| **swAppFileNewNotify2** | 12 = FileNewNotify2  NOTE: Because it is possible to have a NULL active document when an add-in is notified using swAppFileOpenNotify2, use ISldWorks::IGetOpenDocumentByName2 instead of ISldWorks::IActiveDoc2. |
| **swAppFileNewPreNotify** | 26 = FileNewPreNotify |
| **swAppFileOpenNotify** | 1 = Obsolete |
| **swAppFileOpenNotify2** | 13 = FileOpenNotify2 |
| **swAppFileOpenPostNotify** | 22 = FileOpenPostNotify |
| **swAppFileOpenPreNotify** | 21 = FileOpenPreNotify |
| **swAppInterfaceBrightnessThemeChangeNotify** | 35 = InterfaceBrightnessThemeChangeNotify |
| **swAppJournalWriteNotify** | 27 = Not used. |
| **swAppLightPMCreateNotify** | Not used. |
| **swAppLightSheetCreateNotify** | 18 = LightSheetCreateNotify |
| **swAppLightweightComponentOpenNotify** | 10 = Not used. |
| **swAppNonNativeFileOpenNotify** | 7 = NonNativeFileOpenNotify |
| **swAppOnIdleNotify** | 20 = OnIdleNotify |
| **swAppPromptForFilenameNotify** | 15 = PromptForFilenameNotify |
| **swAppPromptForMultipleFilenamesNotify** | 30 = PromptForMultipleFileNamesNotify |
| **swAppPropertySheetCreateNotify** | 6 = PropertySheetCreateNotify |
| **swAppReferencedFilePreNotify** | 23 = ReferencedFilePreNotify |
| **swAppReferencedFilePreNotify2** | 36 = ReferencedFilePreNotify2 |
| **swAppReferenceNotFoundNotify** | 14 = ReferenceNotFoundNotify |
| **swAppStandardsDatabaseChangeNotify** | 19 = Not used. |

# ![](dotnetimages/collapse.gif)Remarks

To receive notifications, a DLL application must register for the notifications by object type. This registration must be done for each instance of a particular object.

For example, in the file in the Visual C++ 6.0 wizard-generated add-in that supports SOLIDWORKS events ( <ATL\_object\_name>.h), include:

BEGIN\_SINK\_MAP(C<ATL\_object\_name>)

SINK\_ENTRY\_EX(ID\_SLDWORKS\_EVENTS, DIID\_DSldWorksEvents, swAppDocumentLoadNotify, DocumentLoadNotify)

SINK\_ENTRY\_EX(ID\_SLDWORKS\_EVENTS, DIID\_DSldWorksEvents, swAppFileNewNotify2, FileNewNotify2)

SINK\_ENTRY\_EX(ID\_SLDWORKS\_EVENTS, DIID\_DSldWorksEvents, swAppActiveDocChangeNotify, ActiveDocChangeNotify)

SINK\_ENTRY\_EX(ID\_SLDWORKS\_EVENTS, DIID\_DSldWorksEvents, swAppActiveModelDocChangeNotify, ActiveModelDocChangeNotify)

END\_SINK\_MAP()

If developing a C++ application, use the enumerators to register for notifications for the ISldWorks events.

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)