=====================================================
OpenSearch Dashboards and Visualisations for Suricata
=====================================================

OpenSearch dashboards for use with `Suricata <https://suricata.io/>`_ IDS/IPS/NSM

This repository provides 58 dashboards for OpenSearch for network threat detection and hunting use with 
Suricata IDS/IPS/NSM - Intrusion Detection, Intrusion Prevention and Network Security Monitoring system.

These dashboards are for use with Suricata 8+, OpenSearch and comprise of more than 400 visualizations and 28 predefined searches.

The dashboards are already included by default in the `Clear NDR Community  <https://www.stamus-networks.com/clear-ndr-community>`_ distribution.

The dashboards list:

 - SN-ALERTS
 - SN-ALL
 - SN-ANOMALY
 - SN-DHCP
 - SN-DNP3
 - SN-DNS
 - SN-FILE-Transactions
 - SN-FLOW
 - SN-FLOW-BITTORRENT
 - SN-FLOW-DCERPC
 - SN-FLOW-DHCP
 - SN-FLOW-DNP3
 - SN-FLOW-DNS
 - SN-FLOW-ENIP
 - SN-FLOW-FTP
 - SN-FLOW-FTPDATA
 - SN-FLOW-HTTP
 - SN-FLOW-HTTP2
 - SN-FLOW-IKE
 - SN-FLOW-IMAP
 - SN-FLOW-KRB5
 - SN-FLOW-LDAP
 - SN-FLOW-MDNS
 - SN-FLOW-MQTT
 - SN-FLOW-NFS
 - SN-FLOW-NTP
 - SN-FLOW-POP3
 - SN-FLOW-QUIC
 - SN-FLOW-RDP
 - SN-FLOW-RFB
 - SN-FLOW-SIP
 - SN-FLOW-SMB
 - SN-FLOW-SMTP
 - SN-FLOW-SNMP
 - SN-FLOW-SSH
 - SN-FLOW-TFTP
 - SN-FLOW-TLS
 - SN-FLOW-WEBSOCKET
 - SN-HTTP
 - SN-HUNT-1
 - SN-IDS
 - SN-IKEv2
 - SN-KRB5
 - SN-MQTT
 - SN-NFS
 - SN-OVERVIEW
 - SN-RDP
 - SN-RFB
 - SN-SIP
 - SN-SMB
 - SN-SMTP
 - SN-SNMP
 - SN-SSH
 - SN-STATS
 - SN-TFTP
 - SN-TLS
 - SN-TrafficID
 - SN-VLAN
 

How to use
==========

To import all the visualizations and dashboards at once - on the host running the OpenSearch stack - simply import the ``ClearNDRCommunity.ndjson`` file located in the ``API-DASHBOARDS/`` folder. To do so go to ``Dashboards Management`` in OpenSearch , on the left hand side select ``Saved objects``, click ``Import`` and select the ``ClearNDRCommunity.ndjson`` file.

**NOTE:**     

You would need to select `logstash-*` as a default index once you open any dashboard for the first time after initial load/import. 
A similar to this logstash conf could be used - https://github.com/StamusNetworks/SELKS/blob/master/staging/etc/logstash/conf.d/logstash.conf 

For optimal results an example of elasticsearch/opensearch template has been included under ``es-template\elasticsearch7-template.json``

