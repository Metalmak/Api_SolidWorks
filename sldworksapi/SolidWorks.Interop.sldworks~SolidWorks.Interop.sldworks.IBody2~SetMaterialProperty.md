<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~SetMaterialProperty.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetMaterialProperty Method (IBody2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html) : SetMaterialProperty Method (IBody2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ConfigName*
:   Name of configuration

*Database*
:   "solidworks material.sldmat" or **""** or "custom materials.sldmat" (see **Remarks**)

*MaterialName*
:   Name of the SOLIDWORKS material to apply to the body (see **Remarks**)

Sets the material for this body.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetMaterialProperty( _    ByVal ConfigName As System.String, _    ByVal Database As System.String, _    ByVal MaterialName As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBody2 Dim ConfigName As System.String Dim Database As System.String Dim MaterialName As System.String Dim value As System.Integer   value = instance.SetMaterialProperty(ConfigName, Database, MaterialName) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetMaterialProperty(     System.string ConfigName,    System.string Database,    System.string MaterialName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetMaterialProperty(  &   System.String^ ConfigName, &   System.String^ Database, &   System.String^ MaterialName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ConfigName*
:   Name of configuration

*Database*
:   "solidworks material.sldmat" or **""** or "custom materials.sldmat" (see **Remarks**)

*MaterialName*
:   Name of the SOLIDWORKS material to apply to the body (see **Remarks**)

#### Return Value

Return status as defined by swBodyMaterialApplicationError\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Body2::SetMaterialProperty.

# ![](dotnetimages/collapse.gif)Example

[Set Material (C#)](Set_Material_Example_CSharp.htm)

[Set Material (VB.NET)](Set_Material_Example_VBNET.htm)

[Set Material (VBA)](Set_Material_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Click **Tools > Options > System Options > File Locations > Material Databases** to verify that a folder for Database is specified.

You can only use materials from a valid SOLIDWORKS materials database. You can specify either "solidworks materials.sldmat" or "" for the SOLIDWORKS Materials database or "custom materials.sldmat" for the Custom Materials database.

You can also find out the names of the materials in the materials database by opening the database as an XML stream and work with the XML API to get the data.

# ![](dotnetimages/collapse.gif)See Also

####

[IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html)

[IBody2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2_members.html)

[IBody2::GetMaterialIdName2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetMaterialIdName2.html)

[IBody2::GetMaterialPropertyName Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetMaterialPropertyName.html)

[IBody2::GetMaterialUserName2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetMaterialUserName2.html)

[IBody2::IGetMaterialPropertyValuesForFace Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IGetMaterialPropertyValuesForFace.html)

[IBody2::IRemoveMaterialProperty Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IRemoveMaterialProperty.html)

[IBody2::RemoveMaterialProperty Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~RemoveMaterialProperty.html)

[IBody2::SetMaterialIdName2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~SetMaterialIdName2.html)

[IBody2::SetMaterialUserName2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~SetMaterialUserName2.html)

[IBody2::IMaterialPropertyValues2 Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IMaterialPropertyValues2.html)

[IBody2::MaterialPropertyValues2 Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~MaterialPropertyValues2.html)

[IBody2::HasMaterialPropertyValues Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~HasMaterialPropertyValues.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0