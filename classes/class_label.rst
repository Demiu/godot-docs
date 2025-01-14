.. Generated automatically by doc/tools/makerst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the Label.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_Label:

Label
=====

**Inherits:** :ref:`Control<class_Control>` **<** :ref:`CanvasItem<class_CanvasItem>` **<** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

**Category:** Core

Brief Description
-----------------

Displays plain text in a line or wrapped inside a rectangle. For formatted text, use :ref:`RichTextLabel<class_RichTextLabel>`.

Properties
----------

+----------------------------------+--------------------------------------------------------------------+
| :ref:`Align<enum_Label_Align>`   | :ref:`align<class_Label_property_align>`                           |
+----------------------------------+--------------------------------------------------------------------+
| :ref:`bool<class_bool>`          | :ref:`autowrap<class_Label_property_autowrap>`                     |
+----------------------------------+--------------------------------------------------------------------+
| :ref:`bool<class_bool>`          | :ref:`clip_text<class_Label_property_clip_text>`                   |
+----------------------------------+--------------------------------------------------------------------+
| :ref:`int<class_int>`            | :ref:`lines_skipped<class_Label_property_lines_skipped>`           |
+----------------------------------+--------------------------------------------------------------------+
| :ref:`int<class_int>`            | :ref:`max_lines_visible<class_Label_property_max_lines_visible>`   |
+----------------------------------+--------------------------------------------------------------------+
| :ref:`float<class_float>`        | :ref:`percent_visible<class_Label_property_percent_visible>`       |
+----------------------------------+--------------------------------------------------------------------+
| :ref:`String<class_String>`      | :ref:`text<class_Label_property_text>`                             |
+----------------------------------+--------------------------------------------------------------------+
| :ref:`bool<class_bool>`          | :ref:`uppercase<class_Label_property_uppercase>`                   |
+----------------------------------+--------------------------------------------------------------------+
| :ref:`VAlign<enum_Label_VAlign>` | :ref:`valign<class_Label_property_valign>`                         |
+----------------------------------+--------------------------------------------------------------------+
| :ref:`int<class_int>`            | :ref:`visible_characters<class_Label_property_visible_characters>` |
+----------------------------------+--------------------------------------------------------------------+

Methods
-------

+-----------------------+--------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>` | :ref:`get_line_count<class_Label_method_get_line_count>` **(** **)** const                       |
+-----------------------+--------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>` | :ref:`get_line_height<class_Label_method_get_line_height>` **(** **)** const                     |
+-----------------------+--------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>` | :ref:`get_total_character_count<class_Label_method_get_total_character_count>` **(** **)** const |
+-----------------------+--------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>` | :ref:`get_visible_line_count<class_Label_method_get_visible_line_count>` **(** **)** const       |
+-----------------------+--------------------------------------------------------------------------------------------------+

Theme Properties
----------------

+---------------------------------+-----------------------+
| :ref:`Font<class_Font>`         | font                  |
+---------------------------------+-----------------------+
| :ref:`Color<class_Color>`       | font_color            |
+---------------------------------+-----------------------+
| :ref:`Color<class_Color>`       | font_color_shadow     |
+---------------------------------+-----------------------+
| :ref:`Color<class_Color>`       | font_outline_modulate |
+---------------------------------+-----------------------+
| :ref:`int<class_int>`           | line_spacing          |
+---------------------------------+-----------------------+
| :ref:`StyleBox<class_StyleBox>` | normal                |
+---------------------------------+-----------------------+
| :ref:`int<class_int>`           | shadow_as_outline     |
+---------------------------------+-----------------------+
| :ref:`int<class_int>`           | shadow_offset_x       |
+---------------------------------+-----------------------+
| :ref:`int<class_int>`           | shadow_offset_y       |
+---------------------------------+-----------------------+

Enumerations
------------

.. _enum_Label_Align:

.. _class_Label_constant_ALIGN_LEFT:

.. _class_Label_constant_ALIGN_CENTER:

.. _class_Label_constant_ALIGN_RIGHT:

.. _class_Label_constant_ALIGN_FILL:

enum **Align**:

- **ALIGN_LEFT** = **0** --- Align rows to the left (default).

- **ALIGN_CENTER** = **1** --- Align rows centered.

- **ALIGN_RIGHT** = **2** --- Align rows to the right.

- **ALIGN_FILL** = **3** --- Expand row whitespaces to fit the width.

.. _enum_Label_VAlign:

.. _class_Label_constant_VALIGN_TOP:

.. _class_Label_constant_VALIGN_CENTER:

.. _class_Label_constant_VALIGN_BOTTOM:

.. _class_Label_constant_VALIGN_FILL:

enum **VAlign**:

- **VALIGN_TOP** = **0** --- Align the whole text to the top.

- **VALIGN_CENTER** = **1** --- Align the whole text to the center.

- **VALIGN_BOTTOM** = **2** --- Align the whole text to the bottom.

- **VALIGN_FILL** = **3** --- Align the whole text by spreading the rows.

Description
-----------

