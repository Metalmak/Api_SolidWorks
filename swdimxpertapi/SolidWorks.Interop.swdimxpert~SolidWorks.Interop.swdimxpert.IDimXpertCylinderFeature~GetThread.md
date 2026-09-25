<!-- source: swdimxpertapi/SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertCylinderFeature~GetThread.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS DimXpert API Help | Send comments on this topic. |
| GetThread Method (IDimXpertCylinderFeature) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdimxpert Namespace](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert_namespace.html) > [IDimXpertCylinderFeature Interface](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertCylinderFeature.html) : GetThread Method (IDimXpertCylinderFeature) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*IsThreaded*
:   True if the cylinder is threaded; false otherwise

*ThreadDesignation*
:   Description of the thread

*ThreadDepth*
:   Depth of the thread for a threaded hole

Gets thread information for this DimXpert cylinder.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetThread( _    ByRef IsThreaded As System.Boolean, _    ByRef ThreadDesignation As System.String, _    ByRef ThreadDepth As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDimXpertCylinderFeature Dim IsThreaded As System.Boolean Dim ThreadDesignation As System.String Dim ThreadDepth As System.Double Dim value As System.Boolean   value = instance.GetThread(IsThreaded, ThreadDesignation, ThreadDepth) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetThread(     out System.bool IsThreaded,    out System.string ThreadDesignation,    out System.double ThreadDepth ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetThread(  &   [Out] System.bool IsThreaded, &   [Out] System.String^ ThreadDesignation, &   [Out] System.double ThreadDepth ) ``` | |

#### Parameters

*IsThreaded*
:   True if the cylinder is threaded; false otherwise

*ThreadDesignation*
:   Description of the thread

*ThreadDepth*
:   Depth of the thread for a threaded hole

#### Return Value

True if method call is successful; false otherwise

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DimXpertCylinderFeature::GetThread.

# ![](dotnetimages/collapse.gif)Example

[Get DimXpert Feature Example (VBA)](Get_DimXpert_Feature_Example_VB.htm)

[Get DimXpert Feature Example (VB.NET)](Get_DimXpert_Feature_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IDimXpertCylinderFeature Interface](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertCylinderFeature.html)

[IDimXpertCylinderFeature Members](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertCylinderFeature_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0