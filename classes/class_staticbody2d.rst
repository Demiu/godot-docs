.. Generated automatically by doc/tools/makerst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the StaticBody2D.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_StaticBody2D:

StaticBody2D
============

**Inherits:** :ref:`PhysicsBody2D<class_PhysicsBody2D>` **<** :ref:`CollisionObject2D<class_CollisionObject2D>` **<** :ref:`Node2D<class_Node2D>` **<** :ref:`CanvasItem<class_CanvasItem>` **<** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

**Category:** Core

Brief Description
-----------------

Static body for 2D physics.

Properties
----------

+-----------------------------------------------+-----------------------------------------------------------------------------------------+
| :ref:`float<class_float>`                     | :ref:`bounce<class_StaticBody2D_property_bounce>`                                       |
+-----------------------------------------------+-----------------------------------------------------------------------------------------+
| :ref:`float<class_float>`                     | :ref:`constant_angular_velocity<class_StaticBody2D_property_constant_angular_velocity>` |
+-----------------------------------------------+-----------------------------------------------------------------------------------------+
| :ref:`Vector2<class_Vector2>`                 | :ref:`constant_linear_velocity<class_StaticBody2D_property_constant_linear_velocity>`   |
+-----------------------------------------------+-----------------------------------------------------------------------------------------+
| :ref:`float<class_float>`                     | :ref:`friction<class_StaticBody2D_property_friction>`                                   |
+-----------------------------------------------+-----------------------------------------------------------------------------------------+
| :ref:`PhysicsMaterial<class_PhysicsMaterial>` | :ref:`physics_material_override<class_StaticBody2D_property_physics_material_override>` |
+-----------------------------------------------+-----------------------------------------------------------------------------------------+

Description
-----------

Static body for 2D physics. A StaticBody2D is a body that is not intended to move. It is ideal for implementing objects in the environment, such as walls or platforms.

Additionally, a constant linear or angular velocity can be set for the static body, which will affect colliding bodies as if it were moving (for example, a conveyor belt).

Property Descriptions
---------------------

.. _class_StaticBody2D_property_bounce:

- :ref:`float<class_float>` **bounce**

+----------+-------------------+
| *Setter* | set_bounce(value) |
+----------+-------------------+
| *Getter* | get_bounce()      |
+----------+-------------------+

The body's bounciness. Values range from ``0`` (no bounce) to ``1`` (full bounciness).

.. _class_StaticBody2D_property_constant_angular_velocity:

- :ref:`float<class_float>` **constant_angular_velocity**

+----------+--------------------------------------+
| *Setter* | set_constant_angular_velocity(value) |
+----------+--------------------------------------+
| *Getter* | get_constant_angular_velocity()      |
+----------+--------------------------------------+

The body's constant angular velocity. This does not rotate the body, but affects colliding bodies, as if it were rotating.

.. _class_StaticBody2D_property_constant_linear_velocity:

- :ref:`Vector2<class_Vector2>` **constant_linear_velocity**

+----------+-------------------------------------+
| *Setter* | set_constant_linear_velocity(value) |
+----------+-------------------------------------+
| *Getter* | get_constant_linear_velocity()      |
+----------+-------------------------------------+

The body's constant linear velocity. This does not move the body, but affects colliding bodies, as if it were moving.

.. _class_StaticBody2D_property_friction:

- :ref:`float<class_float>` **friction**

+----------+---------------------+
| *Setter* | set_friction(value) |
+----------+---------------------+
| *Getter* | get_friction()      |
+----------+---------------------+

The body's friction. Values range from ``0`` (no friction) to ``1`` (full friction).

.. _class_StaticBody2D_property_physics_material_override:

- :ref:`PhysicsMaterial<class_PhysicsMaterial>` **physics_material_override**

+----------+--------------------------------------+
| *Setter* | set_physics_material_override(value) |
+----------+--------------------------------------+
| *Getter* | get_physics_material_override()      |
+----------+--------------------------------------+

