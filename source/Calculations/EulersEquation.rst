
************************
Eulers Equation
************************

Eulers equation relates the rate of change in momentum to a force.

==============
Definition
==============
.. math::
  dp = -\rho V \thinspace dV

:math:`p`
  pressure
:math:`\rho`
  density
:math:`V`
  velocity

==============
Derivation
==============

--------------
Diagram
--------------
We'll look at a infinitesimally small fluid element moving along a streamline.

.. todo:: insert diagram of fluid particle here

--------------
Assumptions
--------------
Assuming that the only the flow is steady, and the only significant sources of
force come from pressure.

Summary:

- the flow field doesn't change with time (steady)
- friction is negligible (inviscid)
- gravity is negligible

--------------
Derivation
--------------

If we apply Newton's second law in the stream wise direction (x).

.. math::
  \sum F = m a

and use the relationship between pressures and force.

.. math::
  F = p A

the force can be estimated using

.. math::
  \sum F = p \thinspace dy \thinspace dz - (p + dp) \thinspace dy \thinspace dz

We can then manipulate the equation by multiplying :math:`dp` by :math:`\frac{dx}{dx}`

.. math::
  \sum F = p \thinspace dy \thinspace dz - (p + \frac{dp}{dx}dx) \thinspace dy \thinspace dz

If you expand the right side and add these together you get the following.

.. math::
  \sum F = -\frac{dp}{dx}(dx \thinspace dy \thinspace dz)

We can also use the following relationships

.. math::
  :label: mass
  m = \rho V = \rho \thinspace dx \thinspace dy \thinspace dz

See equation :eq:`mass`.

.. math::
  :label: acceleration
  a = \frac {dV}{dt} = \frac {dV}{dx} \frac {dx}{dt} = \frac{dV}{dx}

Combining that information we obtain the following.
