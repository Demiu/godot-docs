.. Generated automatically by doc/tools/makerst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the ScrollBar.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_ScrollBar:

ScrollBar
=========

**Inherits:** :ref:`Range<class_Range>` **<** :ref:`Control<class_Control>` **<** :ref:`CanvasItem<class_CanvasItem>` **<** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

**Inherited By:** :ref:`HScrollBar<class_HScrollBar>`, :ref:`VScrollBar<class_VScrollBar>`

**Category:** Core

Brief Description
-----------------

Base class for scroll bars.

Properties
----------

+---------------------------+----------------------------------------------------------+
| :ref:`float<class_float>` | :ref:`custom_step<class_ScrollBar_property_custom_step>` |
+---------------------------+----------------------------------------------------------+

Signals
-------

.. _class_ScrollBar_signal_scrolling:

- **scrolling** **(** **)**

Emitted when the scrollbar is being scrolled.

Description
-----------

Scrollbars are a :ref:`Range<class_Range>`-based :ref:`Control<class_Control>`, that display a draggable area (the size of the page). Horizontal (:ref:`HScrollBar<class_HScrollBar>`) and Vertical (:ref:`VScrollBar<class_VScrollBar>`) versions are available.

Property Descriptions
---------------------

.. _class_ScrollBar_property_custom_step:

- :ref:`float<class_float>` **custom_step**

+----------+------------------------+
| *Setter* | set_custom_step(value) |
+----------+------------------------+
| *Getter* | get_custom_step()      |
+----------+------------------------+

