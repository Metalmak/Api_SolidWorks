<!-- source: obsoleteapi/ModelDoc/ModelDoc__EditDimensionProperties2.htm -->

# ModelDoc::EditDimensionProperties2

This
method is obsolete and has been superseded by [ModelDoc2::EditDimensionProperties2](../ModelDoc2/ModelDoc2__EditDimensionProperties2.htm).

Description

This method edits the currently selected dimension's
properties.

Syntax (OLE Automation)

retval = ModelDoc.EditDimensionProperties2 ( tolType,
tolMax, tolMin, tolMaxFit, tolMinFit, useDocPrec, precision, arrowsIn,
useDocArrows, arrow1, arrow2, prefixText, suffixText, showValue, calloutText1,
calloutText2, centerText )

|  |  |  |
| --- | --- | --- |
| Input: | (long) tolType | Type of tolerance you want to use as defined in swTolType\_e |
| Input: | (double) tolMax | Maximum value for the tolerance |
| Input: | (double) tolMin | Minimum value for the tolerance. |
| Input: | (BSTR) tolMaxFit | Text string for the maximum FIT value when using a fit tolerance type |
| Input: | (BSTR) tolMinFit | Text string for the maximum FIT value when using a fit tolerance type |
| Input: | (BOOL) useDocPrec | TRUE to use the documents precision value, FALSE otherwise |
| Input: | (long) precision | Precision value to use for this dimension |
| Input: | (long) arrowsIn | Value for the arrow direction as defined in swDimensionArrowsSide\_e |
| Input: | (BOOL) useDocArrows | TRUE to use the documents arrow types, FALSE otherwise |
| Input: | (long) arrow1 | Type of arrow to use on the first arrow of this dimension as defined in swArrowStyle\_e |
| Input: | (long) arrow2 | Type of arrow to use on the second arrow of this dimension as defined in swArrowStyle\_e |
| Input: | (BSTR) prefixText | String you want to display as the prefix of this dimension |
| Input: | (BSTR) suffixText | String that you want to display as the suffix of this dimension |
| Input: | (BOOL) showValue | TRUE if you want to display the value of this dimension in the user interface, FALSE otherwise |
| Input: | (BSTR) calloutText1 | Callout text above the dimension |
| Input: | (BSTR) calloutText2 | Callout text below the dimension |
| Input: | (BOOL) centerText | TRUE if you want to center the text in this dimension, FALSE otherwise |
| Return: | (BOOL) retval | TRUE if the dimension was successfully edited, FALSE otherwise |

Syntax (COM)

status = ModelDoc->EditDimensionProperties2 (
tolType, tolMax, tolMin, tolMaxFit, tolMinFit, useDocPrec, precision,
arrowsIn, useDocArrows, arrow1, arrow2, prefixText, suffixText, showValue,
calloutText1, calloutText2, centerText, &retval )

|  |  |  |
| --- | --- | --- |
| Input: | (long) tolType | Type of tolerance you'd like to use. See swTolType\_e. |
| Input: | (double) tolMax | Maximum value for the tolerance. |
| Input: | (double) tolMin | Minimum value for the tolerance. |
| Input: | (BSTR) tolMaxFit | Text string for the maximum FIT value when using a fit tolerance type |
| Input: | (BSTR) tolMinFit | Text string for the maximum FIT value when using a fit tolerance type |
| Input: | (VARIANT\_BOOL) useDocPrec | TRUE to use the documents precision value, FALSE otherwise |
| Input: | (long) precision | Precision value to use for this dimension |
| Input: | (long) arrowsIn | Value for the arrow direction. See swDimensionArrowsSide\_e |
| Input: | (VARIANT\_BOOL) useDocArrows | TRUE to use the documents arrow types, FALSE otherwise |
| Input: | (long) arrow1 | Type of arrow to use on the first arrow of this dimension as defined in swArrowStyle\_e |
| Input: | (long) arrow2 | Type of arrow to use on the second arrow of this dimension as defined in swArrowStyle\_e |
| Input: | (BSTR) prefixText | String you want to display as the prefix of this dimension |
| Input: | (BSTR) suffixText | String that you want to display as the suffix of this dimension |
| Input: | (VARIANT\_BOOL) showValue | TRUE if you want to display the value of this dimension in the user interface, FALSE otherwise |
| Input: | (BSTR) calloutText1 | Callout text above the dimension |
| Input: | (BSTR) calloutText2 | Callout text below the dimension |
| Input: | (VARIANT\_BOOL) centerText | TRUE if you want to center the text in this dimension, FALSE otherwise |
| Output: | (VARIANT\_BOOL) retval | TRUE if the dimension was successfully edited, FALSE otherwise |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks