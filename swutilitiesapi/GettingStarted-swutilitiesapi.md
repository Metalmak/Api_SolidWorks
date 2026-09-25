<!-- source: swutilitiesapi/GettingStarted-swutilitiesapi.html -->

![](images/collapse.gif)
![](images/expand.gif)
![](images/copycode.gif)
![](images/copycodeHighlight.gif)
![](images/drpdown.gif)
![](images/drpdown_orange.gif)

|  |
| --- |
|  |

|  |  |
| --- | --- |
| SOLIDWORKS Utilities API Help |  |
| Getting Started |
| Send comments on this topic. | |

Glossary Item Box

Writing a SOLIDWORKS Utilities application typically involves:

1. Opening the SOLIDWORKS document or documents, either interactively or programmatically.

   - Getting a pointer to the SOLIDWORKS Utilities interface.

     - If comparing faces on the SOLIDWORKS parts, [getting and setting the angular or position tolerances.](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.IUtilOptions.html)

       - Any of these actions:

- [Analyzing the geometry of a part](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.IGeometryAnalysis.html)

  - [Comparing features of the documents](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.ICompareFeature.html)

    - [Comparing geometry of the documents](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.ICompareGeometry.html)

      - [Comparing properties of the documents](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.ICompareDocument.html)

        - [Painting faces on the target part the same color as the source part](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.IFeaturePaint.html)

          - [Running a PowerSelect session](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.IPowerSelect.html)

            - [Running a thickness analysis](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.IThicknessAnalysis.html)

5. Displaying or saving the results to a file.

   - Performing any necessary cleanup.