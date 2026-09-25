<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~ReloadOrReplace.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ReloadOrReplace Method (IModelDocExtension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : ReloadOrReplace Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ReadOnly*
:   True to set the model document read-only after reload or replace, false to allow write access

*ReplaceFileName*
:   Replacement model document; null or Nothing to reload the current model document

*DiscardChanges*
:   True to discard changes made to the current model document, false to abort operation if the model document was changed (see **Remarks**)

*ForceReload*
:   True to force the reload, false to not

Reloads or replaces this model document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ReloadOrReplace( _    ByVal ReadOnly As System.Boolean, _    ByVal ReplaceFileName As System.String, _    ByVal DiscardChanges As System.Boolean, _    ByVal ForceReload As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim ReadOnly As System.Boolean Dim ReplaceFileName As System.String Dim DiscardChanges As System.Boolean Dim ForceReload As System.Boolean Dim value As System.Integer   value = instance.ReloadOrReplace(ReadOnly, ReplaceFileName, DiscardChanges, ForceReload) ``` | |

| C# |  |
| --- | --- |
| ``` System.int ReloadOrReplace(     System.bool ReadOnly,    System.string ReplaceFileName,    System.bool DiscardChanges,    System.bool ForceReload ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int ReloadOrReplace(  &   System.bool ReadOnly, &   System.String^ ReplaceFileName, &   System.bool DiscardChanges, &   System.bool ForceReload ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ReadOnly*
:   True to set the model document read-only after reload or replace, false to allow write access

*ReplaceFileName*
:   Replacement model document; null or Nothing to reload the current model document

*DiscardChanges*
:   True to discard changes made to the current model document, false to abort operation if the model document was changed (see **Remarks**)

*ForceReload*
:   True to force the reload, false to not

#### Return Value

Error codes as defined by swComponentReloadError\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::ReloadOrReplace.

# ![](dotnetimages/collapse.gif)Example

[Reload Model (VBA)](Reload_Model_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

The model to reload or replace must be open in its own window frame.

This method does not reload or replace the model if the top assembly has been opened invisibly. In that case, make the model visible by calling [IModelDoc2::Visible](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~Visible.html) before calling this method.

You must call this method after calling [IModelDoc2::ForceReleaseLocks](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~ForceReleaseLocks.html), which detaches a file from the file system, to re-attach a detached file to the file system. If you do not call this method after calling IModelDoc2::ForceReleaseLocks, then you will experience problems with OLE objects (e.g., design tables). Any changes made to a file while it is detached are not preserved unless you save the file to disk before calling this method. Additionally if you set this method's DiscardChanges parameter to false and you made changes to a detached file that you are attempting to re-attach to the file system, then this method will fail. DiscardChanges must be set to true to re-attach a detached file.

See [ISldWorks::CloseAndReopen](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~CloseAndReopen.html) to perform a similar function with drawing documents.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2022 FCS, Revision Number 30