<!-- source: obsoleteapi/SldWorks/SldWorks__ActivePrinter.htm -->

# SldWorks::ActivePrinter

This property is obsolete and has been superseded
by ModelDoc2::Printer.

Description

This property gets or sets the active SolidWorks printer.

Syntax (OLE Automation)

printer = SldWorks.ActivePrinter (VB
Get property)

SldWorks.ActivePrinter = printer (VB
Set property)

printer = SldWorks.GetActivePrinter
( ) (C++ Get property)

SldWorks.SetActivePrinter ( printer
) (C++ Set property)

|  |  |  |
| --- | --- | --- |
| Property: | (BSTR) printer | Name of the printer |

Syntax (Com)

status = SldWorks->get\_ActivePrinter(
&printer )

status = SldWorks->put\_ActivePrinter(
printer )

|  |  |  |
| --- | --- | --- |
| Property: | (BSTR) printer | Name of the printer |
| Return: | (HRESULT)status | S\_OK if successful |

Remarks