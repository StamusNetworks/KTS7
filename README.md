# OpenSearch Dashboards and Visualisations for Suricata

OpenSearch dashboards for use with [Suricata](https://suricata.io/) IDS/IPS/NSM

This repository provides 60 dashboards for OpenSearch for network threat detection and hunting use with
Suricata IDS/IPS/NSM - Intrusion Detection, Intrusion Prevention and Network Security Monitoring system.

These dashboards are for use with Suricata 8+, OpenSearch and comprise of more than 400 visualizations and 30 predefined searches.

The dashboards are already included by default in the [Clear NDR Community](https://www.stamus-networks.com/clear-ndr-community) distribution.

The dashboards list:

- [SN-ALERTS](README-Details.md#dashboard-sn-alerts)
- [SN-ALL](README-Details.md#dashboard-sn-all)
- [SN-ANOMALY](README-Details.md#dashboard-sn-anomaly)
- [SN-DHCP](README-Details.md#dashboard-sn-dhcp)
- [SN-DNP3](README-Details.md#dashboard-sn-dnp3)
- [SN-DNS](README-Details.md#dashboard-sn-dns)
- [SN-FILE-Transactions](README-Details.md#dashboard-sn-file-transactions)
- [SN-FLOW](README-Details.md#dashboard-sn-flow)
- [SN-FLOW-BITTORRENT](README-Details.md#dashboard-sn-flow-bittorrent)
- [SN-FLOW-DCERPC](README-Details.md#dashboard-sn-flow-dcerpc)
- [SN-FLOW-DHCP](README-Details.md#dashboard-sn-flow-dhcp)
- [SN-FLOW-DNP3](README-Details.md#dashboard-sn-flow-dnp3)
- [SN-FLOW-DNS](README-Details.md#dashboard-sn-flow-dns)
- [SN-FLOW-ENIP](README-Details.md#dashboard-sn-flow-enip)
- [SN-FLOW-FTP](README-Details.md#dashboard-sn-flow-ftp)
- [SN-FLOW-FTPDATA](README-Details.md#dashboard-sn-flow-ftpdata)
- [SN-FLOW-HTTP](README-Details.md#dashboard-sn-flow-http)
- [SN-FLOW-HTTP2](README-Details.md#dashboard-sn-flow-http2)
- [SN-FLOW-HUNT-ICMP-Exfil](README-Details.md#dashboard-sn-flow-hunt-icmp-exfil)
- [SN-FLOW-IKE](README-Details.md#dashboard-sn-flow-ike)
- [SN-FLOW-IMAP](README-Details.md#dashboard-sn-flow-imap)
- [SN-FLOW-KRB5](README-Details.md#dashboard-sn-flow-krb5)
- [SN-FLOW-LDAP](README-Details.md#dashboard-sn-flow-ldap)
- [SN-FLOW-MDNS](README-Details.md#dashboard-sn-flow-mdns)
- [SN-FLOW-MQTT](README-Details.md#dashboard-sn-flow-mqtt)
- [SN-FLOW-NFS](README-Details.md#dashboard-sn-flow-nfs)
- [SN-FLOW-NTP](README-Details.md#dashboard-sn-flow-ntp)
- [SN-FLOW-POP3](README-Details.md#dashboard-sn-flow-pop3)
- [SN-FLOW-QUIC](README-Details.md#dashboard-sn-flow-quic)
- [SN-FLOW-RDP](README-Details.md#dashboard-sn-flow-rdp)
- [SN-FLOW-RFB](README-Details.md#dashboard-sn-flow-rfb)
- [SN-FLOW-SIP](README-Details.md#dashboard-sn-flow-sip)
- [SN-FLOW-SMB](README-Details.md#dashboard-sn-flow-smb)
- [SN-FLOW-SMTP](README-Details.md#dashboard-sn-flow-smtp)
- [SN-FLOW-SNMP](README-Details.md#dashboard-sn-flow-snmp)
- [SN-FLOW-SSH](README-Details.md#dashboard-sn-flow-ssh)
- [SN-FLOW-TFTP](README-Details.md#dashboard-sn-flow-tftp)
- [SN-FLOW-TLS](README-Details.md#dashboard-sn-flow-tls)
- [SN-FLOW-WEBSOCKET](README-Details.md#dashboard-sn-flow-websocket)
- [SN-HTTP](README-Details.md#dashboard-sn-http)
- [SN-HUNT-1](README-Details.md#dashboard-sn-hunt-1)
- [SN-IDS](README-Details.md#dashboard-sn-ids)
- [SN-IKEv2](README-Details.md#dashboard-sn-ikev2)
- [SN-KRB5](README-Details.md#dashboard-sn-krb5)
- [SN-MQTT](README-Details.md#dashboard-sn-mqtt)
- [SN-NFS](README-Details.md#dashboard-sn-nfs)
- [SN-OVERVIEW](README-Details.md#dashboard-sn-overview)
- [SN-RDP](README-Details.md#dashboard-sn-rdp)
- [SN-RFB](README-Details.md#dashboard-sn-rfb)
- [SN-SANS-MTA-Training](README-Details.md#dashboard-sn-sans-mta-training)
- [SN-SIP](README-Details.md#dashboard-sn-sip)
- [SN-SMB](README-Details.md#dashboard-sn-smb)
- [SN-SMTP](README-Details.md#dashboard-sn-smtp)
- [SN-SNMP](README-Details.md#dashboard-sn-snmp)
- [SN-SSH](README-Details.md#dashboard-sn-ssh)
- [SN-STATS](README-Details.md#dashboard-sn-stats)
- [SN-TFTP](README-Details.md#dashboard-sn-tftp)
- [SN-TLS](README-Details.md#dashboard-sn-tls)
- [SN-TrafficID](README-Details.md#dashboard-sn-trafficid)
- [SN-VLAN](README-Details.md#dashboard-sn-vlan)

## How to use

To import all the visualizations and dashboards at once - on the host running the OpenSearch stack - simply import the `ClearNDRCommunity.ndjson` file located in the `API-DASHBOARDS/` folder. To do so go to `Dashboards Management` in OpenSearch , on the left hand side select `Saved objects`, click `Import` and select the `ClearNDRCommunity.ndjson` file.

**NOTE:**

You would need to select `logstash-*` as a default index once you open any dashboard for the first time after initial load/import.
A similar to this logstash conf could be used - https://github.com/StamusNetworks/SELKS/blob/master/staging/etc/logstash/conf.d/logstash.conf

For optimal results an example of elasticsearch/opensearch template has been included under `es-template\elasticsearch7-template.json`

