<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~SaveTo3DExperience.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SaveTo3DExperience Method (IModelDocExtension) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : SaveTo3DExperience Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Options*
:   [ISaveTo3DExperienceOptions](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISaveTo3DExperienceOptions.html) (see **Remarks**)

*Errors*
:   Error codes

*Warnings*
:   Warning codes

Saves this document in SOLIDWORKS Connected using the specified save options.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SaveTo3DExperience( _    ByVal Options As System.Object, _    ByRef Errors As System.Integer, _    ByRef Warnings As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim Options As System.Object Dim Errors As System.Integer Dim Warnings As System.Integer Dim value As System.Boolean   value = instance.SaveTo3DExperience(Options, Errors, Warnings) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SaveTo3DExperience(     System.object Options,    out System.int Errors,    out System.int Warnings ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SaveTo3DExperience(  &   System.Object^ Options, &   [Out] System.int Errors, &   [Out] System.int Warnings ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Options*
:   [ISaveTo3DExperienceOptions](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISaveTo3DExperienceOptions.html) (see **Remarks**)

*Errors*
:   Error codes

*Warnings*
:   Warning codes

#### Return Value

True if the document saved successfully, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::SaveTo3DExperience.

# ![](dotnetimages/collapse.gif)Remarks

If the file is:

* new and the file name is specified in Options, then this method acts like **File > Save**. If any other options are specified, then this method acts like **File > Save With Options**.* already saved to the platform and a new file name is specified in Options, then this method acts like **File > Save As New**.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2020 SP3.1, Revision Number 28.3.1