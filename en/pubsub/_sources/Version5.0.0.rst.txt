
========================================================
Tigase PubSub Component--Version 5.0.0
========================================================

Welcome to Tigase PubSub component guide

1. PubSub Component
===================

Tigase\’s Publish Subscribe component is an XEP-0060 compliant plugin handling all publish and subscribe activity within Tigase server. This is enabled as default with the pubsub name, however you may include the following line if you wish to customize it\’s configuration.
.. code-block:: bash

   pubsub () {}

You may change the name so long as you specify the pubsub class within parenthesis.

1.1. Announcement
-----------------
1.1.1. Major changes
^^^^^^^^^^^^^^^^^^^^
Tigase pubsub component has undergone a few major changes to our code and structure. To continue to use Tigase pubsub component, a few changes may be needed to be made to your systems. Please see them below:

*Database schema changes*

Current version comes with changes to database schema to improve JID comparison during lookup of nodes, subscriptions, affiliations, etc.

To continue usage of new versions of pubsub component it is required to manually load new component database schema, see database preparation section for more information.

