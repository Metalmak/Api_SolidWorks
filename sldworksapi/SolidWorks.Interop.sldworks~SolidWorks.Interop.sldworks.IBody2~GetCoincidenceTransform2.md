<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetCoincidenceTransform2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetCoincidenceTransform2 Method (IBody2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html) : GetCoincidenceTransform2 Method (IBody2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BodyDispIn*
:   [Input body](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html)

*Xform*
:   Pointer to the [transformation matrix](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathTransform.html)

Calculates the transformation matrix, which would make the input body coincident with this body if the transformation matrix is applied.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetCoincidenceTransform2( _    ByVal BodyDispIn As System.Object, _    ByRef Xform As MathTransform _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBody2 Dim BodyDispIn As System.Object Dim Xform As MathTransform Dim value As System.Boolean   value = instance.GetCoincidenceTransform2(BodyDispIn, Xform) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetCoincidenceTransform2(     System.object BodyDispIn,    out MathTransform Xform ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetCoincidenceTransform2(  &   System.Object^ BodyDispIn, &   [Out] MathTransform^ Xform ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*BodyDispIn*
:   [Input body](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html)

*Xform*
:   Pointer to the [transformation matrix](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathTransform.html)

#### Return Value

True if this body and the input body can coincide by applying the transformation matrix, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Body2::GetCoincidenceTransform2.

# ![](dotnetimages/collapse.gif)Example

[Calculate Transformations in Part (C#)](Calculate_Transformations_in_Part_Example_CSharp.htm)

[Calculate Transformations in Part (VB.NET)](Calculate_Transformations_in_Part_Example_VBNET.htm)

[Calculate Transformations in Part (VBA)](Calculate_Transformations_in_Part_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html)

[IBody2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2013 SP1, Revision Number 21.1