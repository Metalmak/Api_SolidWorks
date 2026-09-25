<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICustomPropertyManager~GetAll3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetAll3 Method (ICustomPropertyManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICustomPropertyManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICustomPropertyManager.html) : GetAll3 Method (ICustomPropertyManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*PropNames*
:   Array of the names of custom properties retrieved

*PropTypes*
:   Array of types of PropNames as defined in swCustomInfoType\_e

*PropValues*
:   Array of evaluated values of PropNames

*Resolved*
:   Array of evaluation statuses of PropNames as defined in swCustomInfoGetResult\_e

*PropLink*
:   Array of integers indicating whether PropNames are linked to their parent parts:

    1 = link

    0 = no link

Gets all of the custom properties for this configuration.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetAll3( _    ByRef PropNames As System.Object, _    ByRef PropTypes As System.Object, _    ByRef PropValues As System.Object, _    ByRef Resolved As System.Object, _    ByRef PropLink As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICustomPropertyManager Dim PropNames As System.Object Dim PropTypes As System.Object Dim PropValues As System.Object Dim Resolved As System.Object Dim PropLink As System.Object Dim value As System.Integer   value = instance.GetAll3(PropNames, PropTypes, PropValues, Resolved, PropLink) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetAll3(     out System.object PropNames,    out System.object PropTypes,    out System.object PropValues,    out System.object Resolved,    out System.object PropLink ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetAll3(  &   [Out] System.Object^ PropNames, &   [Out] System.Object^ PropTypes, &   [Out] System.Object^ PropValues, &   [Out] System.Object^ Resolved, &   [Out] System.Object^ PropLink ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*PropNames*
:   Array of the names of custom properties retrieved

*PropTypes*
:   Array of types of PropNames as defined in swCustomInfoType\_e

*PropValues*
:   Array of evaluated values of PropNames

*Resolved*
:   Array of evaluation statuses of PropNames as defined in swCustomInfoGetResult\_e

*PropLink*
:   Array of integers indicating whether PropNames are linked to their parent parts:

    1 = link

    0 = no link

#### Return Value

Number of custom properties returned

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CustomPropertyManager::GetAll3.

# ![](dotnetimages/collapse.gif)Example

See the **Get Custom Properties for Configuration** examples in [ICustomPropertyManager](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICustomPropertyManager.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ICustomPropertyManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICustomPropertyManager.html)

[ICustomPropertyManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICustomPropertyManager_members.html)

[ICustomPropertyManager::Get6 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICustomPropertyManager~Get6.html)

[ICustomPropertyManager::Set2 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICustomPropertyManager~Set2.html)

[ICustomPropertyManager::GetNames Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICustomPropertyManager~GetNames.html)

[ICustomPropertyManager::GetType2 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICustomPropertyManager~GetType2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2018 FCS, Revision Number 26.0