<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc~InsertPart3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertPart3 Method (IPartDoc) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPartDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc.html) : InsertPart3 Method (IPartDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FileName*
:   Name of the part file to insert

*Options*
:   Insertion options as defined in swInsertPartOptions\_e

*ConfigurationName*
:   Name of FileName's configuration

Inserts the specified part in the specified configuration into this part.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertPart3( _    ByVal FileName As System.String, _    ByVal Options As System.Integer, _    ByVal ConfigurationName As System.String _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPartDoc Dim FileName As System.String Dim Options As System.Integer Dim ConfigurationName As System.String Dim value As Feature   value = instance.InsertPart3(FileName, Options, ConfigurationName) ``` | |

| C# |  |
| --- | --- |
| ``` Feature InsertPart3(     System.string FileName,    System.int Options,    System.string ConfigurationName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ InsertPart3(  &   System.String^ FileName, &   System.int Options, &   System.String^ ConfigurationName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FileName*
:   Name of the part file to insert

*Options*
:   Insertion options as defined in swInsertPartOptions\_e

*ConfigurationName*
:   Name of FileName's configuration

#### Return Value

Inserted [feature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PartDoc::InsertPart3.

# ![](dotnetimages/collapse.gif)Example

[Modify Derived Part (VBA)](Modify_Derived_Part_Example_VB.htm)

[Modify Derived Part (VB.NET)](Modify_Derived_Part_Example_VBNET.htm)

[Modify Derived Part (C#)](Modify_Derived_Part_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method inserts the specified part at the origin of this part. To position the inserted part at a different location or orientation or both, use [IFeatureManager::InsertMoveCopyBody2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~InsertMoveCopyBody2.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IPartDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc.html)

[IPartDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc_members.html)

[IDerivedPartFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDerivedPartFeatureData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2019 FCS, Revision Number 27.0