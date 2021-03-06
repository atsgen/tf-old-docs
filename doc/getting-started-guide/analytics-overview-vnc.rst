.. This work is licensed under the Creative Commons Attribution 4.0 International License.
   To view a copy of this license, visit http://creativecommons.org/licenses/by/4.0/ or send a letter to Creative Commons, PO Box 1866, Mountain View, CA 94042, USA.

================================
Understanding Contrail Analytics
================================

Contrail is a distributed system of compute nodes, control nodes, configuration nodes, database nodes, web UI nodes, and analytics nodes.

The analytics nodes are responsible for the collection of system state information, usage statistics, and debug information from all of the software modules across all of the nodes of the system. The analytics nodes store the data gathered across the system in a database that is based on the Apache Cassandra open source distributed database management system. The database is queried by means of an SQL-like language and representational state transfer (REST) APIs.

System state information collected by the analytics nodes is aggregated across all of the nodes, and comprehensive graphical views allow the user to get up-to-date system usage information easily.

Debug information collected by the analytics nodes includes the following types:

- System log (syslog) messages—informational and debug messages generated by system software components.


- Object log messages—records of changes made to system objects such as virtual machines, virtual networks, service instances, virtual routers, BGP peers, routing instances, and the like.


- Trace messages—records of activities collected locally by software components and sent to analytics nodes only on demand.


Statistics information related to flows, CPU and memory usage, and the like is also collected by the analytics nodes and can be queried at the user interface to provide historical analytics and time-series information. The queries are performed using REST APIs.

Analytics data is written to a database in Contrail. The data expires after the default time-to-live (TTL) period of 48 hours. This default TTL time can be changed as needed by changing the value of the ``database_ttl`` value in the cluster configuration.

**Related Documentation**

-  `Contrail Alerts`_ 

-  `Analytics Scalability`_ 

-  `High Availability for Analytics`_ 

-  `Ceilometer Support in a Contrail Cloud`_ 

-  `Underlay Overlay Mapping in Contrail`_ 

-  `Monitoring the System`_ 

-  `Debugging Processes Using the Contrail Introspect Feature`_ 

-  `Monitor > Infrastructure > Dashboard`_ 

-  `Monitor > Infrastructure > Control Nodes`_ 

-  `Monitor > Infrastructure > Virtual Routers`_ 

-  `Monitor > Infrastructure > Analytics Nodes`_ 

-  `Monitor > Infrastructure > Config Nodes`_ 

-  `Monitor > Networking`_ 

-  Understanding Flow Sampling

-  `Query > Flows`_ 

-  `Query > Logs`_ 

-  `System Log Receiver in Contrail Analytics`_ 

-  `Example\:\ Debugging Connectivity Using Monitoring for Troubleshooting`_ 

.. _Contrail Alerts: alerts-overview.html

.. _Analytics Scalability: analytics-scalability-vnc.html

.. _High Availability for Analytics: ha-analytics-vnc.html

.. _Ceilometer Support in a Contrail Cloud: ceilometer-configuring.html

.. _Underlay Overlay Mapping in Contrail: underlay-overlay-mapping-vnc.html

.. _Monitoring the System: monitor-vnc.html

.. _Debugging Processes Using the Contrail Introspect Feature: introspect-process-debugging.html

.. _Monitor > Infrastructure > Dashboard: monitor-dashboard-vnc.html

.. _Monitor > Infrastructure > Control Nodes: monitoring-infrastructure-vnc.html

.. _Monitor > Infrastructure > Virtual Routers: monitoring-vrouters-vnc.html

.. _Monitor > Infrastructure > Analytics Nodes: monitor-analytics-vnc.html

.. _Monitor > Infrastructure > Config Nodes: monitor-config-vnc.html

.. _Monitor > Networking: monitoring-networking-vnc.html

.. _Understanding Flow Sampling: 

.. _Query > Flows: monitoring-flow-vnc.html

.. _Query > Logs: monitoring-syslog-vnc.html

.. _System Log Receiver in Contrail Analytics: syslog-receiver-vnc.html

.. _Example\:\ Debugging Connectivity Using Monitoring for Troubleshooting: debug-connectivity-vnc.html

