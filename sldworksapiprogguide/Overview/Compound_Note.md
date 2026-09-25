<!-- source: sldworksapiprogguide/Overview/Compound_Note.htm -->

# SOLIDWORKS API Help

# Compound Note

In SOLIDWORKS 2015 and earlier, you could create compound notes. A compound
note was a note that contained multiple text strings and
sketch geometry. The compound note entities appeared to the end-user as though
they were one item. If the
user selected the compound note and dragged it, all of the entities and text
moved together.

As of SOLIDWORKS 2016, compound notes cannot be created either in the SOLIDWORKS
user interface or through the SOLIDWORKS API. For documents created
with SOLIDWORKS 2016 and later, instead of creating compound notes you can create
sketch blocks that function like compound notes using ISketchBlockDefinition and
ISketchBlockInstance. See [Block Definitions and Block Instances](Block_Definitions_and_Block_Instances.htm).

For documents created with SOLIDWORKS 2015 or earlier, you can use the following APIs
to create and/or modify compound notes:

**IAnnotation methods**

* IAnnotation::GetTextFormat
* IAnnotation::GetTextFormatCount
* IAnnotation::GetUseDocTextFormat
* IAnnotation::SetTextFormat

**IDrawingDoc methods**

* IDrawingDoc::CreateCompoundNote

**INote methods**

* INote::BeginSketchEdit
* INote::EndSketchEdit
* INote::GetCompoundTextAtIndex
* INote::GetCompoundTextCount
* INote::GetExtent
* INote::GetExtentAtIndex
* INote::GetHeightAtIndex
* INote::GetSketch
* INote::GetTextAtIndex
* INote::GetTextJustification
* INote::GetTextJustificationAtIndex
* INote::GetTextOffsetAtIndex
* INote::IsCompoundNote
* INote::SetTextAtIndex
* INote::SetTextJustificationAtIndex
* INote::SetTextOffsetAtIndex
* INote::SetTextPoint
* INote::SetZeroLengthLeader