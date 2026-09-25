<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITexture~GetSystemTextureName.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetSystemTextureName Method (ITexture) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ITexture Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITexture.html) : GetSystemTextureName Method (ITexture) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FileNameIn*
:   Path and filename of texture (see **Remarks**)

*Res*
:   True if the name of the texture that appears in the Texture PropertyManager is returned, false if not

Gets the name of the texture that appears in the Texture PropertyManager.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetSystemTextureName( _    ByVal FileNameIn As System.String, _    ByRef Res As System.Boolean _ ) As System.String ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ITexture Dim FileNameIn As System.String Dim Res As System.Boolean Dim value As System.String   value = instance.GetSystemTextureName(FileNameIn, Res) ``` | |

| C# |  |
| --- | --- |
| ``` System.string GetSystemTextureName(     System.string FileNameIn,    out System.bool Res ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.String^ GetSystemTextureName(  &   System.String^ FileNameIn, &   [Out] System.bool Res ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FileNameIn*
:   Path and filename of texture (see **Remarks**)

*Res*
:   True if the name of the texture that appears in the Texture PropertyManager is returned, false if not

#### Return Value

Name of texture as it appears in the Texture PropertyManager (see Remarks)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Texture::GetSystemTextureName.

# ![](dotnetimages/collapse.gif)Example

See the [ITexture](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITexture.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

This method only supports SOLIDWORKS-supplied textures.

Call [ITexture::MaterialName](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ITexture~MaterialName.html) to get the value for FileNameIn before calling this method. ITexture::MaterialName returns an abbreviated path and the name of the texture as it appears in the Texture PropertyManager. For example, if ITexture::MaterialName returns *install\_dir***\data\images\textures\plastic\brushed\bred.jpg**, then this method returns Plastic\Brushed\Red.

# ![](dotnetimages/collapse.gif)See Also

####

[ITexture Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITexture.html)

[ITexture Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITexture_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2005 FCS, Revision Number 13.0