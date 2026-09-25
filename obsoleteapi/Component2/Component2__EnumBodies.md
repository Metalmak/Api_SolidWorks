<!-- source: obsoleteapi/Component2/Component2__EnumBodies.htm -->

# Component2::EnumBodies

This method is obsolete and
has been superseded by Component2::EnumBodies2.

Description

This method gets the bodies in the component
in a multibody part.

Syntax (OLE Automation)

enumBodies = Component2.EnumBodies ( bodyType )

| Input: | (long) bodyType | Type of body as defined by swBodyType\_e |
| Output: | (LPENUMBODIES2) enumBodies | Pointer to list of bodies |

Syntax (COM)

status = Component2->EnumBodies ( bodyType, &enumBodies
)

| Input: | (long) bodyType | Type of body as defined by swBodyType\_e |
| Output: | (LPENUMBODIES2) enumBodies | Pointer to list of bodies |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

This method only supports
solid and sheet body types.