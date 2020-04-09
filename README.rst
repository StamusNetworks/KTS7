===============================
Kibana 7 Templates for Suricata
===============================

Templates/Dashboards for Kibana 7 to use with `Suricata
<https://suricata-ids.org/>`_. Suricata IDPS/NSM threat hunting and the ELK 7 stack

This repository provides 26 templates for the Kibana 7.x and Elasticsearch 7.x
for use with Suricata IDS/IPS/NSM - Intrusion Detection, Intrusion Prevention and Network Security Monitoring system

These dashboards are for use with Suricata 5.1+ and enabled Rust build, Elasticsearch, Logstash, 
Kibana 7 and comprise of more than 250 visualizations and 24 predefined searches.

The dashboards are:

 - SN-ALERTS
 - SN-ALL
 - SN-ANOMALY
 - SN-DHCP
 - SN-DNS
 - SN-DNP3
 - SN-FILE-Transactions
 - SN-FLOW
 - SN-HTTP
 - SN-IDS
 - SN-IKEv2
 - SN-KRB5
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
 - SN-TLS
 - SN-VLAN
 - SN-TFTP
 - SN-TrafficID
 

How to use
==========

To import all the vizualizasitons and dahsboards to Kibana 7 using the native API - on the host runing Kibana 7 or ELK7: ::

 cd API-KIBANA7
 curl -X POST "localhost:5601/api/saved_objects/_import" -H 'kbn-xsrf: true' --form file=@index-pattern.ndjson
 curl -X POST "localhost:5601/api/saved_objects/_import" -H 'kbn-xsrf: true' --form file=@search.ndjson
 curl -X POST "localhost:5601/api/saved_objects/_import" -H 'kbn-xsrf: true' --form file=@visualization.ndjson 
 curl -X POST "localhost:5601/api/saved_objects/_import" -H 'kbn-xsrf: true' --form file=@dashboard.ndjson
 service kibana restart

The rest of the folder structure set up is Scirius CE specific and not needed in the manual import.

You would need to select ``logstash-*`` as a default index once you open any dashboard for the first time after initial load/import.  

A similar to this logstash template could be used - https://github.com/StamusNetworks/SELKS/blob/SELKS5/staging/etc/logstash/conf.d/logstash.conf

For optimal results an example of elasticsearch template has been included under ``es-template\elasticsearch7-template.json`` that is used in SELKS 6.
