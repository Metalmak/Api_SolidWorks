<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetMassProperties2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetMassProperties2 Method (ISldWorks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : GetMassProperties2 Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FilePathName*
:   Document path and file name

*ConfigurationName*
:   Name of the configuration to use

*Accuracy*
:   * 0 = as is

      * 1 = default

        * 2 = maximum

Gets the mass properties from the specified document for the specified configuration.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetMassProperties2( _    ByVal FilePathName As System.String, _    ByVal ConfigurationName As System.String, _    ByVal Accuracy As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim FilePathName As System.String Dim ConfigurationName As System.String Dim Accuracy As System.Integer Dim value As System.Object   value = instance.GetMassProperties2(FilePathName, ConfigurationName, Accuracy) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetMassProperties2(     System.string FilePathName,    System.string ConfigurationName,    System.int Accuracy ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetMassProperties2(  &   System.String^ FilePathName, &   System.String^ ConfigurationName, &   System.int Accuracy ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FilePathName*
:   Document path and file name

*ConfigurationName*
:   Name of the configuration to use

*Accuracy*
:   * 0 = as is

      * 1 = default

        * 2 = maximum

#### Return Value

Array of doubles of size 13; last element is the accuracy at which mass properties are calculated

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::GetMassProperties2.

# ![](dotnetimages/collapse.gif)Example

[Get Mass Properties of Inactive Document (VBA)](Get_Mass_Properties_of_Inactive_Document_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

You can get the density of the current SOLIDWORKS part using [ISldWorks::GetUserPreferenceDoubleValue](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~GetUserPreferenceDoubleValue.html) and swMaterialPropertyDensity. If the density has not been explicitly set by the user, then SOLIDWORKS uses 1.0. You can also derive the density of the body from the following calculation:

Density = ( Mass / Volume )

Consistent with all other functions, this method returns metric units unless otherwise specified.

If this [IModelDoc2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2.html) object is an assembly, then any suppressed components are not included in the mass property analysis. See [IComponent2::GetSuppression](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2~GetSuppression.html) to determine the state of each of the assembly components.

This method returns an empty array if mass properties are not calculated when saving the model. This is a system-level setting and is controlled by [ISldWorks::SetUserPreferenceToggle](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~SetUserPreferenceToggle.html) and swUpdateMassPropsDuringSave.

NOTE: The calculated origin for the return values is based on the default coordinate systems of the IModelDoc2, not on the a selected coordinate system.

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[ISldWorks::IGetMassProperties2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~IGetMassProperties2.html)

[IMassProperty Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassProperty.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2003 FCS, Revision Number 11.0