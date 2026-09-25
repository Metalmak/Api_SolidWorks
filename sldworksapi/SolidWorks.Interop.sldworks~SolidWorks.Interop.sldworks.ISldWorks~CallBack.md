<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~CallBack.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CallBack Method (ISldWorks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : CallBack Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*CallBackFunc*
:   Function to call

*DefaultRetVal*
:   Default return value

*CallBackArgs*
:   Arguments to pass to the callback function

Allows an out-of-process executable or a SOLIDWORKS macro to call back a function in a SOLIDWORKS add-in DLL.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CallBack( _    ByVal CallBackFunc As System.String, _    ByVal DefaultRetVal As System.Integer, _    ByVal CallBackArgs As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim CallBackFunc As System.String Dim DefaultRetVal As System.Integer Dim CallBackArgs As System.String Dim value As System.Integer   value = instance.CallBack(CallBackFunc, DefaultRetVal, CallBackArgs) ``` | |

| C# |  |
| --- | --- |
| ``` System.int CallBack(     System.string CallBackFunc,    System.int DefaultRetVal,    System.string CallBackArgs ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int CallBack(  &   System.String^ CallBackFunc, &   System.int DefaultRetVal, &   System.String^ CallBackArgs ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*CallBackFunc*
:   Function to call

*DefaultRetVal*
:   Default return value

*CallBackArgs*
:   Arguments to pass to the callback function

#### Return Value

Return value from the callback function, if it is called; DefaultRetVal if it is not called

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::CallBack.

# ![](dotnetimages/collapse.gif)Example

To set the filename:

result = swApp.CallBack("pworks@miEval", 0, "RenderToFile Filename d:\image\xyz.jpg")

# ![](dotnetimages/collapse.gif)Remarks

The CallBackFunc value contains the callback function to call. The syntax is:

dllname@function

where:

* dllname is the name of the add-in library as specified in your project .def file.

  * function is the name of the function that gets called by this method. It must be declared as an exportin your project .def file.

If the callback function is actually called, then the return value contains the value returned by the callback function, and the DefaultRetVal is not used.

If the callback function is not called, then the DefaultRetVal value is passed back from the API in the retval value. This allows the caller of this API to specify a return value that is different from any return value that the callback function might return so that it can tell if a problem occurred that caused the callback to never get called.

The CallBackArgs value contains the information to pass to the callback function. This value is untouched by the API and is passed through to the callback as a BSTR. Therefore, the format of what is inside of the string can be whatever the caller wants it to be. Handling and use of it is the sole responsibility of the callback function.

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[ISldWorks::AddCallback Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~AddCallback.html)

[ISldWorks::RemoveCallback Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~RemoveCallback.html)

[ISldWorks::SetAddinCallbackInfo Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~SetAddinCallbackInfo.html)