<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IUserUnit.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IUserUnit Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IUserUnit_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IUserUnit Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Allows you to manage units.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface IUserUnit ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IUserUnit ``` | |

| C# |  |
| --- | --- |
| ``` public interface IUserUnit ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IUserUnit ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See UserUnit.

# ![](dotnetimages/collapse.gif)Example

[Get and Set Document Units (VBA)](Get_and_Set_User_Units_Example_VB.htm)

[Get and Set Document Units (VB.NET)](Get_and_Set_User_Units_Example_VBNET.htm)

[Get and Set Document Units (C#)](Get_and_Set_User_Units_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

| If you obtain IUserUnit using... | Then IUserUnit's properties are... |
| --- | --- |
| [IModelDoc2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) | Read only and persistent. Use IModelDocExtension::SetUserPreference\* methods to set the units properties of a document. |
| [ISldWorks](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) | Read-write, but not persistent. The instance of IUserUnit returned by ISldWorks is empty and not tied to any document. Use this instance as a template to store units properties at runtime. |

**NOTE**: Use this interface instead of **mo\_UserUnits.h** file in *public\_documents***\appcomm** of your SOLIDWORKS installation. If you previously used **mo\_UserUnits.h**, you should change your applications to use this interface.

# ![](dotnetimages/collapse.gif)Accessors

[IModelDoc2::GetUserUnit](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~GetUserUnit.html) and [IModelDoc2::IGetUserUnit](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~IGetUserUnit.html)

[ISldWorks::GetUserUnit](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetUserUnit.html) and [ISldWorks::IGetUserUnit](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~IGetUserUnit.html)

# ![](dotnetimages/collapse.gif)Access Diagram

[UserUnit](SWObjectModel.pdf#UserUnit)

# ![](dotnetimages/collapse.gif)See Also

####

[IUserUnit Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IUserUnit_members.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)