<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwComFeature~Regenerate.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| Regenerate Method (ISwComFeature) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) > [ISwComFeature Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwComFeature.html) : Regenerate Method (ISwComFeature) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*app*
:   SOLIDWORKS application

*modelDoc*
:   SOLIDWORKS document in which the macro appears

*feature*
:   Macro feature that you want to rebuild

Allows you to rebuild a macro feature created using COM.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function Regenerate( _    ByVal app As System.Object, _    ByVal modelDoc As System.Object, _    ByVal feature As System.Object _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwComFeature Dim app As System.Object Dim modelDoc As System.Object Dim feature As System.Object Dim value As System.Object   value = instance.Regenerate(app, modelDoc, feature) ``` | |

| C# |  |
| --- | --- |
| ``` System.object Regenerate(     System.object app,    System.object modelDoc,    System.object feature ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ Regenerate(  &   System.Object^ app, &   System.Object^ modelDoc, &   System.Object^ feature ) ``` | |

#### Parameters

*app*
:   SOLIDWORKS application

*modelDoc*
:   SOLIDWORKS document in which the macro appears

*feature*
:   Macro feature that you want to rebuild

#### Return Value

Any one of the following values:

* True if the rebuild is successful (independent and modify)

  * False if the rebuild failed

    * String, as displayed in an error message to the user (see **Remarks**)

      * Body, if a body was created

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwComFeature::Regenerate.

# ![](dotnetimages/collapse.gif)Remarks

This method is required.

Examples of string return values:

* VBA
  swmRebuild = "Macro feature output error message"

  * C++ COM

    CComBSTR bMsg = \_T("Macro feature output error message");
    \_variant\_t vBSTRRet = bMsg;
    \*retval = vBSTRRet;

    * C#

      functionReturnValue = "Macro feature output error message";
      return functionReturnValue;

      * VB.NET

        Regenerate = "Macro feature output error message"

See Exposed COM DLL or Executable and Macro Features and Overview of Macro Features for more information.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwComFeature Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwComFeature.html)

[ISwComFeature Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwComFeature_members.html)

IMacroFeatureData Interface

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2003 FCS, Revision Number 11.0