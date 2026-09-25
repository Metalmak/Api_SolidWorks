<!-- source: sldworksapi/Get_Entity_Name_Example_CPlusPlus_COM.htm -->

# SOLIDWORKS API Help

# Get Entity Name Example (C++ COM)

This example shows how to get the name of the
IEntity object.

BSTR entityName;

res = m\_PartDoc->IGetEntityName(m\_Entity,
&entityName);

CString
message;

message.Format(\_T("Entity
Name is: \t%s"), entityName);

AfxMessageBox(
message );

SysFreeString(entityName);