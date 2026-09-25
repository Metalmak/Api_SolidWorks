<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICustomPropertyManager~Get6.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Get6 Method (ICustomPropertyManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICustomPropertyManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICustomPropertyManager.html) : Get6 Method (ICustomPropertyManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FieldName*
:   Name of the custom property

*UseCached*
:   True if the configuration has been activated, false if not (see Remarks)

*ValOut*
:   Value of the custom property

*ResolvedValOut*
:   Evaluated value of the custom property

*WasResolved*
:   True if the value was evaluated, false if not (see **Remarks**)

*LinkToProperty*
:   True to link FieldName to its parent part, false to not

Gets the value and the evaluated value of the specified custom property.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function Get6( _    ByVal FieldName As System.String, _    ByVal UseCached As System.Boolean, _    ByRef ValOut As System.String, _    ByRef ResolvedValOut As System.String, _    ByRef WasResolved As System.Boolean, _    ByRef LinkToProperty As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICustomPropertyManager Dim FieldName As System.String Dim UseCached As System.Boolean Dim ValOut As System.String Dim ResolvedValOut As System.String Dim WasResolved As System.Boolean Dim LinkToProperty As System.Boolean Dim value As System.Integer   value = instance.Get6(FieldName, UseCached, ValOut, ResolvedValOut, WasResolved, LinkToProperty) ``` | |

| C# |  |
| --- | --- |
| ``` System.int Get6(     System.string FieldName,    System.bool UseCached,    out System.string ValOut,    out System.string ResolvedValOut,    out System.bool WasResolved,    out System.bool LinkToProperty ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int Get6(  &   System.String^ FieldName, &   System.bool UseCached, &   [Out] System.String^ ValOut, &   [Out] System.String^ ResolvedValOut, &   [Out] System.bool WasResolved, &   [Out] System.bool LinkToProperty ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FieldName*
:   Name of the custom property

*UseCached*
:   True if the configuration has been activated, false if not (see Remarks)

*ValOut*
:   Value of the custom property

*ResolvedValOut*
:   Evaluated value of the custom property

*WasResolved*
:   True if the value was evaluated, false if not (see **Remarks**)

*LinkToProperty*
:   True to link FieldName to its parent part, false to not

#### Return Value

Result code as defined in swCustomInfoGetResult\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CustomPropertyManager::Get6.

# ![](dotnetimages/collapse.gif)Example

See the **Get Custom Properties for Configuration** examples in [ICustomPropertyManager](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICustomPropertyManager.html).

# ![](dotnetimages/collapse.gif)Remarks

This method returns configuration-specific, linked, and evaluated custom-property data more quickly than the now obsolete ICustomPropertyManager::Get2, if the configuration is previously activated.

This method gets the cached custom property, even if its configuration is not currently active.

|  |  |  |
| --- | --- | --- |
| If UseCached is set to... | And the configuration has already been activated... | Then... |
| True | Yes | Up-to-date data is returned and WasResolved = true |
| True | No | Cached data is returned and WasResolved = false |
| False | Yes | Up-to-date data is returned and WasResolved = true |
| False | No | Up-to-date data is returned and WasResolved = true |

If you always want up-to-date data, then you should set UseCached to false.

If the configuration is not previously activated, this method might take longer, as it loops through all of the model's configurations to find the specified custom property. When it finishes, the model might not be in its original configuration. To return the model to its original configuration, call [IModelDoc2::ForceRebuild3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ForceRebuild3.html) after calling this method.

This method does not preface the resolved evaluated values of external referenced documents with fromparent+, unlike the now obsolete ICustomPropertyManager::Get3.

# ![](dotnetimages/collapse.gif)See Also

####

[ICustomPropertyManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICustomPropertyManager.html)

[ICustomPropertyManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICustomPropertyManager_members.html)

[ICustomPropertyManager::GetAll3 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICustomPropertyManager~GetAll3.html)

[ICustomPropertyManager::GetNames Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICustomPropertyManager~GetNames.html)

[ICustomPropertyManager::GetType2 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICustomPropertyManager~GetType2.html)

[ICustomPropertyManager::Set2 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICustomPropertyManager~Set2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2018 FCS, Revision Number 26.0