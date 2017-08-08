CECA - User Guide
=================

Table of Contents
-----------------




Getting Started
---------------

- basic CECA description, most common application scenarios, etc.




Provisioning
------------

- based on PNDA guide.

================================================================================


CECA - Connector Model
----------------------

Description
~~~~~~~~~~~

- What is this subsystem;
- How to setup it in dashboard (if applicable);
- Dashboard screens (illustration), indicating user information displayed on screen.


Model Diagram
~~~~~~~~~~~~~

- More technical details on the subsystem (tech report);
- Uml or Graphical Diagrams.


Setup and Workflow
~~~~~~~~~~~~~~~~~~

- Basic workflow description (describe how it does what it does);
- Configuration files location (if applicable);
- Config file parameters description (if optional or not, accepted values, consequences of misconfiguration, etc).
- Developing a new CECA connector.

Example
~~~~~~~

- a simple example description and setup for the given subsystem;
- expected results, with screenshots and descriptions (the alarms, logs, etc);
- make any configuration files available on Github.

================================================================================

CECA - Camera Subsystem
-----------------------

Description
~~~~~~~~~~~

- What is this subsystem;
- How to setup it in dashboard (if applicable);
- Dashboard screens (illustration), indicating user information displayed on screen.


Model Diagram
~~~~~~~~~~~~~

- More technical details on the subsystem (tech report);
- Uml or Graphical Diagrams.


Setup and Workflow
~~~~~~~~~~~~~~~~~~

- Basic workflow description (describe how it does what it does);
- Configuration files location (if applicable);
- Config file parameters description (if optional or not, accepted values, consequences of misconfiguration, etc).

- VSM References for setup
- Camera CRUD and Setup

Example
~~~~~~~

- a simple example description and setup for the given subsystem;
- expected results, with screenshots and descriptions (the alarms, logs, etc);
- make any configuration files available on Github.

================================================================================

CECA - Basic Sensor Subsystem
-----------------------------

Description
~~~~~~~~~~~

- What is this subsystem;
- How to setup it in dashboard (if applicable);
- Dashboard screens (illustration), indicating user information displayed on screen.
- Focused on Temperature, humidity and smoke sensors.

Model Diagram
~~~~~~~~~~~~~

- More technical details on the subsystem (tech report);
- Uml or Graphical Diagrams.


Setup and Workflow
~~~~~~~~~~~~~~~~~~

- Basic workflow description (describe how it does what it does);
- Configuration files location (if applicable);
- Config file parameters description (if optional or not, accepted values, consequences of misconfiguration, etc).

- Sensor CRUD and Setup

Example
~~~~~~~

- a simple example description and setup for the given subsystem;
- expected results, with screenshots and descriptions (the alarms, logs, etc);
- make any configuration files available on Github.

================================================================================

CECA - Person/Asset Location subsystem
--------------------------------------

Description
~~~~~~~~~~~

- What is this subsystem;
- How to setup it in dashboard (if applicable);
- Dashboard screens (illustration), indicating user information displayed on screen.
- Focused on Person and asset location.
- Routing mechanism description.

Model Diagram
~~~~~~~~~~~~~

- More technical details on the subsystem (tech report);
- Uml or Graphical Diagrams.


Setup and Workflow
~~~~~~~~~~~~~~~~~~

- Basic workflow description (describe how it does what it does);
- Configuration files location (if applicable);
- Config file parameters description (if optional or not, accepted values, consequences of misconfiguration, etc).

- Sensor CRUD and Setup
- CMX Basic setup (description or reference to Bootstrap section)

Example
~~~~~~~

- a simple example description and setup for the given subsystem;
- expected results, with screenshots and descriptions (the alarms, logs, etc);
- make any configuration files available on Github.

================================================================================

CECA - Alerts Subsystem
-----------------------

Description
~~~~~~~~~~~

- What is this subsystem;
- How to setup it in dashboard (if applicable);
- Dashboard screens (illustration), indicating user information displayed on screen.
- Focused on common alerts description.
- For advanced alerts confioguration, link to Correlation Events (Rule Monitor)
- Describes call manager integration.

Model Diagram
~~~~~~~~~~~~~

- More technical details on the subsystem (tech report);
- Uml or Graphical Diagrams.


Setup and Workflow
~~~~~~~~~~~~~~~~~~

