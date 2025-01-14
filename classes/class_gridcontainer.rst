.. Generated automatically by doc/tools/makerst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the GridContainer.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_GridContainer:

GridContainer
=============

**Inherits:** :ref:`Container<class_Container>` **<** :ref:`Control<class_Control>` **<** :ref:`CanvasItem<class_CanvasItem>` **<** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

**Category:** Core

Brief Description
-----------------

Grid container used to arrange elements in a grid like layout.

Properties
----------

+-----------------------+------------------------------------------------------+
| :ref:`int<class_int>` | :ref:`columns<class_GridContainer_property_columns>` |
+-----------------------+------------------------------------------------------+

Theme Properties
----------------

+-----------------------+-------------+
| :ref:`int<class_int>` | hseparation |
+-----------------------+-------------+
| :ref:`int<class_int>` | vseparation |
+-----------------------+-------------+

Description
-----------

Grid container will arrange its children in a grid like structure, the grid columns are specified using the :ref:`columns<class_GridContainer_property_columns>` property and the number of rows will be equal to the number of children in the container divided by the number of columns. For example, if the container has 5 children, and 2 columns, there will be 3 rows in the container. Notice that grid layout will preserve the columns and rows for every size of the container.

Property Descriptions
---------------------

.. _class_GridContainer_property_columns:

- :ref:`int<class_int>` **columns**

+----------+--------------------+
| *Setter* | set_columns(value) |
+----------+--------------------+
| *Getter* | get_columns()      |
+----------+--------------------+

The number of columns in the ``GridContainer``. If modified, ``GridContainer`` reorders its children to accommodate the new layout.

