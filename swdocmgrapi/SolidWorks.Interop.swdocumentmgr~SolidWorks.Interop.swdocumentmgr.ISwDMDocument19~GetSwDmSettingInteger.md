<!-- source: swdocmgrapi/SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument19~GetSwDmSettingInteger.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Document Manager API Help | Send comments on this topic. |
| GetSwDmSettingInteger Method (ISwDMDocument19) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdocumentmgr Namespace](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr_namespace.html) > [ISwDMDocument19 Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument19.html) : GetSwDmSettingInteger Method (ISwDMDocument19) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DmSetting*
:   Setting as defined by [swDmDocumentUnitsIntegerValue\_e](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.swDmDocumentUnitsIntegerValue_e.html)

Gets the specified document setting.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetSwDmSettingInteger( _    ByVal DmSetting As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwDMDocument19 Dim DmSetting As System.Integer Dim value As System.Integer   value = instance.GetSwDmSettingInteger(DmSetting) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetSwDmSettingInteger(     System.int DmSetting ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetSwDmSettingInteger(  &   System.int DmSetting ) ``` | |

#### Parameters

*DmSetting*
:   Setting as defined by [swDmDocumentUnitsIntegerValue\_e](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.swDmDocumentUnitsIntegerValue_e.html)

#### Return Value

Value for DmSetting

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwDMDocument19::GetSwDmSettingInteger.

# ![](dotnetimages/collapse.gif)Example

See the [ISwDMDocument19](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument19.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

This method works only with documents saved in SOLIDWORKS 2015 or later.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwDMDocument19 Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument19.html)

[ISwDMDocument19 Members](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument19_members.html)

[ISwDMDocument19::GetSwDmSettingToggle Method ()](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument19~GetSwDmSettingToggle.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Document Manager API 2015 SP0