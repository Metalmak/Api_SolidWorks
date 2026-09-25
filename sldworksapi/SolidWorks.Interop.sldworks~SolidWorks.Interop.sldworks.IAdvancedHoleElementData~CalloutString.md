<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedHoleElementData~CalloutString.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CalloutString Property (IAdvancedHoleElementData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAdvancedHoleElementData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedHoleElementData.html) : CalloutString Property (IAdvancedHoleElementData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the hole callout string for this Advanced Hole element.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property CalloutString As System.String ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAdvancedHoleElementData Dim value As System.String   instance.CalloutString = value   value = instance.CalloutString ``` | |

| C# |  |
| --- | --- |
| ``` System.string CalloutString {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.String^ CalloutString {    System.String^ get();    void set ( &   System.String^ value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

Hole callout string (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AdvancedHoleElementData::CalloutString.

# ![](dotnetimages/collapse.gif)Example

See the [IAdvancedHoleElementData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedHoleElementData.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

This property is valid only if [IAdvancedHoleFeatureData::CustomizeCallout](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedHoleFeatureData~CustomizeCallout.html) is set to true.

The hole callout string is formatted as follows:

<*LibraryName*-*SymbolName*> <*callout\_var1*> <*callout\_var2*>... <*callout\_varn*>

where:

* *LibraryName* and *SymbolName* are defined in ***c:\ProgramData\SolidWorks\SolidWorks 20**nn**\lang\english\gtol.sym**.** *callout\_var1-n* are callout variables. Use [IModelDocExtension::GetCalloutVariableString](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~GetCalloutVariableString.html) to get the strings for hole callout variables defined in swCalloutVariable\_e. You can also find the hole callout variable strings by clicking **Hole Callout > Callout Variables** in the Advanced Hole PropertyManager.

**Note**: You must include the right- and left-angle brackets and the hyphens when setting the elements of this property string:

```
   "<HOLE-SPOT><MOD-DIAM> <ah-cboredia> <HOLE-DEPTH> <ah-cboredepth><ah-cboreside>"
```

# ![](dotnetimages/collapse.gif)See Also

####

[IAdvancedHoleElementData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedHoleElementData.html)

[IAdvancedHoleElementData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedHoleElementData_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2018 FCS, Revision Number 26.0