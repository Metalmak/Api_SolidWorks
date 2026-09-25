<!-- source: sldworksapiprogguide/GettingStarted/Understanding_the_SolidWorks_API_Class_Hierarchy.htm -->

# SOLIDWORKS API Help

# Understanding the SOLIDWORKS API Class Hierarchy

SOLIDWORKS does not document its API with a complete class hierarchy
diagram, much like the famous MFC and .NET/WinFX class hierarchy diagrams.
The reason for this is that MFC and .NET rely heavily on:

* Classes
* Implementation inheritance
* Casting between classes using static casts (C++)

These types of class libraries and APIs can often benefit from a hierarchy
diagram.

 However,
SOLIDWORKS is a COM-based API that uses:

* Interfaces
* Interface inheritance
* Factory methods to return interfaces on existing
  and new objects
* Casting between interfaces through:

  + QueryInterface
    (C++), which
    returns a pointer to
    a specified interface on an object to which a client currently holds an
    interface pointer.
  + direct assignment (VB/VB.NET).
  + the is/as
    reserved words (C#).

While a graphical hierarchy diagram often does not convey as much information
in this style of API, there are a few places where it can be useful.

## Interface Inheritance in the SOLIDWORKS API

Objects that implement:

* IAssemblyDoc,
  IDrawingDoc,
  or IPartDoc
  can QueryInterface to IModelDoc2.
* IEdge,
  IFace2,
  IFeature,
  ILoop2,
  or IVertex
  can QueryInterface to IEntity.
* IBomTableAnnotation,
  IHoleTableAnnotation,
  IRevisionTableAnnotation,
  IWeldmentCutListAnnotation,
  and other table-annotation interfaces
  can QueryInterface to ITableAnnotation.
  See
  swTableAnnotationType\_e for a list of the interfaces that can
  QueryInterface to ITableAnnotation.
* IAttribute
  also can QueryInterface to IFeature.
* ISketchArc,
  ISketchEllipse,
  ISketchLine,
  ISketchParabola,
  ISketchPoint,
  ISketchSpline,
  or ISketchText
  can QueryInterface to ISketchSegment.
* PropertyManager page controls, such as IPropertyManagerPageActiveX,
  IPropertyManagerPageBitmap,
  IPropertyManagerPageBitmapButton,
  IPropertyManagerPageButton,
  etc., can QueryInterface to IPropertyManagerPageControl.

NOTE:
The phrase can QueryInterface
to is synonymous with implements
or can be assigned to in Visual
Basic.

While it is technically incorrect to say, for example, that IPartDoc
derives from IModelDoc2, the way that developers use these interfaces
is similar to the way they would use a derived class with implementation
inheritance.

## Using methods as an alternative to QueryInterface/Interface inheritance

There are several other areas of the API that use other methods to perform
operations similar to a QueryInterface().

* IAnnotation::GetSpecificAnnotation
  can return:

+ ICThread\*
+ IGtol\*
+ INote\*
+ others. See
  swAnnotationType\_e
  for a list of the types that can be returned

* IFeature::GetSpecificFeature2
  can return:

+ IAttribute\*
+ IMate2\*
+ ISketch\*
+ others.

## Accessors

To find out how to get a specific SOLIDWORKS interface or object from
other SOLIDWORKS interfaces or objects, use the Accessors
link located at the bottom of an interface's topic.

## Reference material

For more information on classes, objects, casting, interfaces, QueryInterface,
COM, and inheritance, see:

* Inside COM by Dale Rogerson. (Microsoft
  Press)
* Programming
  .NET Components by Juval Lowy (O'Reilly)