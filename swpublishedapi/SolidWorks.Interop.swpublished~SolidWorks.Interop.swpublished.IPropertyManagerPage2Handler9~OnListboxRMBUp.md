<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9~OnListboxRMBUp.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| OnListboxRMBUp Method (IPropertyManagerPage2Handler9) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) > [IPropertyManagerPage2Handler9 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.html) : OnListboxRMBUp Method (IPropertyManagerPage2Handler9) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Id*
:   ID of the list box

*PosX*
:   X coordinate of the right-mouse button menu

*PosY*
:   Y coordinate of the right-mouse button menu

Called when the right-mouse button is released in a list box on this PropertyManager page.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub OnListboxRMBUp( _    ByVal Id As System.Integer, _    ByVal PosX As System.Integer, _    ByVal PosY As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPropertyManagerPage2Handler9 Dim Id As System.Integer Dim PosX As System.Integer Dim PosY As System.Integer   instance.OnListboxRMBUp(Id, PosX, PosY) ``` | |

| C# |  |
| --- | --- |
| ``` void OnListboxRMBUp(     System.int Id,    System.int PosX,    System.int PosY ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void OnListboxRMBUp(  &   System.int Id, &   System.int PosX, &   System.int PosY ) ``` | |

#### Parameters

*Id*
:   ID of the list box

*PosX*
:   X coordinate of the right-mouse button menu

*PosY*
:   Y coordinate of the right-mouse button menu

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PropertyManagerPage2Handler9::OnListboxRMBUp.

# ![](dotnetimages/collapse.gif)Example

See the [IPropertyManagerPage2Handler9](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[IPropertyManagerPage2Handler9 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.html)

[IPropertyManagerPage2Handler9 Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2012 FCS, Revision Number 20.0