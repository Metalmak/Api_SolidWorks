<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMateEntity2~EntityParams.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| EntityParams Property (IMateEntity2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IMateEntity2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMateEntity2.html) : EntityParams Property (IMateEntity2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the parameters for this mate entity.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` ReadOnly Property EntityParams As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMateEntity2 Dim value As System.Object   value = instance.EntityParams ``` | |

| C# |  |
| --- | --- |
| ``` System.object EntityParams {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.Object^ EntityParams {    System.Object^ get(); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

Array of doubles representing the mate entity parameters (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See MateEntity2::EntityParams.

# ![](dotnetimages/collapse.gif)Example

[Edit Mate (VBA)](Edit_Mate_Example_VB.htm)

[Get Mate Definition (VBA)](Get_Mate_Definition_Example_VB.htm)

[Get Mates and Mate Entities (C#)](Get_Mates_and_Mate_Entities_Example_CSharp.htm)

[Get Mates and Mate Entities (VB.NET)](Get_Mates_and_Mate_Entities_Example_VBNET.htm)

[Get Mates and Mate Entities (VBA)](Get_Mates_and_Mate_Entities_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

The return value is the following array of doubles:

[ pointX, pointY, pointZ, vectorI, vectorJ, vectorK, radius1, radius2 ]

 where

* pointX is the X location of this mate entity in the assembly model space

  * pointY is the Y location of this mate entity in the assembly model space

    * pointZ is the Z location of this mate entity in the assembly model space

      * vectorI is the i component of the assembly mate vector

        * vectorJ is the j component of the assembly mate vector

          * vectorK is the k component of the assembly mate vector

            * radius1 is the value for the first radius

              * radius2 is the value for the second radius

To define the mate entity, the following information is returned based on the mate type. All coordinate information is given in terms of the assembly coordinate system where the mate resides.

|  |  |
| --- | --- |
| **Mate Type** | **Returned** |
| swMatePoint | pointX, pointY, pointZ |
| swMateLine | pointX, pointY, pointZ, vectorI, vectorJ, vectorK where the point is a point on the line and the vector represents the line direction. |
| swMatePlane | pointX, pointY, pointZ, vectorI, vectorJ, vectorK where the point is a point on the plane and the vector represents the plane normal. |
| swMateCylinder | pointX, pointY, pointZ, vectorI, vectorJ, vectorK, radius1 where the point is a point on the cylinder axis and the vector represents the cylinder axis. |
| swMateCone | pointX, pointY, pointZ, vectorI, vectorJ, vectorK, radius1, radius2 where the point is a point on the cone axis and the vector represents the cone axis. |

To get the [IMateEntity2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMateEntity2.html) interface, use [IMate2::MateEntity](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMate2~MateEntity.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IMateEntity2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMateEntity2.html)

[IMateEntity2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMateEntity2_members.html)

[IMateEntity2::GetEntityParamsSize Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMateEntity2~GetEntityParamsSize.html)

[IMateEntity2::IGetEntityParams Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMateEntity2~IGetEntityParams.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12.0