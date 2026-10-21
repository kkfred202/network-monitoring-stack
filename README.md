# Network Monitoring and Alerting Stack

## **Overview**
This project documents a monitoring setup for the lab network using **SNMPv3**, **syslog** and **NetFlow**, with **Grafana** dashboards and alerts. It finishes with a runbook for the first alert a NOC would handle: an interface going down.

## **Lab Setup**
- **Monitoring Server:** Linux VM running LibreNMS or Zabbix, plus Grafana
- **Network Devices:** the routers and switches from the earlier labs
- **Alert Destination:** email, Teams, Slack or Discord webhook

## **Project Objectives**
- Discover devices with **SNMPv3**
- Collect **syslog** messages and filter by severity
- Export **NetFlow** and find the top talkers
- Build a **Grafana** dashboard for interfaces, errors, CPU and OSPF neighbours
- Send alerts to a webhook
- Write a runbook for an interface-down alert

---

## **1. Monitoring Server Setup**
1. **Install the monitoring system on a Linux VM**
2. **Install Grafana**
3. **Connect the VM to the management network**

## Monitoring Server Setup - Visual Guide

<!-- screenshots -->


## **2. SNMPv3 Discovery**
1. **Configure SNMPv3 on every device**
2. **Add the devices to the monitoring system**
3. **Check that interfaces and sensors appear**

## SNMPv3 Discovery - Visual Guide

<!-- screenshots -->


## **3. Syslog**
1. **Send syslog from every device**
2. **Filter the messages by severity**

## Syslog - Visual Guide

<!-- screenshots -->


## **4. NetFlow**
1. **Export flows from the edge router**
2. **Collect them and view the top talkers**

## NetFlow - Visual Guide

<!-- screenshots -->


## **5. Dashboards**
1. **Add interface utilisation and error graphs**
2. **Add device CPU and memory**
3. **Add the OSPF neighbour count**

## Dashboards - Visual Guide

<!-- screenshots -->


## **6. Alerts and Runbook**
1. **Create alerts for interface down, high utilisation, neighbour change and device unreachable**
2. **Send the alerts to a webhook**
3. **Shut a link and time how long the alert takes**
4. **Write the interface-down runbook**

## Alerts and Runbook - Visual Guide

<!-- screenshots -->


## **Project Outcomes & Key Results**
- **Full Visibility** – Devices, interfaces and flows visible in one place
- **Working Alerts** – A link failure raising an alert
- **Measured Detection** – Time from failure to alert recorded
- **Runbook** – A triage page for the interface-down alert

## **Potential Next Steps**
- **Add alerts for BGP and OSPF changes**
- **Add synthetic checks for DNS and DHCP**
- **Add a status page**

---

This project is part of my **Networking and Infrastructure portfolio**. For any inquiries, reach out via **[LinkedIn](https://www.linkedin.com/in/kimutai-fredrick/)**.

**_Built and documented by Fredrick Kimutai._**
