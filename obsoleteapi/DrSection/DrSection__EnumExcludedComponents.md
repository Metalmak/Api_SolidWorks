<!-- source: obsoleteapi/DrSection/DrSection__EnumExcludedComponents.htm -->

# DrSection::EnumExcludedComponents

This method is obsolete and has been superseded
by DrSection::EumExcludedComponents2.

Description

This method gets all of the assembly components
that are excluded from this section cut.

Syntax (OLE Automation)

See DrSection::GetExcludedComponents.

Syntax (COM)

status = DrSection->EnumExcludedComponents ( &exComps
)

| Output: | (LPENUMCOMPONENTS) exComps | Pointer to the EnumComponents object |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

The ability to exclude components from section
cuts applies only to assembly section views. For section views of parts,
this method returns NULL. To access the enumerated list of excluded components,
see the EnumComponents object.