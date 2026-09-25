<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9~OnClose.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| OnClose Method (IPropertyManagerPage2Handler9) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) > [IPropertyManagerPage2Handler9 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.html) : OnClose Method (IPropertyManagerPage2Handler9) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Reason*
:   Reason this method is called as defined in swPropertyManagerPageCloseReasons\_e

Called when this PropertyManager page is closing.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub OnClose( _    ByVal Reason As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPropertyManagerPage2Handler9 Dim Reason As System.Integer   instance.OnClose(Reason) ``` | |

| C# |  |
| --- | --- |
| ``` void OnClose(     System.int Reason ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void OnClose(  &   System.int Reason ) ``` | |

#### Parameters

*Reason*
:   Reason this method is called as defined in swPropertyManagerPageCloseReasons\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PropertyManagerPage2Handler9::OnClose.

# ![](dotnetimages/collapse.gif)Example

See the [IPropertyManagerPage2Handler9](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

This handler method is called when the PropertyManager page is about to close. This function should contain code to avoid potential problems with garbage collection.

SOLIDWORKS controls when add-ins can do work. An add-in is unable to do any real work within the PropertyManager2Handler9::OnClose handler because the PropertyManager page and command are closing. So, typically the [IPropertyPage2Handler9::AfterClose](SOLIDWORKS.Interop.swpublished~SOLIDWORKS.Interop.swpublished.IPropertyManagerPage2Handler9~AfterClose.html) handler is called after IPropertyManager2Handler9::OnClose to allow an add-in to do work. However:

|  |  |  |
| --- | --- | --- |
| **If PropertyManager page is...** | **And you implemented the handler in...** | **Then you...** |
| Not pinned | C++ | Can prevent the PropertyManager page from closing by setting the HRESULT return value to S\_FALSE. |
|  | Visual Basic | Should use the Err.Raise method with a value of 1 to prevent the PropertyManager page from closing. In VB.NET, use 0 with Err.Raise. |
|  | NOTE:  When control returns to SOLIDWORKS:   * The IPropertyManager page remains displayed on the screen. * The IPropertyManagerPage2Handler9::AfterClose handler is not called. | |
| Pinned | C++ or Visual Basic | Set HRESULT to S\_FALSE to close the PropertyManager page (i.e., ignore the fact that the page is pinned).  This allows your add-in to call the IPropertyManagerPage2Handler9::AfterClose handler and do its work. To avoid aggravating your user, who expected the PropertyManager page  to remain pinned, you should re-display and re-pin the PropertyManager page after the add-in finishes its work.  To close a pinned PropertyManager page by raising an exception, your application has to clear all selections by calling IModelDoc2::ClearSelection2(true) in the call to IPropertyManagerPage2Handler9::OnClose. The PropertyManager page will not close if selections exist. |

NOTE: In a previous version of this method, [IPropertyManagerPage2Handler3::OnClose](SOLIDWORKS.Interop.swpublished~SOLIDWORKS.Interop.swpublished.IPropertyManagerPage2Handler3~OnClose.html), if the user clicked the Cancel button and the PropertyManager page had a pushpin, then this method returned swPropertyManagerPageClose\_Closed. This version of this method returns swPropertyManagerPageClose\_Cancel in this scenario.

Managed code can indicate that a PropertyManager page cannot be closed. Throw a COM exception with an error code of 1. For example, in C#:

    void OnClose (int reason)
    {

         // Throw a COM exception as an indication the PropertyManager
         // page cannot be closed at this time:
         // The error code must be 1, which equates to S\_FALSE.
        COMException ex = new COMException("Cannot close PropertyManager page", 1);

        throw ex;

    }

SOLIDWORKS does not allow suppressing components or features while a PropertyManager page is open.

# ![](dotnetimages/collapse.gif)See Also

####

[IPropertyManagerPage2Handler9 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.html)

[IPropertyManagerPage2Handler9 Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2012 FCS, Revision Number 20.0