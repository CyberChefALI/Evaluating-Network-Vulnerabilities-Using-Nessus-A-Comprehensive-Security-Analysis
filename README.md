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
<img width="1920" height="1020" alt="Nessus Essentials _ Folders _ View Scan - Personal - Microsoft​ Edge 30_09_2026 19_45_23" src="https://github.com/user-attachments/assets/14c92616-4d52-4c0d-8702-0eb768341ea6" />



# Step-3 Run Vulnerability Scan

1.Find and open your pre-set vulnerability scan for Metasploitable/Windows .

2.Double-check that the target IP address is accurate.

3.Start the scan by clicking the launch button.

4.Allow the scan to finish running.

5.Review the findings by opening the finished report.
Outcome: The scanner successfully probes Metasploitable & Windows and creates a list of discovered vulnerabilities.
<img width="1920" height="1020" alt="Nessus Essentials _ Folders _ View Scan - Personal - Microsoft​ Edge 30_09_2026 19_45_23" src="https://github.com/user-attachments/assets/d1002ced-81e9-4b5f-a4e9-31d8c5a73e8f" /> 


# Step-4 Categorize the security risks (based on how dangerous or critical they are)

Severity	Color	Description
🟥 Critical	Red	          Very serious vulnerability
🟧 High	Orange	          Serious vulnerability
🟨 Medium	Yellow        	 Moderate risk
🟦 Low	Blue	             Low risk
⬜ Info	White/Grey	       Informational finding

1.Review the finished scan report by heading over to the Vulnerabilities tab.

2.Evaluate how serious every discovered security flaw is.

3.Prioritize the most dangerous issues, focusing on Critical and High ratings right away.

4.Document key information for each finding, including its name, risk level, impacted port or service, and specific details.

Outcome: Vulnerabilities are grouped by their threat level, highlighting the high-priority findings for deeper investigation.
<img width="1920" height="1020" alt="Nessus Essentials _ Folders _ View Scan - Personal - Microsoft​ Edge 30_09_2026 19_55_15" src="https://github.com/user-attachments/assets/4edac479-1ee9-4b8a-a5e4-8139e1ae45bb" />
<img width="1920" height="1020" alt="Nessus Essentials _ Folders _ View Scan - Personal - Microsoft​ Edge 30_09_2026 19_43_28" src="https://github.com/user-attachments/assets/c81bc705-95fc-42f6-bf04-5b0266725a0f" />


# Step-5 Investigate the critical threats found during the scan

1.Navigate to the Vulnerabilities tab inside your Nessus report.

2.Filter the results to show only the Critical severity issues.

3.There is no severe Vulnerabilities found .

4.Record the following details:(if vulnerabilities found)

Vulnerability Name
Severity
CVE ID (if available)
Affected Port & Service
Description
Security Impact
Solution/Recommendation

5.Capture screenshots of the relevant Nessus findings for documentation.
Outcome: The critical security flaws are successfully spotted, and their information is gathered to document and review further.

<img width="1920" height="1020" alt="Nessus Essentials _ Folders _ View Scan - Personal - Microsoft​ Edge 30_09_2026 20_20_26" src="https://github.com/user-attachments/assets/5fd4fb35-8be1-4c69-9a7d-391dea760fca" />
<img width="1920" height="1020" alt="Nessus Essentials _ Folders _ View Scan - Personal - Microsoft​ Edge 30_09_2026 20_20_10" src="https://github.com/user-attachments/assets/fcc67f77-b1cd-44b8-8711-be96d89105ab" /> 

# Step-6 Review Informational Findings

1.Navigate to the Vulnerabilities tab in Nessus and apply the "Info" severity filter.

2.Go through the 131 informational items discovered on the target machine.

3.Examine the specifics of the findings that matter to your assessment.

4.Log key reconnaissance data, such as active ports, running services, and system configurations.

5.Take screenshots to use as proof or documentation.
outcome:The informational findings are reviewed and useful system and service information is recorded.

<img width="1920" height="1020" alt="Nessus Essentials _ Folders _ View Scan - Personal - Microsoft​ Edge 30_09_2026 20_20_26" src="https://github.com/user-attachments/assets/0caf2f1c-f0d6-4da3-8c72-9b61928280af" /> 

# Step-7 Recording Vulnerabilities and Evaluating Threats

1.Review the vulnerabilities identified(if found)

2.Select the important Critical, High, and Medium vulnerabilities for detailed documentation.

3.For each vulnerability, record:

Vulnerability Name
Severity
CVE ID (if available)
Affected Port & Service
Description
Security Impact
Recommendation
Evidence/Screenshot
4.Organize the findings according to their severity.

5.Prepare a summary of the identified vulnerabilities and their risks.

outcome: The identified vulnerabilities(if found) are properly documented and their security risks are analyzed

# Step-8 Corrective Actions and Risk Control

1.Examine the security fixes suggested by Nessus.

2.Focus first on the most dangerous issues, targeting Critical and High severity flaws.

3.Implement proper security measures within your windows test lab.

4.Adjust or patch vulnerable services wherever necessary.

5.Confirm that your updates and changes took effect and were completed properly.




