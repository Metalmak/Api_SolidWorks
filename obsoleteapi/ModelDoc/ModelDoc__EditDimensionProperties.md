<!-- source: obsoleteapi/ModelDoc/ModelDoc__EditDimensionProperties.htm -->

# ModelDoc::EditDimensionProperties

This
method is now obsolete and has been superseded by [ModelDoc::EditDimensionProperties2](ModelDoc__EditDimensionProperties2.htm).

Description

This method edits the currently selected dimension's
properties.

Syntax (OLE Automation)

retval = ModelDoc.EditDimensionProperties ( tolType, tolMax, tolMin, tolMaxFit, tolMinFit, useDocPrec,
precision, arrowsIn, useDocArrows, arrow1, arrow2 )

|  |  |  |
| --- | --- | --- |
| Input: | (long) tolType | Type of tolerance you want to use as defined in swTolType\_e |
| Input: | (double) tolMax | Maximum value for the tolerance |
| Input: | (double) tolMin | Minimum value for the tolerance |
| Input: | (BSTR) tolMaxFit | Text string for the maximum FIT value when using a fit tolerance type |
| Input: | (BSTR) tolMinFit | Text string for the maximum FIT value when using a fit tolerance type |
| Input: | (BOOL) useDocPrec | TRUE to use the documents precision value, FALSE otherwise |
| Input: | (long) precision | Precision value to use for this dimension |
| Input: | (long) arrowsIn | Value for the arrow direction as defined in swDimensionArrowsSide\_e |
| Input: | (BOOL) useDocArrows | TRUE to use the documents arrow types, FALSE otherwise |
| Input: | (long) arrow1 | Type of arrow to use on the first arrow of this dimension as defined in swArrowStyle\_e |
| Input: | (long) arrow2 | Type of arrow to use on the second arrow of this dimension as defined in swArrowStyle\_e |
| Return: | (BOOL) retval | TRUE if the dimension was successfully edited, FALSE otherwise |

Syntax (COM)

status = ModelDoc->EditDimensionProperties ( tolType,
tolMax, tolMin, tolMaxFit, tolMinFit, useDocPrec, precision, arrowsIn,
useDocArrows, arrow1, arrow2, &retval )

|  |  |  |
| --- | --- | --- |
| Input: | (long) tolType | Type of tolerance you want to use as defined in swTolType\_e |
| Input: | (double) tolMax | Maximum value for the tolerance |
| Input: | (double) tolMin | Minimum value for the tolerance |
| Input: | (BSTR) tolMaxFit | Maximum FIT value when using a fit tolerance type |
| Input: | (BSTR) tolMinFit | Maximum FIT value when using a fit tolerance type |
| Input: | (VARIANT\_BOOL) useDocPrec | TRUE to use the documents precision value, FALSE otherwise |
| Input: | (long) precision | Precision value to use for this dimension |
| Input: | (long) arrowsIn | Value for the arrow direction as defined in swDimensionArrowsSide\_e |
| Input: | (VARIANT\_BOOL) useDocArrows | TRUE to use the documents arrow types, FALSE otherwise |
| Input: | (long) arrow1 | Type of arrow to use on the first arrow of this dimension as defined in swArrowStyle\_e |
| Input: | (long) arrow2 | Type of arrow to use on the second arrow of this dimension as defined in swArrowStyle\_e |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks