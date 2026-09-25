<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertMacroFeature3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertMacroFeature3 Method (IFeatureManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertMacroFeature3 Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BaseName*
:   Name of the base feature (see **Remarks**)

*ProgId*
:   COM or .NET callback object; empty string if VBA (see Remarks)

*MacroMethods*
:   Array of strings of size 9 only for VBA; "" otherwise (see Remarks)

*ParamNames*
:   Array of strings of the names of the parameters

*ParamTypes*
:   Array of the types of parameters of size paramCount as defined by swMacroFeatureParamType\_e

*ParamValues*
:   Array of strings of the values of parameters

*DimTypes*
:   Array of the types of dimensions as defined by swDimensionType\_e (see **Remarks**)

*DimValues*
:   Array of values of the dimensions

*EditBodies*
:   Array of [IBody2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html) objects to modify in the macro feature

*IconFiles*
:   Array of strings of the files names for the icons (see **Remarks**)

*Options*
:   Placement of the macro feature in the FeatureManager design tree as defined by swMacroFeatureOptions\_e (see **Remarks**)

Inserts a macro feature in this model.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertMacroFeature3( _    ByVal BaseName As System.String, _    ByVal ProgId As System.String, _    ByVal MacroMethods As System.Object, _    ByVal ParamNames As System.Object, _    ByVal ParamTypes As System.Object, _    ByVal ParamValues As System.Object, _    ByVal DimTypes As System.Object, _    ByVal DimValues As System.Object, _    ByVal EditBodies As System.Object, _    ByVal IconFiles As System.Object, _    ByVal Options As System.Integer _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim BaseName As System.String Dim ProgId As System.String Dim MacroMethods As System.Object Dim ParamNames As System.Object Dim ParamTypes As System.Object Dim ParamValues As System.Object Dim DimTypes As System.Object Dim DimValues As System.Object Dim EditBodies As System.Object Dim IconFiles As System.Object Dim Options As System.Integer Dim value As Feature   value = instance.InsertMacroFeature3(BaseName, ProgId, MacroMethods, ParamNames, ParamTypes, ParamValues, DimTypes, DimValues, EditBodies, IconFiles, Options) ``` | |

| C# |  |
| --- | --- |
| ``` Feature InsertMacroFeature3(     System.string BaseName,    System.string ProgId,    System.object MacroMethods,    System.object ParamNames,    System.object ParamTypes,    System.object ParamValues,    System.object DimTypes,    System.object DimValues,    System.object EditBodies,    System.object IconFiles,    System.int Options ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ InsertMacroFeature3(  &   System.String^ BaseName, &   System.String^ ProgId, &   System.Object^ MacroMethods, &   System.Object^ ParamNames, &   System.Object^ ParamTypes, &   System.Object^ ParamValues, &   System.Object^ DimTypes, &   System.Object^ DimValues, &   System.Object^ EditBodies, &   System.Object^ IconFiles, &   System.int Options ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*BaseName*
:   Name of the base feature (see **Remarks**)

*ProgId*
:   COM or .NET callback object; empty string if VBA (see Remarks)

*MacroMethods*
:   Array of strings of size 9 only for VBA; "" otherwise (see Remarks)

*ParamNames*
:   Array of strings of the names of the parameters

*ParamTypes*
:   Array of the types of parameters of size paramCount as defined by swMacroFeatureParamType\_e

*ParamValues*
:   Array of strings of the values of parameters

*DimTypes*
:   Array of the types of dimensions as defined by swDimensionType\_e (see **Remarks**)

*DimValues*
:   Array of values of the dimensions

*EditBodies*
:   Array of [IBody2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html) objects to modify in the macro feature

*IconFiles*
:   Array of strings of the files names for the icons (see **Remarks**)

*Options*
:   Placement of the macro feature in the FeatureManager design tree as defined by swMacroFeatureOptions\_e (see **Remarks**)

#### Return Value

[IFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertMacroFeature3.

# ![](dotnetimages/collapse.gif)Example

[Create Macro Feature Subfeature (VBA)](Create_Macro_Feature_Subfeature_Example_VB.htm)

[Create Multibody Macro Feature (VBA)](Create_Multibody_Macro_Feature_Example_VB.htm)

[Create Multibody Macro Feature (VB.NET)](Create_Multibody_Macro_Feature_Example_VBNET.htm)

[Create Multibody Macro Feature (C#)](Create_Multibody_Macro_Feature_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

**BaseName**

* The argument BaseName is serialized within the feature and cannot be changed.

  * You can find out the name of the base feature by using [IMacroFeatureData::GetBaseName](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMacroFeatureData~GetBaseName.html).

    * The BaseName argument is also used to generate the name of the feature when the feature is first created.

**ProgId**

| **If creating a macro feature using...** | **Then ProgId is...** |
| --- | --- |
| COM callbacks | The name of the program ID for the component that implements the COM callback methods. The object that is represented by ProgID must support the ISwComFeature interface.  InsertMacroFeature3 ("Sample", "Sample.MyFeature", \_            Nothing, paramNames, paramTypes, \_                 paramValues, dimTypes, dimValues, \_                     editBodies, iconFiles, \_                        swMacroFeatureByDefault)  In the COM server, the Sample.Feature class is derived from ISwComFeature and implements rebuild, edit, and security functions. |
| VBA | An empty string.  InsertMacroFeature3("Sample", "",...) |
| .NET add-in callbacks | The name of the class that implements the .NET callbacks and ISwComFeature.  InsertMacroFeature3("Sample", "*project\_name.class\_module*",...) |

**MacroMethods**

> The macroMethods argument is implemented for VBA only. The array of nine strings consists of the following values:
>
> 1. Filename - File executed during feature generation.
>
>    - Module - Source module executed during feature generation.
>
>      - Procedure - Source procedure executed during feature generation.
>
>        - Filename - File executed after edit definition is selected.
>
>          - Module - Source module executed after edit definition is selected.
>
>            - Procedure - Source procedure executed after edit definition is selected.
>
>              - Filename - File executed while querying security; optional, see the next paragraph.
>
>                - Module - Source Module executed while querying security; optional, see the next paragraph.
>
>                  - Procedure - Source Procedure executed while querying security; optional, see the next paragraph.
>
> Filename should be the full pathname to the macro file. If the procedure resides in the same macro file that calls IFeatureManager::InsertMacroFeature3, then a call to [ISldWorks::GetCurrentMacroPathName](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~GetCurrentMacroPathName.html) provides all of the information necessary for the Filename.
>
> [IModelDoc2::ListAuxiliaryExternalFileReferences](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~ListAuxiliaryExternalFileReferences.html) returns an array containing the names of the features that include external references and an array containing the names of the external files for Filename elements 1, 4, and 7 in the array.
>
> The list of:

* features can contain duplicates, if the macro feature uses more than one procedure.

  * file names can contain duplicates if:

    + the procedures are implemented in the same macro file.

      + more than one instance of the same macro feature is present.

> If a security procedure is not used, then Filename, Module, and Procedure must all be empty strings.
>
> Procedure names must have an swm prefix in the name. This prefix identifies the procedures to execute.

**DimTypes**

Only these dimension types are supported by this method:

* swAngularDimension

  * swLinearDimension

    * swRadialDimension

**IconFiles**

> The array of the file names for the icons can contain either three or nine strings.
>
> | Number of strings in array | Types of images in this order | Image format and sizes |
> | --- | --- | --- |
> | Three | 1. Regular- Suppressed- Highlighted | * Windows bitmap (**\*.bmp**) format* 16 pixels wide X 18 pixels high |
> | Nine  **NOTES:**   * This size array is only valid for macro features created in parts, assemblies, and drawings in SOLIDWORKS 2017 and later.* SOLIDWORKS displays the appropriate images based on the current DPI setting of the display device. | 1. Regular small- Suppressed small- Highlighted small- Regular medium- Suppressed medium- Highlighted medium- Regular large- Suppressed large- Highlighted large | * Windows bitmap (**\*.bmp**) format* Recommended sizes are:     + Small: 20 pixels wide X 20 pixels high+ Medium: 32 pixels wide X 32 pixels high+ Large: 40 pixels wide X 40 pixels high |
>
> You can specify either the full path name or just the file name for the strings; for example, c:\bitmaps\icon1.bmp or icon1.bmp.

**Options**

> swMacroFeatureOptions\_e.swMacroFeatureEmbedMacroFile is not supported by programming languages for the Microsoft .NET Framework; for example, not supported by C#, Visual Basic .NET, or Managed C++.

See Overview of Macro Features for more information.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IFeatureManager::IInsertMacroFeature3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~IInsertMacroFeature3.html)

[IMacroFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0