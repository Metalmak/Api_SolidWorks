<!-- source: sldworksapiprogguide/Overview/Accessing_Bodies_in_Body_Folders.htm -->

# SOLIDWORKS API Help

# Accessing Bodies in Body Folders

The IBodyFolder
interface lets you access bodies in solid, surface, and various weldment
body folders.

1. If traversing the FeatureManager design tree,
   then use IFeature::GetTypeName
   to determine the type of feature. If the feature is any of the following
   types, then you have a body folder feature:

* SolidBodyFolder
* SurfaceBodyFolder
* CutListFolder
* SubWeldFolder
* SubAtomFolder

- or -

If you selected a folder and it is any of
the following types of folders, then you have a body folder feature:

* swSelBODYFOLDER
* swSelSUBATOMFOLDER
* swSelSUBWELDFOLDER

NOTE:
A top-level folder feature named Cut
list is identified as SolidBodyFolder, a solid body folder feature.
Any subfolder feature named Cut-List-Item
is identified CutListFolder, a cut list subfolder feature.

2. Call IFeature::GetSpecificFeature2
   to get the BodyFolder interface.
3. Call IBodyFolder::Type
   to get the type of body folder.
4. Call IBodyFolder::GetBodyCount
   to get the number
   of bodies in the folder and call IBodyFolder::GetBodies
   to get the bodies in the folder in the order in which they appear in the
   FeatureManager design tree.

   NOTE: These methods deal only with the bodies in the folder; they do
   not include the bodies within any subfolders. You must call IFeature::GetFirstSubFeature
   and IFeature::GetNextSubFeature
   to traverse through the subfolders.
5. To get the feature for a body, call IBodyFolder::GetFeature.