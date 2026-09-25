<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICustomPropertyManager~Get3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Get3 Method (ICustomPropertyManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICustomPropertyManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICustomPropertyManager.html) : Get3 Method (ICustomPropertyManager) |

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
:   True if configuration has been activated, false if not (see Remarks)

*ValOut*
:   Value of the custom property

*ResolvedValOut*
:   Evaluated value of the custom property

Obsolete. Superseded by [ICustomPropertyManager::Get4](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICustomPropertyManager~Get4.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function Get3( _    ByVal FieldName As System.String, _    ByVal UseCached As System.Boolean, _    ByRef ValOut As System.String, _    ByRef ResolvedValOut As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICustomPropertyManager Dim FieldName As System.String Dim UseCached As System.Boolean Dim ValOut As System.String Dim ResolvedValOut As System.String Dim value As System.Boolean   value = instance.Get3(FieldName, UseCached, ValOut, ResolvedValOut) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool Get3(     System.string FieldName,    System.bool UseCached,    out System.string ValOut,    out System.string ResolvedValOut ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool Get3(  &   System.String^ FieldName, &   System.bool UseCached, &   [Out] System.String^ ValOut, &   [Out] System.String^ ResolvedValOut ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FieldName*
:   Name of the custom property

*UseCached*
:   True if configuration has been activated, false if not (see Remarks)

*ValOut*
:   Value of the custom property

*ResolvedValOut*
:   Evaluated value of the custom property

#### Return Value

True if up-to-date data is returned, false if not (see Remarks)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CustomPropertyManager::Get3.

# ![](dotnetimages/collapse.gif)Remarks

This method can get the cached custom property, even if the configuration is not currently active, without having to change configurations.

|  |  |  |
| --- | --- | --- |
| If UseCached is set to... | And the configuration has already been activated... | Then... |
| True | Yes | * Up-to-date data is returned and return value = True |
| True | No | * Cached data is returned and return value = False |
| False | Yes | * Up-to-date data is returned and return value = True |
| False | No | * Up-to-date data is returned and return value = True |

This method returns configuration-specific, linked, custom-property, evaluated data more quickly than the now obsolete [ICustomPropertyManager::Get2 method](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICustomPropertyManager~Get2.html), if the configuration was previously activated.

If you always want up-to-date data, then you should set UseCached to false. This may result in a more time-consuming call if the configuration was not previously activated.

# ![](dotnetimages/collapse.gif)See Also

####

[ICustomPropertyManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICustomPropertyManager.html)

[ICustomPropertyManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICustomPropertyManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 SP4, Revision Number 16.4