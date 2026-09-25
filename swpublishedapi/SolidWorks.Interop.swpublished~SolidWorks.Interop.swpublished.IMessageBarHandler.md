<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IMessageBarHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| IMessageBarHandler Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IMessageBarHandler_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) : IMessageBarHandler Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Must be implemented by the add-in application to handle callbacks from IMessageBarDefinition.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface IMessageBarHandler ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMessageBarHandler ``` | |

| C# |  |
| --- | --- |
| ``` public interface IMessageBarHandler ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IMessageBarHandler ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See MessageBarHandler.

# ![](dotnetimages/collapse.gif)Example

To create a SOLIDWORKS .NET add-in that implements this interface:

1. Open a new project in Visual Studio using SOLIDWORKS template, **Visual C# - SwCSharpAddin**.

   - Add **CMessageBar\_B\_Handler.cs** with the following code to the add-in to handle message bars:

using System;

using System.Collections.Generic;

using System.Linq;

using System.Text;

using SolidWorks.Interop.sldworks;

using SolidWorks.Interop.swpublished;

using System.Diagnostics;

namespace *addin\_name*

{

    public class CMessageBar\_B\_Handler : IMessageBarHandler

    {

        // The add-in author needs to decide how the handler should react to user responses

        // In this example, pass the SOLIDWORKS application object and the target model into the handler's constructor for later use.

        // Model must be not null since message bars belong to a document

        private ISldWorks iswApp;

        private IModelDoc2 iswModelDoc;

        public CMessageBar\_B\_Handler(ISldWorks swApp, IModelDoc2 swModelDoc)

        {

            iswApp = swApp;

            iswModelDoc = swModelDoc;

        }

        public void OnUserClose()

        {

            Debug.Print("CMessageBar\_B\_Handler::OnUserClose");

            // To Do: Implement desired response.

        }

        public void OnUserResponseA(bool DoNotShowAgain)

        {

            Debug.Print(String.Format("CMessageBar\_B\_Handler::OnUserResponseA, Don't Show Again? == {0}", DoNotShowAgain));

            // To Do: Implement desired response.

        }

        public void OnUserResponseB(bool DoNotShowAgain)

        {

            Debug.Print(String.Format("CMessageBar\_B\_Handler::OnUserResponseB, Don't Show Again? == {0}", DoNotShowAgain));

            // To Do: Implement desired response.

        }

    }

}

3. Add a ShowUserMessage() function to the UI Callbacks region in **SwAddin.cs** to declare and define a user message bar and create its handler:

```
class SwAddin : ISwAddin
{
    ...

    private const String MessageBarID_B = "MyAddInName+MessageBar_B";
    private IMessageBarDefinition MessageBarDefn_B;
```

```
    void ShowUserMessage()
    {
        // Have we already defined this message bar in this session? If so, reuse it
        if ( MessageBarDefn_B == null)
        {
            // Create a new message bar definition
            MessageBarDefn_B = swApp.DefineMessageBar(MessageBarID_B) As IMessageBarDefinition;
            // Configure the Message Bar definition
            MessageBarDefn_B.Severity = (int) swMessageBarSeverity_e.swMessageBarSeverity_Warning;
            MessageBarDefn_B.Title = "Message bar for my add-in"
            MessageBarDefn_B.ResponseAType = (int) swMessageBarResponseType_e.swMessageBarResponseType_Button;
            MessageBarDefn_B.ResponseAText = "OK";
            // ResponseBType & ResponseBText have default values: swMessageBarResponseType_None & ""
            // IncludeDoNotShowAgain has default value: VARIANT_TRUE
        }

```

```
        ModelDoc2 swModelDoc = swApp.ActiveDoc;
```

```
        // Format this instance of this message bar without having to completely redefine it
        MessageBarDefn_B.Message = String.Format( "Something important happened to {0} that you should know about.", swModelDoc.GetTitle());

        // Create a handler for this instance of the message bar;
        // In this example, the handler will go out of scope here
        // SOLIDWORKS will retain its pointer to the handler object until the message bar has been dismissed and the response callback has been called.
        CMessageBar_B_Handler myHandler = new CMessageBar_B_Handler(swApp, swModelDoc);

        // Show the message bar for the document
        swShowMessageBarResult_e notifyResult = (swShowMessageBarResult_e) swModelDoc.Extension.ShowMessageBar( MessageBarDefn_B, myHandler);
        switch (notifyResult)
        {

```

```
            case swShowMessageBarResult_e.swShowMessageBarResult_Shown:
                // The *modeless* message bar has been shown
                break;
            case swShowMessageBarResult_e.swShowMessageBarResult_DontShowAgain:
                // The message bar was not shown because 'Don't show again' was previously checked
                break;
            case swShowMessageBarResult_e.swShowMessageBarResult_FailedInvalidDefinition:
                // The message bar could not be displayed due to an invalid definition (e.g. empty title/description)
                break;
            case swShowMessageBarResult_e.swShowMessageBarResult_FailedInvalidHandler:
                // The message bar was not displayed because the handler argument was null or did not support the expected interface
                break;
            default:
                // Unknown error
                break;

        }
    }
}
```

4. Modify the UI Methods region of **SwAddin.cs** to add a command item to the add-in's toolbar:

cmdIndex0 = cmdGroup.AddCommandItem2("Show User Message", -1, "Show User Message", "Show User Message", 0, "ShowUserMessage", "EnableUserMessage", mainItemID3, menuToolbarOption);

# ![](dotnetimages/collapse.gif)See Also

####

[IMessageBarHandler Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IMessageBarHandler_members.html)

[SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html)

[IUserNotificationHandler Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IUserNotificationHandler.html)