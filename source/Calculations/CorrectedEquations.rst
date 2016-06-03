########################
Corrected Equations
########################

************************
Correction Terms
************************

-----------------------------
Pressure Correction Factor
-----------------------------
The pressure correction factor corrects to a reference or standard pressure. [#]_ [#]_.

.. math::
  \delta = P/P_{ref}

where

:math:`P`
  the actual pressure.
:math:`P_{ref}`
  the reference pressure. Typically :math:`P_{ref} = 1 \thinspace atm = 101.326 \thinspace kPa = 14.696 \thinspace psia`

.. [#] The first automatic.
.. [#] https://en.wikipedia.org/wiki/Atmosphere_(unit)

.. todo:: Get the source

-----------------------------
Temperature Correction Factor
-----------------------------
.. math::
  \theta = T/T_{ref}

.. todo:: Get the source


-----------------------------
Gas Correction Factor
-----------------------------
hello


************************
Corrected Equations
************************
Corrected parameters correct for pressure and temperature.

-----------------
Corrected Flow
-----------------

.. math::

  w_{corr} = \frac{w\sqrt{\theta}}{\delta}

-----------------
Corrected Speed
-----------------

Corrected speed corrects to standard temperature. [#]_.

.. math::

  N_{corr} = \frac{N}{\sqrt{\theta}}

.. [#] https://en.wikipedia.org/wiki/Corrected_speed


Corrected

************************
Equivalent Equations
************************
Equivalent parameters correct for pressure, temperature as well as gas property changes.

-----------------------------
Equivalent Flow
-----------------------------

-----------------------------
Equivalent Power
-----------------------------
