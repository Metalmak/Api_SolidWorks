<!-- source: sldworksapiprogguide/Macro_Features/Macro_Features_and_Dimensions.htm -->

# SOLIDWORKS API Help

# Macro Features and Dimensions

The following sample code shows how you might create a dimension for
a macro feature.

1. In C++, create containers for the dimension types
   and values before inserting the macro feature:

 //Create
dimension containers

 long
dimType[MBossDimNum] =

 {

         swLinearDimension,

         swLinearDimension,

         swLinearDimension,

         swLinearDimension,

         swLinearDimension,

         swLinearDimension,

         swLinearDimension,

         swAngularDimension,

         swAngularDimension,

         swAngularDimension

 };

double dimValue[MBossDimNum] =

{

        pData->m\_BaseRadius\*2,

        pData->m\_BaseHeight,

        pData->m\_FinHeight,

        pData->m\_FinLength,

        pData->m\_FinWidth,

        pData->m\_InsideRadius\*2,

        pData->m\_InsideHeight,

        pData->m\_BaseDraft,

        pData->m\_FinDraft,

        pData->m\_InsideDraft

};

2. Insert the macro feature.

pFeatMan->IInsertMacroFeature2(\_bstr\_t(baseName),

        \_bstr\_t("SldFuncFeat.MBossFeature"),

        macroMethods,
MBossParamNum, MBossParamName,

        MBossParamType,
paramVal, MBossDimNum, dimType, dimValue, pEditBody,3,

        icons,
swMacroFeatureIsPatternable, &pFeat);

3. Set the lines for the dimensions in your rebuild
   function:

dim->put\_DimensionLineDirection(transformedVectLineDir);

dim->put\_ExtensionLineDirection(transformedVectExtDir);

dim->ISetReferencePoints(2,
refPoints);

NOTE: When regenerating a macro
feature, IDimension::ReferencePointsgets and sets the reference points of a display dimension (IDisplayDimension
object).  In
all other cases, this property gets and sets the reference points of a
dimension (IDimension
object).