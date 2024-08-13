# Elastic Stack SIEM Configuration and Management

**Project Overview:**  
This project demonstrates the setup and configuration of an Elastic Stack SIEM in a home lab environment. The goal is to create a functional SIEM system for security event monitoring, analysis, and alerting.

## 🛠️ Technologies Used
- **Elastic Stack (Elasticsearch, Logstash, Kibana)**
- **Kali Linux**
- **Elastic Agents**
- **Nmap**

## 📁 Project Structure
- **configurations/**: Contains configuration files for Elastic Stack and Elastic Agents.
- **scripts/**: Includes scripts used for automation or setup.
- **screenshots/**: Visuals of the SIEM dashboard and alert configurations.
- **README.md**: Project documentation (this file).

---

## 📝 Setup Instructions

### 1. Deploy Elastic Stack

**Install Elasticsearch:**
1. Download Elasticsearch and follow the installation guide.
2. Edit the `elasticsearch.yml` file to configure Elasticsearch.

**Install Kibana:**
1. Download Kibana and follow the installation guide.
2. Edit the `kibana.yml` file to connect Kibana to your Elasticsearch instance.

**Install Logstash:**
1. Download Logstash and follow the installation guide.
2. Configure Logstash to parse and forward logs to Elasticsearch.

### 2. Configure Elastic Agents

**Install Elastic Agents:**
- Install Elastic Agents on the Kali Linux VM.
- Configure the agents to collect logs and forward them to the Elastic Stack.

**Log Collection:**
- Set up log collection by configuring input files for Elastic Agents, focusing on system logs and security-related events.

### 3. Simulate Security Events with Nmap

**Install Nmap on your Kali Linux VM:**
```bash
sudo apt-get install nmap
```
**Run Security Scans:**
- Execute various Nmap scans, such as:
```bash
nmap -sS
```

### 4. Query and Visualize Data Access in Kibana

**Open Kibana:**
- Navigate to the “Discover” section in the Kibana dashboard.

**Create Dashboards:**
- Build custom dashboards to visualize security events and identify patterns.
- Use the saved queries to monitor ongoing activity and detect any anomalies.

### 5. Set Up Alerts

**Create Alert Rules in Kibana:**
- Detect specific security events, like multiple failed login attempts or unauthorized access.
- Configure alerting to send notifications or take action when these events are detected.

**Features:**
- **Custom Dashboard**: Visualize security events in real-time.
- **Alerting System**: Set up alerts for specific security events, enabling proactive incident response.

## Acknowledgments

The steps and instructions provided in this project were inspired by the article [A Simple Elastic SIEM Lab](https://medium.com/@aali23/a-simple-elastic-siem-lab-6765159ee2b2) by Aali, which offers an excellent guide on setting up an Elastic SIEM lab.

