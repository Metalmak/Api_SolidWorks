<!-- source: obsoleteapi/AssemblyDoc/AssemblyDoc__CompConfigProperties2.htm -->

# AssemblyDoc::CompConfigProperties2

This
method is obsolete and has been superseded by [AssemblyDoc::CompConfigProperties3](AssemblyDoc__CompConfigProperties3.htm).

Description

This method sets the configuration properties for the selected component.

Syntax (OLE Automation)

retval = AssemblyDoc.CompConfigProperties2
( m\_suppressed, showComp, m\_fdetail)

| Input: | (long) m\_suppressed | Suppression state of this component instance as defined in swComponentSuppressionState\_e |
| Input: | (BOOL) showComp | TRUE if you want to show the selected component in the graphics display area, if not   | If the selected component is a... | Then... | | Part | Setting this option also sets the m\_fdetail option | | Sub-assembly | You can hide the component in the graphics area and still show its details in the FeatureManager design tree | |
| Input: | (BOOL) m\_fdetail | TRUE if you want the feature details for this component to be displayed in the FeatureManager design tree, FALSE if you want to see only the component name in the FeatureManager design tree.   | If the selected component is a... | Then... | | Part | Setting this option also sets the m\_show\_component option | | Sub-assembly | You can hide the feature details in the FeatureManager design tree and still show the component in the graphics area | |
| Return: | (BOOL) retval | TRUE if successful, FALSE if not |

Syntax (COM)

status = AssemblyDoc->CompConfigProperties2(
m\_suppressed, m\_show\_component, m\_fdetail, &retval )

| Input: | (long) m\_suppressed | Suppression state of this component instance as defined in swComponentSuppressionState\_e. |
| Input: | (VARIANT\_BOOL) showComp | TRUE if you want to show the selected component in the graphics display area, if not   | If the selected component is a... | Then... | | Part | Setting this option also sets the m\_fdetail option | | Sub-assembly | You can hide the component in the graphics area and still show its details in the FeatureManager design tree | |
| Input: | (BOOL) m\_fdetail | TRUE if you want the feature details for this component to be displayed in the FeatureManager design tree, FALSE if you want to see only the component name in the FeatureManager design tree.   | If the selected component is a... | Then... | | Part | Setting this option also sets the m\_show\_component option | | Sub-assembly | You can hide the feature details in the FeatureManager design tree and still show the component in the graphics area | |
| Output: | (VARIANT\_BOOL) retval | TRUE if successful, FALSE if not |
| Return: | (HRESULT)status | S\_OK if successful |

Remarks

You can use configurations
to save certain display characteristics with each of the assembly components
and retrieve that configuration in the future. SolidWorks applies the
settings that you specify with this method to the active configuration.

You cannot set a component to lightweight (that
is,  m\_suppressed
= swComponentLightweight is not valid).

Known reasons for failure of this method include:

* Invalid suppression
  state specified
* Not preselecting
  a component