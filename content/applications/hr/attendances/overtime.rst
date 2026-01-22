=================
Overtime rulesets
=================

Odoo's **Attendances** app allows for the configuration of overtime rules to determine if and when
employees earn overtime, and at what rate. No overtime rulesets come preconfigured in the
**Attendances** app; all overtime rulesets must be created individually.

Create an overtime ruleset
==========================

To create an overtime ruleset, navigate to :menuselection:`Attendances app --> Configuration -->
Overtime Rulesets`.

.. note::
   Any existing overtime rulesets appear in a default list view, and displays the ruleset
   :guilabel:`Name`, the :guilabel:`Rate Mode`, and the :guilabel:`Rules Count` (the number of rules
   configured for the ruleset).

Click the :guilabel:`New` button, and a blank :guilabel:`Ruleset` form loads. Enter the following
information on the top-half of the form:

- :guilabel:`Ruleset Name`: Enter a name for the ruleset.
- :guilabel:`Rate Combination Mode`: Using the drop-down menu, select how the overtime rate is
  calculated. The options are:

  - :guilabel:`Maximum Rate`: The highest rate is used to determine the overtime pay. For example,
    if there are two available rates of 150% and 125%, the highest available rate, 150%, is applied.
  - :guilabel:`Sum of all rates`: A combination of all applicable rates is used to calculate the
    overtime pay. For example, if two rates apply, 150% and 120%, a rate of 170% is applied.

- :guilabel:`Description`: Enter a brief description for the ruleset.
- :guilabel:`Country`: Using the drop-down menu, select the country the ruleset applies to.

Overtime rules
--------------

Once the main information of the ruleset is created, the next step is to add the individual rules.
Click :guilabel:`Add a line` at the bottom of the :guilabel:`Overtime Rules` tab of the
:guilabel:`Ruleset` form, and a :guilabel:`Create Rule` pop-up window loads.

Enter the :guilabel:`Rule Name` in the corresponding field. Next, enter the following information in
the :guilabel:`Definition` tab:

Condition section
~~~~~~~~~~~~~~~~~

- :guilabel:`The rule is based on?`: Select when overtime applies. the options are:

  - :guilabel:`Quantity`: Select this option if overtime is accrued when the total logged hours for
    a day or week exceed what is expected.
  - :guilabel:`Timing`: Select this option if overtime is accrued only on specific days or at
    specific times.

- :guilabel:`If the worked hours on a (Day/Week) differes`: First, select if the total expected time
  is calculated by the :guilabel:`Day` or :guilabel:`Week`, using the drop down menu. Next, select
  if the difference is compared:

  - :guilabel:`from the amount defined on the contract`: Select this option if the overtime is based
    on the working hours :ref:`definied on the employees contract <payroll/gen-info>`.
  - :guilabel:`from a specific duration`: Select this option if the overtime is based on a
    specified amount of time. If this is selected, a :guilabel:`Duration to exceed` field appears.
    Enter the number of :guilabel:`hours` in an `HH:MM` format the employee must exceed each
    :guilabel:`Day` or :guilabel:`Week`, depending on what is selected in the :guilabel:`If the
    worked hours on a (Day/Week) differes` field.

- :guilabel:`With a tolerance in favor of the employer of`:
- :guilabel:`With a tolerance in favor of the employee of`:

Action section
~~~~~~~~~~~~~~

- :guilabel:`Pay extra hours`:   - :guilabel:`Work entry type to use`:
- :guilabel:`Give back as time off`:


