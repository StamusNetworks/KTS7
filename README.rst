============================================================
OpenSearch Kibana Dashboards and Visualisations for Suricata
============================================================

Dashboards for Kibana to use with `Suricata
<https://suricata.io/>`_. Suricata IDS/IPS/NSM network threat hunting and the OpenSearch stack.

This repository provides 55 dashboards for Kibana and OpenSearch for network threat detection use with 
Suricata IDS/IPS/NSM - Intrusion Detection, Intrusion Prevention and Network Security Monitoring system.

These dashboards are for use with Suricata 8+, OpenSearch and Kibana and comprise of more than 400 visualizations and 24 predefined searches.

The dashboards are already included by default in the `Clear NDR Community  <https://www.stamus-networks.com/clear-ndr-community>`_ distribution.

The dashboards are:

 - SN-SMB
 - SN-SNMP
 - SN-HUNT-1
 - SN-SIP
 - SN-MQTT
 - SN-KRB5
 - SN-RFB
 - SN-IKEv2
 - SN-ALERTS
 - SN-ALL
 - SN-DNS
 - SN-FILE-Transactions
 - SN-FLOW
 - SN-HTTP
 - SN-IDS
 - SN-OVERVIEW
 - SN-SMTP
 - SN-SSH
 - SN-STATS
 - SN-TLS
 - SN-VLAN
 - SN-TFTP
 - SN-DHCP
 - SN-TrafficID
 - SN-RDP
 - SN-ANOMALY
 - SN-DNP3
 - SN-NFS
 - SN-FLOW-HTTP
 - SN-FLOW-SMTP
 - SN-FLOW-SMB
 - SN-FLOW-DNS
 - SN-FLOW-TLS
 - SN-FLOW-NTP
 - SN-FLOW-FTPDATA
 - SN-FLOW-DCERPC
 - SN-FLOW-KRB5
 - SN-FLOW-DHCP
 - SN-FLOW-QUIC
 - SN-FLOW-MDNS
 - SN-FLOW-LDAP
 - SN-FLOW-FTP
 - SN-FLOW-SIP
 - SN-FLOW-BITTORRENT
 - SN-FLOW-WEBSOCKET
 - SN-FLOW-HTTP2
 - SN-FLOW-SNMP
 - SN-FLOW-TFTP
 - SN-FLOW-IMAP
 - SN-FLOW-POP3
 - SN-FLOW-IKE
 - SN-FLOW-ENIP
 - SN-FLOW-DNP3
 - SN-FLOW-SSH
 - SN-FLOW-NFS
 

How to use
==========

To import all the visualizations and dashboards - on the host running Kibana with the OpenSearch stack - simply import the ``ClearNDRCommunity.ndjson`` file located in the ``API-KIBANA7/`` folder.
