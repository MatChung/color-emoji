# Color Emoji support in OpenType #

This project consists of the following components:

  * A proposed specification to add support for embedded color image glyphs in OpenType fonts.  See the links section on the left for the live version of the specification,

  * A tool called emoji\_builder.py, to embed a set of PNG images into an existing fonts,

  * Two sets of sample PNG images for ASCII characters and sample scripts to build them into test fonts: FruityGirl and Funkster.

  * Scripts to build a real color emoji font out of the Open Source PhantomOpenEmoji images.

The above bits are in the default git repository of the project.

There are also the following git trees available:

  * freetype2: A fully functional patch to the FreeType text rasterizer to support this specification,

  * freetype2-demos: Adjust demo tools to render color fonts.  Requires the above freetype2 tree,

  * skia: Support new color bitmaps in the FreeType font host,

  * cairo: A proof-of-concept version of the Cairo graphics library to use the above FreeType library and use fallback software rendering for the Xlib backend, with support for color glyphs.

The patches are in the 'color-emoji' branch of the trees.  Note that the freetype2 and freetype2-demos patches were upstreamed on May 29, 2013.

The built versions of the fonts can be downloaded from the "Sample fonts" link on the left.  All three are licensed under OFL and can be used for testing in other projects.