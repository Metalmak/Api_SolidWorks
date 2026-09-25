<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICustomPropertyManager~IGetAll.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetAll Method (ICustomPropertyManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICustomPropertyManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICustomPropertyManager.html) : IGetAll Method (ICustomPropertyManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Count*
:   Number of custom properties

*PropNames*
:   Array of the names of custom properties

*PropTypes*
:   Array of property types as defined in swCustomInfoType\_e

*PropValues*
:   Array of values of custom properties

Gets all of the custom properties for this configuration.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub IGetAll( _    ByVal Count As System.Integer, _    ByRef PropNames As System.String, _    ByRef PropTypes As System.Integer, _    ByRef PropValues As System.String _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICustomPropertyManager Dim Count As System.Integer Dim PropNames As System.String Dim PropTypes As System.Integer Dim PropValues As System.String   instance.IGetAll(Count, PropNames, PropTypes, PropValues) ``` | |

| C# |  |
| --- | --- |
| ``` void IGetAll(     System.int Count,    out System.string PropNames,    out System.int PropTypes,    out System.string PropValues ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void IGetAll(  &   System.int Count, &   [Out] System.String^ PropNames, &   [Out] System.int PropTypes, &   [Out] System.String^ PropValues ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Count*
:   Number of custom properties

*PropNames*
:   Array of the names of custom properties

*PropTypes*
:   Array of property types as defined in swCustomInfoType\_e

*PropValues*
:   Array of values of custom properties

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CustomPropertyManager::IGetAll.

# ![](dotnetimages/collapse.gif)See Also

####

[ICustomPropertyManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICustomPropertyManager.html)

[ICustomPropertyManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICustomPropertyManager_members.html)

[ICustomPropertyManager::Get2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICustomPropertyManager~Get2.html)

[ICustomPropertyManager::GetAll Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICustomPropertyManager~GetAll.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0