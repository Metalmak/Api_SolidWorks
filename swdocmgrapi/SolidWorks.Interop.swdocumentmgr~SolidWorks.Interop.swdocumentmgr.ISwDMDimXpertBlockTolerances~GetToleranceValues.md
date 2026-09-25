<!-- source: swdocmgrapi/SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDimXpertBlockTolerances~GetToleranceValues.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Document Manager API Help | Send comments on this topic. |
| GetToleranceValues Method (ISwDMDimXpertBlockTolerances) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdocumentmgr Namespace](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr_namespace.html) > [ISwDMDimXpertBlockTolerances Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDimXpertBlockTolerances.html) : GetToleranceValues Method (ISwDMDimXpertBlockTolerances) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Linear1*
:   Tolerance for x dimension

*Linear1Prec*
:   Number of decimal places for Linear1 tolerance

*Linear2*
:   Tolerance for y dimension

*Linear2Prec*
:   Number of decimal places for Linear2 tolerance

*Linear3*
:   Tolerance for z dimension

*Linear3Prec*
:   Number of decimal places for Linear3 tolerance

*Angular*
:   Tolerance for angular dimension

Gets block tolerance settings for a given document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetToleranceValues( _    ByRef Linear1 As System.Double, _    ByRef Linear1Prec As System.Integer, _    ByRef Linear2 As System.Double, _    ByRef Linear2Prec As System.Integer, _    ByRef Linear3 As System.Double, _    ByRef Linear3Prec As System.Integer, _    ByRef Angular As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwDMDimXpertBlockTolerances Dim Linear1 As System.Double Dim Linear1Prec As System.Integer Dim Linear2 As System.Double Dim Linear2Prec As System.Integer Dim Linear3 As System.Double Dim Linear3Prec As System.Integer Dim Angular As System.Double Dim value As System.Boolean   value = instance.GetToleranceValues(Linear1, Linear1Prec, Linear2, Linear2Prec, Linear3, Linear3Prec, Angular) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetToleranceValues(     out System.double Linear1,    out System.int Linear1Prec,    out System.double Linear2,    out System.int Linear2Prec,    out System.double Linear3,    out System.int Linear3Prec,    out System.double Angular ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetToleranceValues(  &   [Out] System.double Linear1, &   [Out] System.int Linear1Prec, &   [Out] System.double Linear2, &   [Out] System.int Linear2Prec, &   [Out] System.double Linear3, &   [Out] System.int Linear3Prec, &   [Out] System.double Angular ) ``` | |

#### Parameters

*Linear1*
:   Tolerance for x dimension

*Linear1Prec*
:   Number of decimal places for Linear1 tolerance

*Linear2*
:   Tolerance for y dimension

*Linear2Prec*
:   Number of decimal places for Linear2 tolerance

*Linear3*
:   Tolerance for z dimension

*Linear3Prec*
:   Number of decimal places for Linear3 tolerance

*Angular*
:   Tolerance for angular dimension

#### Return Value

True if method call is successful; false otherwise

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwDMDimXpertBlockTolerances::GetToleranceValues.

# ![](dotnetimages/collapse.gif)Example

See the examples on the interface page.

# ![](dotnetimages/collapse.gif)Remarks

This interface accesses the DimXpert block tolerance settings that are specified in the SOLIDWORKS System Options and Document Properties dialog (Tools > Options > Document Properties > DimXpert).

# ![](dotnetimages/collapse.gif)See Also

####

[ISwDMDimXpertBlockTolerances Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDimXpertBlockTolerances.html)

[ISwDMDimXpertBlockTolerances Members](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDimXpertBlockTolerances_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0