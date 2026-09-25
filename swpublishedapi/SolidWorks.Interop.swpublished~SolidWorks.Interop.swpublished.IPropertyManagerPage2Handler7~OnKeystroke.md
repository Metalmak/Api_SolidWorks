<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler7~OnKeystroke.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| OnKeystroke Method (IPropertyManagerPage2Handler7) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) > [IPropertyManagerPage2Handler7 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler7.html) : OnKeystroke Method (IPropertyManagerPage2Handler7) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Wparam*
:   wparam argument from Windows processing; indicates the keystroke that occurred

    NOTE: From the standard set of virtual keys from Windows. Refer to the Virtual Key Code information from Microsoft documentation; for example, the Alt key is VK\_MENU.

*Message*
:   Message being processed by Windows; one of these values:

    * WM\_KEYDOWN 0x0100

      * WM\_KEYUP 0x0101

        * WM\_CHAR 0x0102

          * WM\_DEADCHAR 0x0103

            * WM\_SYSKEYDOWN 0x0104

              * WM\_SYSKEYUP 0x0105

                * WM\_SYSCHAR 0x0106

                  * WM\_SYSDEADCHAR 0x0107

*Lparam*
:   lparam argument from Windows processing; bitmask containing various pieces of information; dependent on specific message

*Id*
:   ID of the control that has focus when the keystroke was made; this is the ID specified when the control was created in IPropertyManagerPage2::AddControl or IPropertyManagerPage2::IAddControl or IPropertyManagerPage2::AddGroupBox or IPropertyManagerPage2::IAddGroupBox.

Obsoleted. Superseded by [IPropertyManagerPage2Handler8::OnKeystroke](SOLIDWORKS.Interop.swpublished~SOLIDWORKS.Interop.swpublished.IPropertyManagerPage2Handler8~OnKeystroke.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function OnKeystroke( _    ByVal Wparam As System.Integer, _    ByVal Message As System.Integer, _    ByVal Lparam As System.Integer, _    ByVal Id As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPropertyManagerPage2Handler7 Dim Wparam As System.Integer Dim Message As System.Integer Dim Lparam As System.Integer Dim Id As System.Integer Dim value As System.Boolean   value = instance.OnKeystroke(Wparam, Message, Lparam, Id) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool OnKeystroke(     System.int Wparam,    System.int Message,    System.int Lparam,    System.int Id ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool OnKeystroke(  &   System.int Wparam, &   System.int Message, &   System.int Lparam, &   System.int Id ) ``` | |

#### Parameters

*Wparam*
:   wparam argument from Windows processing; indicates the keystroke that occurred

    NOTE: From the standard set of virtual keys from Windows. Refer to the Virtual Key Code information from Microsoft documentation; for example, the Alt key is VK\_MENU.

*Message*
:   Message being processed by Windows; one of these values:

    * WM\_KEYDOWN 0x0100

      * WM\_KEYUP 0x0101

        * WM\_CHAR 0x0102

          * WM\_DEADCHAR 0x0103

            * WM\_SYSKEYDOWN 0x0104

              * WM\_SYSKEYUP 0x0105

                * WM\_SYSCHAR 0x0106

                  * WM\_SYSDEADCHAR 0x0107

*Lparam*
:   lparam argument from Windows processing; bitmask containing various pieces of information; dependent on specific message

*Id*
:   ID of the control that has focus when the keystroke was made; this is the ID specified when the control was created in IPropertyManagerPage2::AddControl or IPropertyManagerPage2::IAddControl or IPropertyManagerPage2::AddGroupBox or IPropertyManagerPage2::IAddGroupBox.

#### Return Value

True indicates that the keystroke has been handled by the add-in and SOLIDWORKS should not continue to try to process it, false indicates that the keystroke has not been handled by the add-in and SOLIDWORKS will continue to try to process it

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PropertyManagerPage2Handler7::OnKeystroke.

# ![](dotnetimages/collapse.gif)Remarks

After the add-in has finished processing the keystroke, the message continues on and is processed by Windows. Because processing must occur, nothing should be done to destroy the page nor any action performed that could disrupt normal Windows processing while the add-in is handling this keystroke.

To enable this functionality for this PropertyManager page, set the Options argument of ISldWorks::CreatePropertyManagerPage or ISldWorks::ICreatePropertyManagerPage to swPropertyManagerOptions\_HandleKeystrokes. By default, this style is not enabled because most applications are not interested in processing keystrokes, and it is a potential performance bottleneck if lots of keystrokes are occurring.

# ![](dotnetimages/collapse.gif)See Also

####

[IPropertyManagerPage2Handler7 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler7.html)

[IPropertyManagerPage2Handler7 Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler7_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0