Label displays plain text on the screen. It gives you control over the horizontal and vertical alignment, and can wrap the text inside the node's bounding rectangle. It doesn't support bold, italics or other formatting. For that, use :ref:`RichTextLabel<class_RichTextLabel>` instead.

**Note:** Contrarily to most other :ref:`Control<class_Control>`\ s, Label's :ref:`Control.mouse_filter<class_Control_property_mouse_filter>` defaults to :ref:`Control.MOUSE_FILTER_IGNORE<class_Control_constant_MOUSE_FILTER_IGNORE>` (i.e. it doesn't react to mouse input events). This implies that a label won't display any configured :ref:`Control.hint_tooltip<class_Control_property_hint_tooltip>`, unless you change its mouse filter.

Property Descriptions
---------------------

.. _class_Label_property_align:

- :ref:`Align<enum_Label_Align>` **align**

+----------+------------------+
| *Setter* | set_align(value) |
+----------+------------------+
| *Getter* | get_align()      |
+----------+------------------+

Controls the text's horizontal align. Supports left, center, right, and fill, or justify. Set it to one of the ``ALIGN_*`` constants.

.. _class_Label_property_autowrap:

- :ref:`bool<class_bool>` **autowrap**

+----------+---------------------+
| *Setter* | set_autowrap(value) |
+----------+---------------------+
| *Getter* | has_autowrap()      |
+----------+---------------------+

If ``true``, wraps the text inside the node's bounding rectangle. If you resize the node, it will change its height automatically to show all the text. Default: ``false``.

.. _class_Label_property_clip_text:

- :ref:`bool<class_bool>` **clip_text**

+----------+----------------------+
| *Setter* | set_clip_text(value) |
+----------+----------------------+
| *Getter* | is_clipping_text()   |
+----------+----------------------+

If ``true``, the Label only shows the text that fits inside its bounding rectangle. It also lets you scale the node down freely.

.. _class_Label_property_lines_skipped:

- :ref:`int<class_int>` **lines_skipped**

+----------+--------------------------+
| *Setter* | set_lines_skipped(value) |
+----------+--------------------------+
| *Getter* | get_lines_skipped()      |
+----------+--------------------------+

The node ignores the first ``lines_skipped`` lines before it starts to display text.

.. _class_Label_property_max_lines_visible:

- :ref:`int<class_int>` **max_lines_visible**

+----------+------------------------------+
| *Setter* | set_max_lines_visible(value) |
+----------+------------------------------+
| *Getter* | get_max_lines_visible()      |
+----------+------------------------------+

Limits the lines of text the node shows on screen.

.. _class_Label_property_percent_visible:

- :ref:`float<class_float>` **percent_visible**

+----------+----------------------------+
| *Setter* | set_percent_visible(value) |
+----------+----------------------------+
| *Getter* | get_percent_visible()      |
+----------+----------------------------+

Limits the count of visible characters. If you set ``percent_visible`` to 50, only up to half of the text's characters will display on screen. Useful to animate the text in a dialog box.

.. _class_Label_property_text:

- :ref:`String<class_String>` **text**

+----------+-----------------+
| *Setter* | set_text(value) |
+----------+-----------------+
| *Getter* | get_text()      |
+----------+-----------------+

The text to display on screen.

.. _class_Label_property_uppercase:

- :ref:`bool<class_bool>` **uppercase**

+----------+----------------------+
| *Setter* | set_uppercase(value) |
+----------+----------------------+
| *Getter* | is_uppercase()       |
+----------+----------------------+

If ``true``, all the text displays as UPPERCASE.

.. _class_Label_property_valign:

- :ref:`VAlign<enum_Label_VAlign>` **valign**

+----------+-------------------+
| *Setter* | set_valign(value) |
+----------+-------------------+
| *Getter* | get_valign()      |
+----------+-------------------+

Controls the text's vertical align. Supports top, center, bottom, and fill. Set it to one of the ``VALIGN_*`` constants.

.. _class_Label_property_visible_characters:

- :ref:`int<class_int>` **visible_characters**

+----------+-------------------------------+
| *Setter* | set_visible_characters(value) |
+----------+-------------------------------+
| *Getter* | get_visible_characters()      |
+----------+-------------------------------+

Restricts the number of characters to display. Set to -1 to disable.

Method Descriptions
-------------------

.. _class_Label_method_get_line_count:

- :ref:`int<class_int>` **get_line_count** **(** **)** const

Returns the amount of lines of text the Label has.

.. _class_Label_method_get_line_height:

- :ref:`int<class_int>` **get_line_height** **(** **)** const

Returns the font size in pixels.

.. _class_Label_method_get_total_character_count:

- :ref:`int<class_int>` **get_total_character_count** **(** **)** const

Returns the total number of printable characters in the text (excluding spaces and newlines).

.. _class_Label_method_get_visible_line_count:

- :ref:`int<class_int>` **get_visible_line_count** **(** **)** const

Returns the number of lines shown. Useful if the ``Label``'s height cannot currently display all lines.

