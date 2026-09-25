<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICustomPropertyManager~Add2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Add2 Method (ICustomPropertyManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICustomPropertyManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICustomPropertyManager.html) : Add2 Method (ICustomPropertyManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FieldName*
:   Name of custom property

*FieldType*
:   Type of custom property as defined in swCustomInfoType\_e

*FieldValue*
:   Value of custom property

Obsolete. Superseded by [ICustomPropertyManager::Add3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICustomPropertyManager~Add3.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function Add2( _    ByVal FieldName As System.String, _    ByVal FieldType As System.Integer, _    ByVal FieldValue As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICustomPropertyManager Dim FieldName As System.String Dim FieldType As System.Integer Dim FieldValue As System.String Dim value As System.Integer   value = instance.Add2(FieldName, FieldType, FieldValue) ``` | |

| C# |  |
| --- | --- |
| ``` System.int Add2(     System.string FieldName,    System.int FieldType,    System.string FieldValue ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int Add2(  &   System.String^ FieldName, &   System.int FieldType, &   System.String^ FieldValue ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FieldName*
:   Name of custom property

*FieldType*
:   Type of custom property as defined in swCustomInfoType\_e

*FieldValue*
:   Value of custom property

#### Return Value

* 1 if custom property is added* 0 if custom property is not added* -1 if the custom property already exists

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CustomPropertyManager::Add2.

# ![](dotnetimages/collapse.gif)See Also

####

[ICustomPropertyManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICustomPropertyManager.html)

[ICustomPropertyManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICustomPropertyManager_members.html)

[ICustomerPropertyManager::Delete Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICustomPropertyManager~Delete.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0