<!-- source: obsoleteapi/ModelDoc2/ModelDoc2__AddRelation.htm -->

# ModelDoc2::AddRelation

This
method is obsolete and has been superseded by EquationMgr::Add.

Description

This method adds a new relation.

Syntax (OLE Automation)

void ModelDoc2.AddRelation ( relStr)

|  |  |  |
| --- | --- | --- |
| Input: | (BSTR) relStr | String containing the relationship to add |

Syntax (COM)

status = ModelDoc2->AddRelation
( relStr )

|  |  |  |
| --- | --- | --- |
| Input: | (BSTR) relStr | String containing the relationship to add |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

This method adds a new equation based on a relationship
between two items. For example, you could use the following relStr to
set the D2 dimension to twice the value of the D1 dimension:

"""D2@Sketch1""
= (""D1@Sketch1"" \* 2)"

For information about adding constraints,
see ModelDoc2::SketchAddConstraints.