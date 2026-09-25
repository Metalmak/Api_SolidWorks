<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler5~OnSubmitSelection.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| OnSubmitSelection Method (IPropertyManagerPage2Handler5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) > [IPropertyManagerPage2Handler5 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler5.html) : OnSubmitSelection Method (IPropertyManagerPage2Handler5) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Id*
:   ID of the active selection box, where this selection is being made

*Selection*
:   Object being selected

*SelType*
:   Entity type of the selection as defined in swSelectType\_e

*ItemText*
:   Item for selection list box (see **Remarks**)

Obsoleted. Superseded by [IPropertyManagerPage2Handler6::OnSubmitSelection](SOLIDWORKS.Interop.swpublished~SOLIDWORKS.Interop.swpublished.IPropertyManagerPage2Handler6~OnSubmitSelection.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function OnSubmitSelection( _    ByVal Id As System.Integer, _    ByVal Selection As System.Object, _    ByVal SelType As System.Integer, _    ByRef ItemText As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPropertyManagerPage2Handler5 Dim Id As System.Integer Dim Selection As System.Object Dim SelType As System.Integer Dim ItemText As System.String Dim value As System.Boolean   value = instance.OnSubmitSelection(Id, Selection, SelType, ItemText) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool OnSubmitSelection(     System.int Id,    System.object Selection,    System.int SelType,    out System.string ItemText ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool OnSubmitSelection(  &   System.int Id, &   System.Object^ Selection, &   System.int SelType, &   [Out] System.String^ ItemText ) ``` | |

#### Parameters

*Id*
:   ID of the active selection box, where this selection is being made

*Selection*
:   Object being selected

*SelType*
:   Entity type of the selection as defined in swSelectType\_e

*ItemText*
:   Item for selection list box (see **Remarks**)

#### Return Value

True if the selection is accepted, false if the selection is rejected

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PropertyManagerPage2Handler5::OnSubmitSelection.

# ![](dotnetimages/collapse.gif)Remarks

If writing a VBA macro, then you must set this method to true for the user to select something. If this method is not set to true, then the user cannot select anything. This method is set to false by default.

This method is called by SOLIDWORKS when an add-in has a PropertyManager page displayed and a selection is made that passes the selection filter criteria set up for a selection list box. The add-in can then:

* Take the Dispatch pointer and the selection type.

  * QueryInterface the Dispatch pointer to get the specific interface.

    * Use APIs of that interface to determine if the selection should be allowed or not.

      + If the selection is accepted, return true, and processing will continue normally.

        - or -

        + If the selection is rejected, return false, and SOLIDWORKS will not accept the selection, just as if the selection did not pass the selection filter criteria of the selection list box.

The add-in should not Release() the Dispatch pointer. SOLIDWORKS will Release() the Dispatch pointer upon return from this method.

The method is called during the process of SOLIDWORKS selection. It is neither a pre-notification nor post-notification. The add-in should not be taking any action that might affect the model or the selection list. The add-in should only be querying information and then returning True/VARIANT\_TRUE or false/VARIANT\_FALSE.

ItemText is returned to SOLIDWORKS and stored on the selected object and can be used by your PropertyManager page selection list boxes for the life of that selection.

# ![](dotnetimages/collapse.gif)See Also

####

[IPropertyManagerPage2Handler5 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler5.html)

[IPropertyManagerPage2Handler5 Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0