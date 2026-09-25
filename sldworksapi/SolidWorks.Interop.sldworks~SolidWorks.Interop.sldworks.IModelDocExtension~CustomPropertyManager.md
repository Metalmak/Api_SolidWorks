<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~CustomPropertyManager.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CustomPropertyManager Property (IModelDocExtension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : CustomPropertyManager Property (IModelDocExtension) |

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

Gets the custom properties for this document or configuration.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` ReadOnly Property CustomPropertyManager( _    ByVal ConfigName As System.String _ ) As CustomPropertyManager ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim ConfigName As System.String Dim value As CustomPropertyManager   value = instance.CustomPropertyManager(ConfigName) ``` | |

| C# |  |
| --- | --- |
| ``` CustomPropertyManager CustomPropertyManager(     System.string ConfigName ) {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property CustomPropertyManager^ CustomPropertyManager {    CustomPropertyManager^ get(System.String^ ConfigName); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ConfigName*
:   Name of configuration

#### Property Value

[ICustomPropertyManager](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICustomPropertyManager.html) object

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::CustomPropertyManager.

# ![](dotnetimages/collapse.gif)Example

[Get Custom Properties of Referenced Part (C#)](Get_Custom_Properties_of_Referenced_Part_Example_CSharp.htm)

[Get Custom Properties of Referenced Part (VB.NET)](Get_Custom_Properties_of_Referenced_Part_Example_VBNET.htm)

[Get Custom Properties of Referenced Part (VBA)](Get_Custom_Properties_of_Referenced_Part_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

File custom information is stored in the document file. It can be:

* General to the file, in which case there is a single value whatever the model's configuration

   - or -

* Configuration-specific, in which case a different value may be set for each configuration in the model

To access a general custom information value, set the configuration argument to an empty string. To get a document-level property, pass an empty string ("") to the configuration argument.

As per Microsoft recommendations for OLE support, the file summary information for SOLIDWORKS documents is written as an OLE property set into a stream named "\005Summary Information" off the root storage of the SOLIDWORKS document's compound file.

NOTE: MFC does not currently provide classes that manage summary information. However, the DRAWCLI application shipped with Visual C++ includes a sample implementation, in the form of the class CSummInfo, that you can use as an example when implementing your own. This class is used by the document class CDrawDoc. DRAWCLI also includes property pages for displaying and modifying Summary Information.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

[IConfiguration::CustomPropertyManager Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~CustomPropertyManager.html)

[IFeature::CustomPropertyManager Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~CustomPropertyManager.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0