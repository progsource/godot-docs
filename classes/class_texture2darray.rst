:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/master/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/master/doc/classes/Texture2DArray.xml.

.. _class_Texture2DArray:

Texture2DArray
==============

**Inherits:** :ref:`ImageTextureLayered<class_ImageTextureLayered>` **<** :ref:`TextureLayered<class_TextureLayered>` **<** :ref:`Texture<class_Texture>` **<** :ref:`Resource<class_Resource>` **<** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

A single texture resource which consists of multiple, separate images. Each image has the same dimensions and number of mipmap levels.

Description
-----------

A Texture2DArray is different from a Texture3D: The Texture2DArray does not support trilinear interpolation between the :ref:`Image<class_Image>`\ s, i.e. no blending.

A Texture2DArray is also different from an :ref:`AtlasTexture<class_AtlasTexture>`: In a Texture2DArray, all images are treated separately. In an atlas, the regions (i.e. the single images) can be of different sizes. Furthermore, you usually need to add a padding around the regions, to prevent accidental UV mapping to more than one region. The same goes for mipmapping: Mipmap chains are handled separately for each layer. In an atlas, the slicing has to be done manually in the fragment shader.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
