<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9~OnKeystroke.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| OnKeystroke Method (IPropertyManagerPage2Handler9) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) > [IPropertyManagerPage2Handler9 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.html) : OnKeystroke Method (IPropertyManagerPage2Handler9) |

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

    * WM\_KEYDOWN 256 or 0x100

      * WM\_KEYUP 257 or 0x101

        * WM\_CHAR 258 or 0x102

          * WM\_DEADCHAR 259 or 0x103

            * WM\_SYSKEYDOWN 260 or 0x104

              * WM\_SYSKEYUP 261 or 0x105

                * WM\_SYSCHAR 262 or 0x106

                  * WM\_SYSDEADCHAR 263 or 0x107

*Lparam*
:   lparam argument from Windows processing; bitmask containing various pieces of information; dependent on specific message

*Id*
:   ID of the control that has focus when the keystroke was made; this is the ID specified when the control was created in IPropertyManagerPage2::AddControl or IPropertyManagerPage2::IAddControl or IPropertyManagerPage2::AddGroupBox or IPropertyManagerPage2::IAddGroupBox.

Processes a keystroke that occurred on this PropertyManager page.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function OnKeystroke( _    ByVal Wparam As System.Integer, _    ByVal Message As System.Integer, _    ByVal Lparam As System.Integer, _    ByVal Id As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPropertyManagerPage2Handler9 Dim Wparam As System.Integer Dim Message As System.Integer Dim Lparam As System.Integer Dim Id As System.Integer Dim value As System.Boolean   value = instance.OnKeystroke(Wparam, Message, Lparam, Id) ``` | |

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

    * WM\_KEYDOWN 256 or 0x100

      * WM\_KEYUP 257 or 0x101

        * WM\_CHAR 258 or 0x102

          * WM\_DEADCHAR 259 or 0x103

            * WM\_SYSKEYDOWN 260 or 0x104

              * WM\_SYSKEYUP 261 or 0x105

                * WM\_SYSCHAR 262 or 0x106

                  * WM\_SYSDEADCHAR 263 or 0x107

*Lparam*
:   lparam argument from Windows processing; bitmask containing various pieces of information; dependent on specific message

*Id*
:   ID of the control that has focus when the keystroke was made; this is the ID specified when the control was created in IPropertyManagerPage2::AddControl or IPropertyManagerPage2::IAddControl or IPropertyManagerPage2::AddGroupBox or IPropertyManagerPage2::IAddGroupBox.

#### Return Value

True indicates that the keystroke has been handled by the add-in and SOLIDWORKS should not continue to try to process it, false indicates that the keystroke has not been handled by the add-in and SOLIDWORKS will continue to try to process it

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PropertyManagerPage2Handler9::OnKeystroke.

# ![](dotnetimages/collapse.gif)Example

See the [IPropertyManagerPage2Handler9](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[IPropertyManagerPage2Handler9 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.html)

[IPropertyManagerPage2Handler9 Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2012 FCS, Revision Number 20.0