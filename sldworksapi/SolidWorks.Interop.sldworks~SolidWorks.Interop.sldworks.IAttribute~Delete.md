<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAttribute~Delete.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Delete Method (IAttribute) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAttribute Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAttribute.html) : Delete Method (IAttribute) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BuildTree*
:   True to update the FeatureManager design tree, false to not

Deletes an attribute and lets you indicate whether or not to update the FeatureManager design tree if the deleted attribute appears in it.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function Delete( _    ByVal BuildTree As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAttribute Dim BuildTree As System.Boolean Dim value As System.Boolean   value = instance.Delete(BuildTree) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool Delete(     System.bool BuildTree ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool Delete(  &   System.bool BuildTree ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*BuildTree*
:   True to update the FeatureManager design tree, false to not

#### Return Value

True if the attribute is deleted, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Attribute::Delete.

# ![](dotnetimages/collapse.gif)Example

[Delete Faces (VBA)](Delete_Faces_Example_VB.htm)

[Delete Attribute (C#)](Delete_Attribute_Example_CSharp.htm)

[Delete Attribute (VB.NET)](Delete_Attribute_Example_VBNET.htm)

[Delete Attribute (VBA)](Delete_Attribute_Example_VB.htm)

[Delete Blended Faces (C#)](Delete_Blended_Faces_Example_CSharp.htm)

[Delete Blended Faces (VB.NET)](Delete_Blended_Faces_Example_VBNET.htm)

[Delete Blended Faces (VBA)](Delete_Blended_Faces_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IAttribute Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAttribute.html)

[IAttribute Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAttribute_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2003 FCS, Revision Number 11.0