- Basic workflow description (describe how it does what it does);
- Configuration files location (if applicable);
- Config file parameters description (if optional or not, accepted values, consequences of misconfiguration, etc).

- Sensor CRUD and Setup
- Call manager basic setup (description or reference to Bootstrap section)

Example
~~~~~~~

- a simple example description and setup for the given subsystem;
- expected results, with screenshots and descriptions (the alarms, logs, etc);
- make any configuration files available on Github.


================================================================================

CECA - Correlation Events SubSystem
-----------------------------------

**Description**


Basically, decision tables provides a compact way to model complex rule sets and
their respective actions, for business logic or even a semantic rule applied to
an specific problem. It is simply an approach to model rules and actions (a good
one, but not the only one).

In a decision table, business logic is well divided into conditions, actions
(decisions) and rules for representing the various components that form the
given problem logic.

Moreover, decision table is a way to decision making that involves considering a
variety of conditions and their interrelationships, particular for complex
interrelationships.

While it is desirable to have an analytics engine to provide additional
information, decision taking and predictive analysis for a Big Data system,
it is also relevant to point out that a SCCT is able to provide flexibility
since it can be defined to setup a basic set of unusual issues which might need
immediate actions (since it is known that any analytic problem needs data collection
and processing before going into field operation).

The figure depicted below illustrates this concept:

+------------------------+------------------------+
| Condition Variables    | Condition Alternatives |
+------------------------+------------------------+
| Actions                | Action Exec. Order     |
+------------------------+------------------------+

- **Conditions** : the variables (or simple relation) that needs to be matched
- **Condition Alternatives** : the value of the condition, usually 'True', 'False' or 'Don't Care'; eventually an advanced DT may allow more complex conditions;
- **Actions** : procedures, functions or methods associated with the problem domain of that specific DT;
- **Action Entries** : flags or sequencer ids associated with the respective Actions which will be triggered when a given condition is fulfilled.

In CECA, this concept was implemented through an easy going interface, where user
can define his own set of rules according to the alarms and events in need of
triggering.

This subsystem can be accessed through the "Event Correlation" menu option:

Wikipedia_
.. _Wikipedia: http://www.wikipedia.org/

    .. image:: images/eventcorrelation_01.png


- What is this subsystem;
- How to setup it in dashboard (if applicable);
- Dashboard screens (illustration), indicating user information displayed on screen.


Model Diagram
~~~~~~~~~~~~~

- More technical details on the subsystem (tech report);
- Uml or Graphical Diagrams.


Setup and Workflow
~~~~~~~~~~~~~~~~~~

- Basic workflow description (describe how it does what it does);
- Configuration files location (if applicable);
- Config file parameters description (if optional or not, accepted values, consequences of misconfiguration, etc).

Example
~~~~~~~

- a simple example description and setup for the given subsystem;
- expected results, with screenshots and descriptions (the alarms, logs, etc);
- make any configuration files available on Github.


================================================================================

CECA - The Bootstrap procedure
------------------------------

Description
~~~~~~~~~~~

- What is this phase;
- How to setup it in dashboard (if applicable);
- Dashboard screens (illustration), indicating user information displayed on screen.


Model Diagram
~~~~~~~~~~~~~

- More technical details on the subsystem (tech report);
- Uml or Graphical Diagrams.


Setup and Workflow
~~~~~~~~~~~~~~~~~~

- Basic workflow description (describe how it does what it does);
- Configuration files location (if applicable);
- Config file parameters description (if optional or not, accepted values, consequences of misconfiguration, etc).

- PNDA Setup (description and/or references)
- Talend Setup
- Tropo Setup
- Cisco Spark Setup
- VSM Setup
- CMX Setup
- Security issues or constraints (if necessary to mention)

- Cameras Setup
- Sensors setup
- Sensor CRUD
- Plant Upload
- Logical Setup of a Plant (Hierarchy model)
- Connectors setup (configuration)
- HBase configuration (if applicable)
- Kafka configuration (if applicable)

Example
~~~~~~~

- a simple example description and setup for the given subsystem;
- expected results, with screenshots and descriptions (the alarms, logs, etc);
- make any configuration files available on Github.

================================================================================

Troubleshooting
---------------

- most common known issues and their solution (storage issues, restarting the system, corrupted log files, etc);


================================================================================

References
----------
