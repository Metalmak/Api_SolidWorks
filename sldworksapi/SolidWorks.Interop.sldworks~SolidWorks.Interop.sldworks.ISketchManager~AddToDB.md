<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~AddToDB.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddToDB Property (ISketchManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html) : AddToDB Property (ISketchManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets whether sketch entities are added directly to the SOLIDWORKS database.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property AddToDB As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchManager Dim value As System.Boolean   instance.AddToDB = value   value = instance.AddToDB ``` | |

| C# |  |
| --- | --- |
| ``` System.bool AddToDB {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool AddToDB {    System.bool get();    void set ( &   System.bool value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

True to add items directly to the SOLIDWORKS database, false to not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SketchManager::AddToDb.

# ![](dotnetimages/collapse.gif)Example

[Get Assembly Bounding Box Using Components (C#)](Get_Assembly_Bounding_Box_Using_Components_Example_CSharp.htm)

[Get Assembly Bounding Box Using Components (VB.NET)](Get_Assembly_Bounding_Box_Using_Components_Example_VBNET.htm)

[Get Assembly Bounding Box Using Components (VBA)](Get_Assembly_Bounding_Box_using_Components_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

One of the benefits of adding sketch entities directly to the database is that you can avoid grid and entity snapping. For example, if you create a sketch line whose endpoint is near another entity or grid point, the new sketch line endpoint snaps to the other entity or grid point. Setting this property to true avoids this behavior during sketch entity creation.

After setting this property to true:

* It is not possible to undo the creation of some types of sketch entities.* You must reset it to false to restore SOLIDWORKS' normal operating mode.

This property and [ISketchManager::DisplayWhenAdded](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchManager~DisplayWhenAdded.html) improve performance during sketch entity creation. ISketchManager::DisplayWhenAdded requires that this property be set to true.

If you want to constrain all the sketch entities after creation, use [ISketch::ConstrainAll](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~ConstrainAll.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html)

[ISketchManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0