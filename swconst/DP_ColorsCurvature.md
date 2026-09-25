<!-- source: swconst/DP_ColorsCurvature.htm -->

# SOLIDWORKS API Help

# Document Properties > Colors > Curvature

The Curvature dialog appears when you click Curvature...
in Document Properties > Colors.  Click
Help on the Curvature dialog to
learn more about Curvature settings.

![](DP_ColorsCurvature.gif)

| Setting | Get/Set Methods | Return Value or <Value> | Comments |
| Curvature value 1 | IModelDocExtension::GetUserPreferenceDouble(swUserPreferenceDoubleValue\_e.swCurvatureValue1, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceDouble(swUserPreferenceDoubleValue\_e.swCurvatureValue1, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Double value between 0.0005 and 1000, inclusive | Maps the greatest curvature value to red |
| Curvature value 2 | IModelDocExtension::GetUserPreferenceDouble(swUserPreferenceDoubleValue\_e.swCurvatureValue2, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceDouble(swUserPreferenceDoubleValue\_e.swCurvatureValue2, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Double value between 0.0005 and 1000, inclusive | Maps the second greatest curvature value to green |
| Curvature value 3 | IModelDocExtension::GetUserPreferenceDouble(swUserPreferenceDoubleValue\_e.swCurvatureValue3, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceDouble(swUserPreferenceDoubleValue\_e.swCurvatureValue3, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Double value between 0.0005 and 1000, inclusive | Maps the third greatest curvature value to blue |
| Curvature value 4 | IModelDocExtension::GetUserPreferenceDouble(swUserPreferenceDoubleValue\_e.swCurvatureValue4, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceDouble(swUserPreferenceDoubleValue\_e.swCurvatureValue4, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Double value between 0.0005 and 1000, inclusive | Maps the fourth greatest curvature value to gray |
| Curvature value 5 | IModelDocExtension::GetUserPreferenceDouble(swUserPreferenceDoubleValue\_e.swCurvatureValue5, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  IModelDocExtension::SetUserPreferenceDouble(swUserPreferenceDoubleValue\_e.swCurvatureValue5, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <Value>) | Double value between 0.0005 and 1000, inclusive | Maps the least curvature value to black |