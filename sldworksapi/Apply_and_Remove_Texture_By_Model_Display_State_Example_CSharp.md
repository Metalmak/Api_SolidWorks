<!-- source: sldworksapi/Apply_and_Remove_Texture_By_Model_Display_State_Example_CSharp.htm -->

# SOLIDWORKS API Help

# Apply and Remove Texture To and From Model By Display State Example (C#)

This example shows how to apply and remove texture to and from a model by a
display state.

//------------------------------------------------------
// Preconditions:
// 1. Verify that the specified part and texture exist.
// 2. Open the Immediate window.
//
// Postconditions:
// 1. Opens the specified part and applies texture to the part.
// 2. Examine the part
// 3. In the IDE, click the **Continue** button at

//    System.Diagnostics.Debugger.Break().
// 4. Removes the texture from the selected face.
// 5. Examine the Immediate window and part.
//
// NOTE: Because the part is used elsewhere, do not save
// changes.
//----------------------------------------------------

using

 SolidWorks.Interop.sldworks;

using

 SolidWorks.Interop.swconst;

using

 System;

using

 System.Diagnostics;

    namespace

ApplyRemoveTextureByDisplayStateCSharp.csproj

    {

partial class
SolidWorksMacro

         {

public void
Main()

{

ModelDoc2 swModel =
default(ModelDoc2);
> > > ModelDocExtension
> > > swModelDocExt = default(ModelDocExtension);
> > >
> > > Texture
> > > texture = default(Texture);
> > >
> > > string
> > > displayState = null;
> > >
> > > int
> > > errors = 0;
> > >
> > > int
> > > warnings = 0;
> > >
> > > string
> > > namStr = null;
> > >
> > > // Open document
> > >
> > > swModel = (
> > >
> > > ModelDoc2)swApp.**OpenDoc6**("C:\\Users\\Public\\Documents\\SOLIDWORKS\SOLIDWORKS
> > > 2018\\samples\\tutorial\\motionstudies\\valve.sldprt",
> > > (int)swDocumentTypes\_e.swDocPART,
> > > (int)swOpenDocOptions\_e.swOpenDocOptions\_Silent,
> > > "",
> > > ref
> > > errors, ref
> > > warnings);
> > >
> > > swModelDocExt = (
> > >
> > > ModelDocExtension)
> > > swModel.**Extension**;
> > >
> > > // Set texture on
> > > model in the
> > >
> > > //
> > > specified display state
> > >
> > > displayState =
> > >
> > > "<Default>\_Display State 1";
> > >
> > > namStr =
> > >
> > > "<SystemTexture>\\images\\textures\\pattern\\checker2.jpg";
> > >
> > > texture = (
> > >
> > > Texture)
> > > swModelDocExt.**CreateTexture**(namStr, 5, 45,
> > > false);Debug.Print("Texture
> > > set: " + swModelDocExt.**SetTextureByDisplayState**(displayState,
> > > texture));

               //
Examine the selected face to verify

               //
that the specified texture was set

               //
In the IDE, click the Continue button to resume

               //
running macro

               System.Diagnostics.Debugger.Break();

> > > // Remove
> > > texture from model by display state
> > >
> > > Debug.Print("Texture
> > > removed: " + swModelDocExt.**RemoveTextureByDisplayState**(displayState));
> > >
> > > // Rebuild model
> > >
> > > swModel.**ForceRebuild3**(
> > >
> > > false);

}

> > ///
> > <summary>
> >
> > ///
> > The SldWorks swApp variable is pre-assigned for you.
> > ///
> > </summary>
> >
> > public
> > SldWorks
> > swApp;

    }

}