<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~InsertBomTable2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertBomTable2 Method (IModelDocExtension) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : InsertBomTable2 Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*TemplateName*
:   Path and name of BOM table template (see **Remarks**)

*X*
:   X coordinate for the placement of the BOM table

*Y*
:   Y coordinate for the placement of the BOM table

*BomType*
:   Type of BOM table as defined by swBomType\_e

*ConfigurationName*
:   Name of the configuration for this BOM table (see Remarks)

*Hidden*
:   True to hide the BOM table, false to show it

Obsolete. Superseded by [IModelDocExtension::InsertBomTable3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~InsertBomTable3.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertBomTable2( _    ByVal TemplateName As System.String, _    ByVal X As System.Integer, _    ByVal Y As System.Integer, _    ByVal BomType As System.Integer, _    ByVal ConfigurationName As System.String, _    ByVal Hidden As System.Boolean _ ) As BomTableAnnotation ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim TemplateName As System.String Dim X As System.Integer Dim Y As System.Integer Dim BomType As System.Integer Dim ConfigurationName As System.String Dim Hidden As System.Boolean Dim value As BomTableAnnotation   value = instance.InsertBomTable2(TemplateName, X, Y, BomType, ConfigurationName, Hidden) ``` | |

| C# |  |
| --- | --- |
| ``` BomTableAnnotation InsertBomTable2(     System.string TemplateName,    System.int X,    System.int Y,    System.int BomType,    System.string ConfigurationName,    System.bool Hidden ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` BomTableAnnotation^ InsertBomTable2(  &   System.String^ TemplateName, &   System.int X, &   System.int Y, &   System.int BomType, &   System.String^ ConfigurationName, &   System.bool Hidden ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*TemplateName*
:   Path and name of BOM table template (see **Remarks**)

*X*
:   X coordinate for the placement of the BOM table

*Y*
:   Y coordinate for the placement of the BOM table

*BomType*
:   Type of BOM table as defined by swBomType\_e

*ConfigurationName*
:   Name of the configuration for this BOM table (see Remarks)

*Hidden*
:   True to hide the BOM table, false to show it

#### Return Value

[BOM table annotation](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBomTableAnnotation.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::InsertBomTable2.

# ![](dotnetimages/collapse.gif)Remarks

The system does not default to the Default configuration when you specify an empty string for Configuration. You must specify the configuration.

BOM table templates are in the <*SOLIDWORKS\_*install\_dir>\lang\<language> folder and have a filename extension of .sldbomtbt. The template and table must be of the same type. For example, you could specify C:\Program Files\SOLIDWORKS\lang\English\bom-standard.sldbomtbt for TemplateName if you wanted to insert an English-version of the standard BOM table template.

If the BOM table is a parts-only or indented-style BOM and ConfigurationName is invalid, then the BOM is not created.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

[IView::InsertBomTable3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~InsertBomTable3.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0