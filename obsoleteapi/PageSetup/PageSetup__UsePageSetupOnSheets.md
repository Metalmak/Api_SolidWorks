<!-- source: obsoleteapi/PageSetup/PageSetup__UsePageSetupOnSheets.htm -->

# PageSetup::UsePageSetupOnSheets

This property is obsolete and has been superseded
by ModelDocExtension::UsePageSetup.

Description

This property gets or sets whether or not the
settings associated with the PageSetup object for individual sheets page
setup objects overrides these settings.

Syntax (OLE Automation)

UseSheet = PageSetup.UsePageSetupOnSheets (VB Get
property)

PageSetup.UsePageSetupOnSheets = UseSheet (VB Set
property)

UseSheet = PageSetup.UsePageSetupOnSheets ( ) (C++
Get property)

PageSetup.UsePageSetupOnSheets ( UseSheet ) (C++
Set property)

| Property: | (BOOL) UseSheet | TRUE uses PageSetup for sheets, FALSE does not |

Syntax (COM)

status = PageSetup->get\_UsePageSetupOnSheets (
&UseSheet )

status = PageSetup->put\_UsePageSetupOnSheets (
UseSheet )

| Property: | (VARIANT\_BOOL) UseSheet | TRUE uses PageSetup for sheets, FALSE does not |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks