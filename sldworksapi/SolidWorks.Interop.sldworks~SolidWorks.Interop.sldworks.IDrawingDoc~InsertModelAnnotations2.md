<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~InsertModelAnnotations2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertModelAnnotations2 Method (IDrawingDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html) : InsertModelAnnotations2 Method (IDrawingDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Option*

*AllTypes*

*Types*

*AllViews*

*DuplicateDims*

*HiddenFeatureDims*

Obsolete. Superseded by [IDrawingDoc::InsertModelAnnotations3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDrawingDoc~InsertModelAnnotations3.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertModelAnnotations2( _    ByVal Option As System.Integer, _    ByVal AllTypes As System.Boolean, _    ByVal Types As System.Integer, _    ByVal AllViews As System.Boolean, _    ByVal DuplicateDims As System.Boolean, _    ByVal HiddenFeatureDims As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDrawingDoc Dim Option As System.Integer Dim AllTypes As System.Boolean Dim Types As System.Integer Dim AllViews As System.Boolean Dim DuplicateDims As System.Boolean Dim HiddenFeatureDims As System.Boolean Dim value As System.Boolean   value = instance.InsertModelAnnotations2(Option, AllTypes, Types, AllViews, DuplicateDims, HiddenFeatureDims) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool InsertModelAnnotations2(     System.int Option,    System.bool AllTypes,    System.int Types,    System.bool AllViews,    System.bool DuplicateDims,    System.bool HiddenFeatureDims ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool InsertModelAnnotations2(  &   System.int Option, &   System.bool AllTypes, &   System.int Types, &   System.bool AllViews, &   System.bool DuplicateDims, &   System.bool HiddenFeatureDims ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Option*

*AllTypes*

*Types*

*AllViews*

*DuplicateDims*

*HiddenFeatureDims*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DrawingDoc::InsertModelAnnotations2.

# ![](dotnetimages/collapse.gif)See Also

####

[IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html)

[IDrawingDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc_members.html)