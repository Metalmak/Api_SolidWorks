<!-- source: sldworksapiprogguide/Overview/Accessing_Attributes_Imported_from_ACIS_SAT_Files.htm -->

# SOLIDWORKS API Help

# Accessing Attributes Imported from ACIS SAT Files

After an SAT file containing generic attributes has been imported into
the SOLIDWORKS application, the attributes are imported as SOLIDWORKS
attributes. You can access these attributes using the standard SOLIDWORKS
attribute methods and properties.

The names of the attribute definitions are:

XLTR\_ATTRIBUTE\_DEFINITION\_DOUBLE\_TYPE for
ATTRIB\_GEN\_REAL

XLTR\_ATTRIBUTE\_DEFINITION\_STRING\_TYPE for
ATTRIB\_GEN\_STRING

XLTR\_ATTRIBUTE\_DEFINITION\_INTEGER\_TYPE for
ATTRIB\_GEN\_INTEGER

XLTR\_ATTRIBUTE\_DEFINITION\_DVECTOR\_TYPE for
ATTRIB\_GEN\_POSITION & ATTRIB\_GEN\_VECTOR

Each attribute definition has two parameters:

* Value.
  This parameter is of type swParamTypeString. It is of type swParamTypeDouble,
  swParamTypeString, swParamTypeInteger or swParamTypeDVector, depending
  on the attribute previously listed definitions.
* Name.
  The data contained in the Name parameter is the name of the attribute
  as defined in ACIS and the Value parameter contains the actual data in
  the attribute.