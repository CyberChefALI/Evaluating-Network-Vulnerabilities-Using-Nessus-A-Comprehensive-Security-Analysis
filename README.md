# Evaluating-Network-Vulnerabilities-Using-Nessus-A-Comprehensive-Security-Analysis

## 🔍 Project Overview

Modern network infrastructures are continuously exposed to evolving cyber threats, misconfigurations, and unpatched software vulnerabilities. Proactive security assessments are critical to identifying and neutralizing these risks before they can be exploited by malicious actors.

This repository documents a comprehensive security analysis and vulnerability assessment performed using Tenable Nessus. The project outlines an end-to-end vulnerability management workflow—from initial environment scoping and scan configuration to severity-based result analysis and actionable remediation planning.

## 🎯 Objectives

•	 Infrastructure Discovery: Deploy and configure Nessus to detect active hosts, open ports, and running services on the target network. 

•	 Vulnerability Identification: Execute targeted scans (both unauthenticated and authenticated) to uncover security gaps, outdated packages, and system misconfigurations. 

•	  Risk Prioritization: Analyze scan output by severity levels (Critical, High, Medium, Low, and Informational) utilizing CVSS scores and CVE references.

•	  Remediation Strategy: Translate raw technical scanner logs into clear, prioritized mitigation steps to harden target assets.

## 🛠️ Tools & Environment

•	Laptop/PC with minimum 4 GB RAM

•	VMware Workstation or VirtualBox

•	Nessus Essentials

•	Kali Linux / Windows

•	Authorized vulnerable target machine

•	Stable network connection

•	Basic networking and cybersecurity knowledge


## STEP-1 Nessus Setup

1.	Launch the Web Interface: Navigate to the Nessus portal in your browser.
   
2.	Authenticate: Sign in using your registered administrator credentials.
   
3.	Run Initial Setup: Complete the system configuration wizard.
   
4.	Compile Signatures: Allow the application to download and initialize its plugin database.
   
5.	Confirm Access: Validate that the main scanner dashboard loads successfully.
    
Outcome: Nessus is fully initialized and operational for vulnerability assessment.

<img width="1920" height="1020" alt="Nessus _ Initializing and 2 more pages - Personal - Microsoft​ Edge 28_09_2026 14_10_31" src="https://github.com/user-attachments/assets/41c89e6c-98b4-482d-ba7e-90bd8fc16978" />


# STEP-2 Configure Target Scan

1.Access the Console: From the Nessus dashboard, navigate to My Scans and initiate a New Scan.

2.Choose Scan Template: Select the Basic Network Scan policy option.

3.Define Parameters: Provide an appropriate project title and specify the target asset by entering the IP address of the Metasploitable 2 virtual machine in the Targets field.

4.Persist Settings: Save the configuration to queue the scan.

Outcome: The vulnerability scan profile is successfully established and primed for execution.

<img width="1920" height="1020" alt="Screenshot 28_09_2026 14_15_14" src="https://github.com/user-attachments/assets/4b6ae1e7-9129-4952-b4e9-0fcf9441b741" />
<img width="1920" height="1020" alt="Nessus Essentials _ Scan Templates - Personal - Microsoft​ Edge 29_09_2026 15_57_28" src="https://github.com/user-attachments/assets/efea9226-1ffa-4045-b6c9-d3034008ab3a" />
<img width="1920" height="1020" alt="meta  Running  - Oracle VirtualBox 29_09_2026 15_10_29" src="https://github.com/user-attachments/assets/3f469113-5b1d-457f-a6d7-8c40ca64ce37" />
<img width="1920" height="991" alt="meta  Running  - Oracle VirtualBox 29_09_2026 14_41_45" src="https://github.com/user-attachments/assets/d0cc5616-ff28-47d9-a9c3-65c80daebb00" />


# Step-3 Run Vulnerability Scan

1.Find and open your pre-set vulnerability scan for Metasploitable .

2.Double-check that the target IP address is accurate.

3.Start the scan by clicking the launch button.

4.Allow the scan to finish running.

5.Review the findings by opening the finished report.
Outcome: The scanner successfully probes Metasploitable 2 and creates a list of discovered vulnerabilities.
