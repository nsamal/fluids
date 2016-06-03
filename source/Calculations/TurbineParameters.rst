########################
Turbine Parameters
########################

.. todo:
 add this as a reference https://books.google.com/books?id=dY6a4bZg-LsC&pg=PA73&lpg=PA73&dq=loss+coefficient+definition&source=bl&ots=YenKAp-rO_&sig=e-oLWUWkZNtYtQCUq5N4Ud68qGA&hl=en&sa=X&ved=0ahUKEwiLupa3r_7MAhVM72MKHQ-tD60Q6AEIVDAI#v=onepage&q=loss coefficient definition&f=false

************************
Pressure Coefficients
************************

========================
Pressure Loss
========================

Pressure loss is a fractional value that compares the total pressure loss
against the dynamic head. [#]_ [#]_

.. math::

  Y = \frac{P_{t,x} - P_{t, inlet}} {P_{t,inlet} - P_{s,inlet}} = \frac {\Delta P_t} {\frac{1}{2}\rho v^2}

.. note:

  For rotating components use total pressure in the relative frame.

.. [#] http://www.energy.kth.se/courses/4A4314/material/GT2006-90105.pdf
.. [#] https://books.google.com/books?id=oGPLBQAAQBAJ&pg=PA737&lpg=PA737&dq=turbine+loss+coefficient&source=bl&ots=7gL9p4bJV5&sig=JzxcvRz6ARkHEyFguljBVG8nu7Q&hl=en&sa=X&ved=0ahUKEwjyt9qNt_7MAhVcVWMKHWhRCuk4FBDoAQgwMAM#v=onepage&q=turbine loss coefficient&f=false

========================
Pressure Recovery
========================

Pressure recovery is a ratio between the actual static pressure rise and the
ideal static pressure rise.

Ideally you would be able to fully recover all the kinetic energy from the
total pressure and turn it into a static pressure rise. ie: :math:`c_p=1.0`

.. math::

  c_p = \frac{P_{s,x} - P_{s, inlet}} {P_{t,inlet} - P_{s, inlet}} = \frac {\Delta P_s} {\frac{1}{2}\rho v^2}

**************
Reaction
**************
Reaction or degree of reaction describes the fraction of stage expansion which
occurs in the rotor. [#]_ [#]_

.. todo: insert benefit of using temperature vs pressure based reaction

A stage can be broken up into 3 interfaces or stations.

:Station 1: Stator inlet
:Station 2: Stator outlet/Rotor inlet
:Station 3: Rotor outlet

=============================
Enthalpy Based Reaction
=============================
.. math::

  \Lambda_h = \frac{h_2 - h_3}{h_1 - h_3}

=============================
Pressure Based Reaction
=============================
.. math::

  \Lambda_P = \frac{P_2 - P_3}{P_1 - P_3}

=============================
Temperature Based Reaction
=============================
.. math::

  \Lambda_T = \frac{T_2 - T_3}{T_1 - T_3}

=============================
Interpretation
=============================
Depending on the value of reaction this will tell you where the stage expansion
is occurring.

.. math::

  \begin{array}{llr}

  \Lambda = 0 & :  \thinspace & Only  \thinspace \Delta_{stator} \\
  0 \leq \Lambda \leq 0.50 & :  \thinspace & \Delta_{rotor} < \Delta_{stator} \\
  0.50 \leq \Lambda \leq 1.00  \thinspace & : & \Delta_{rotor} > \Delta_{stator} \\
  \Lambda = 1 & :  \thinspace & Only  \thinspace \Delta_{rotor} \\

  \end{array}

.. [#] https://en.wikipedia.org/wiki/Degree_of_reaction
.. [#] http://www.lth.se/fileadmin/tpe/Kurser/Chapter_4.pdf

**************
Swirl Angle
**************
The swirl angle indicates the angle between the meridional and tangential flow components.

========================
Absolute Swirl Angle
========================

.. math::

  \alpha = \arctan(v_{\theta}/v_{mer})

========================
Relative Swirl Angle
========================
Identical to to the absolute swirl angle however here we use velocities in the
relative frame.

.. math::

  \beta = \arctan(w_{\theta}/w_{mer})
