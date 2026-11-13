# DG-INTERNS-WEEK-4


DG Interns Hub – Week 4 README
Name: PREETHI R
Intern ID: DG/15/OCT/CYBER/008
Track: Cyber Security
Week: 4
Topic: SIEM in Practice: Splunk, Wazuh and Log Ingestion
Submission deadline: 15 November 2026, 11:59 PM IST
1. Goal of the week
Ingest endpoint and network logs into a free SIEM, search them, and turn attacker behaviour into alerts.
Topics covered: SIEM architecture, log ingestion with forwarders and agents, basic SPL, Wazuh decoders and rules, alert triage and tuning.
2. Folder structure
DG Interns Hub
└── Week 4
    ├── Notes
    ├── Writeups
    ├── Findings
    ├── Detections
    ├── Cheat Sheet
    ├── PDF Report
    ├── Presentation Report
    └── README
3. Contents and status
Folder / file
What it contains
Status
Notes
Q1 What is a SIEM; Q2 Log ingestion methods; Q3 SPL basics; Q4 Wazuh architecture; Q5 TP/FP/TN/FN, alert fatigue, tuning; Q6 Detection logic T1110; Q7 Correlation, thresholds, baselines, allowlists; Q8 SOC tiers and alert lifecycle (8 separate files)
[Done]
Writeups
TryHackMe: Introduction to SIEM; TryHackMe: Splunk: Exploring SPL (2 separate files)
[Done / In progress]
Findings
Screenshots of all hands-on tasks, attack-to-alert evidence, 3 triage notes
[Done / In progress]
Detections
5 SPL searches and the custom Wazuh rule (ID 100001+)
[Done / In progress]
Cheat Sheet
SPL Command table (15+ entries) and SIEM Alert table (10+ entries)
[Done]
PDF Report
Weekly work report
[Pending]
Presentation Report
Weekly work slides
[Pending]

4. Lab environment
Machine
OS
Role
IP
Splunk server
[Ubuntu / host]
Splunk Enterprise (index: lab)
[fill]
Wazuh server
Ubuntu (dedicated VM)
Wazuh manager, indexer, dashboard
[fill]
Windows VM
[Windows version]
Sysmon, Splunk UF, Wazuh agent
[fill]
Ubuntu VM
[Ubuntu version]
auth.log source, Wazuh agent, attack target
[fill]
Kali VM
Kali Linux
Attacker (Hydra, Nmap)
[fill]

Note: write which SIEM you built fully if your hardware was limited (see the hardware note in the task).
5. Hands-on summary
Task
What was done
Evidence
1. Install Splunk
Installed Splunk Enterprise and created the lab index
Findings: login page, empty index
2. Ingest logs into Splunk
Universal Forwarder on Windows (Security and Sysmon) and auth.log on Ubuntu
Findings: forwarder config, search on index=lab, Sysmon and auth.log events
3. Install Wazuh
Quickstart install, two agents enrolled, FIM on a test folder
Findings: dashboard, agents, FIM alert
4. Attack to alert
Hydra SSH brute force and Nmap -sS scan found in the SIEM
Findings: raw event, parsed fields, alert
5. Detections
5 SPL searches, 2 scheduled alerts, 4-panel dashboard, 1 custom Wazuh rule tested with wazuh-logtest
Detections folder and Findings screenshots
6. Triage notes
3 alerts triaged with who, what, when, where, why, verdict and next step
Findings: triage notes
7. Cheat sheets
SPL command table and SIEM alert table
Cheat Sheet folder

6. Ingestion flow
Log source → Forwarder / Agent → Indexer / Manager → Search head / Dashboard
7. Key learnings
[Write 3 to 5 points in your own words, for example how a forwarder differs from a Wazuh agent.]
[What you learned about tuning false positives.]
[What you would improve next time.]
9. LinkedIn activity
P


https://lnkd.in/p/g8mpiyqq


https://lnkd.in/p/gbXPuATB
[paste link]

10. Tools used
Splunk Enterprise (free licence), Splunk Universal Forwarder, Splunk Add-on for Sysmon, Sysmon, Wazuh, Kali Linux, Hydra, Nmap, VirtualBox / VMware, TryHackMe.
11. Declaration
All notes are written in my own words, all screenshots are from my own lab, and only free tools were used.
PREETHI R – DG/15/OCT/CYBER/008
