########################
Fundamental Principles
########################

.. toctree::
   :maxdepth: 2

   EulersEquation.rst

************************
Conservation Laws
************************

========================
Conservation of Mass
========================

.. todo: insert stuff here

************************
Dimensionless Parameters
************************

===================
Reynolds Number
===================

Reynolds number is a dimensionless parameter that can be derived using
the Buckingham Pi theorem. [#]_ Reynolds number tells us how the inertial forces
compare to the viscous forces in our flow field. [#]_

.. math::

  Re = \frac{\rho v d}{\mu} = \frac{v d}{\nu} \thinspace \approx \thinspace \frac{F_{inertial}}{F_{viscous}}

:math:`\rho`
  density
:math:`v`
  velocity
:math:`d`
  the relevant dimension *ie: length or diameter*
:math:`\mu`
  kinematic viscoscity
:math:`\nu`
  dynamic viscoscity

.. [#] https://en.wikipedia.org/wiki/Buckingham_π_theorem
.. [#] https://en.wikipedia.org/wiki/Reynolds_number
