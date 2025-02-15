+++++++++++++++
Gamepad Look
+++++++++++++++

.. figure:: /images/Logic_Nodes/gamepad_look_node.png
   :align: right
   :width: 215
   :alt: Gamepad Look Node.

The *Gamepad Look* node is a quick way to make objects follow controller stick movement.
It's possible to assign a *Body* and a *Head* object.

If no *Head* object is assigned, the body will be used for both axis, but
that is generally discouraged as it can lead to unwanted side effects.

Parameters
==========

Axis
   Which stick of the controller to use for the transformation.

Inputs
=======

Condition
   Input Condition.

Main Object
   This is the body object

Head (Optional)
   This is the head object. If set, both objects will be rotated along their corresponding local axis.

Invert XY
   Option to invert movement for each axis (Vec2).

Index
   The index of the controller to poll.

Sensitivity
   Multiplier for translating mouse movement to object rotation.

Exponent
   Exponent for fine-tuning the stick behavior.

Cap Left/Right
   Limit the body objects rotation on its local Z axis.

X Limits
   The limits for the body objects local Z rotaion (Vec2).

Cap Up/Down
   Limit the head object's rotation on its local X/Y axis.

Y Limits
   The limits for the head object's local X/Y rotaion (Vec2).

Threshold
   Ignore stick values under this threshold.

Outputs
=======

Done
   *True* if the node performed successfully, else *False*
