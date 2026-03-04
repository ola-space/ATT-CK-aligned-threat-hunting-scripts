# Threat Intelligence and Threat Hunting Using MITRE ATT&CK, SOCradar and MITRE ATT&CK Navigator


---
## Project overview
This project analyzes overlapping tactics, techniques, and procedures (TTPs) of three advanced threat actors (Volatile Cedar, APT31, and APT41) targeting the Information Services. Using SOCradar, MITRE ATT&CK, and MITRE ATT&CK Navigator, the project identifies high-frequency behaviors and produces a combined overlap layer highlighting shared techniques. Findings demonstrate sector-wide operational patterns, emphasizing stealth, credential theft, and living-off-the-land execution strategies.


---
## Objective
To identify prevalent threat actors and their overlapping techniques in the Information Services sector, providing actionable insight for threat detection and defensive strategies.

---

### Threat Actors Analyzed

The following threat actors targeting the Information Services were selected using SOCradar and analyzed:

- Volatile Cedar
- APT32
- APT41

Each actor was evaluated based on vailability of mapped tactics and techniques within the MITRE ATT&CK.

--- 

## Tools & Resources Used

- SOCradar – Threat actor intelligence collection
- MITRE ATT&CK Framework – Mapping tactics and techniques
- MITRE ATT&CK Navigator – Visualizing overlaps and combined layers
- Microsoft Excel – Documentation and overlap analysis

--- 

## Methodology (MITRE ATT&CK Mapping & Overlap Analysis)

- Threat Actor Identification – Collected documented TTPs for Volatile Cedar, APT31, and APT41 using SOCradar.
- TTP Verification – Mapped techniques to the MITRE ATT&CK framework.
- Navigator Layer Creation – Generated individual actor layers in MITRE ATT&CK Navigator.
- Overlap Analysis – Produced a combined layer highlighting shared techniques.
- Reporting & Documentation – Compiled findings into Excel sheets and visual summaries.

---

## Key Findings

----
### Command and Control (Most Prevalent – Score: 6)

High-Overlap Techniques:

- Ingress Tool Transfer – Score: 6
- Web Service – Score: 5

Actors Observed: **Volatile Cedar, APT31, APT41**

**_Observation:_**   
All actors prioritize stealthy post-compromise communication. The use of web services and standard protocols allows malicious traffic to blend with legitimate network activity.

----

### Discovery (High Overlap – Score: 5)

Common Techniques:

- File and Directory Discovery
- Network Service Discovery
- Network Share Discovery
- Query Registry
- Remote System Discovery
- System Information Discovery
- System Network Information Discovery
- System Owner/User Discovery

**_Observation:_**    
Actors perform structured internal reconnaissance to identify critical systems, privileged accounts, and lateral movement paths.

---

### Execution (Strong Overlap – Score: 4–5)

Key Techniques:

- Command and Scripting Interpreter
- PowerShell
- Windows Command Shell
- Exploitation for Client Execution

**_Observation:_**    
Reliance on Living-off-the-Land binaries and native Windows tooling demonstrates stealth and reduced reliance on custom malware.


---

### Defense Evasion (Medium-High Overlap – Score: 3–5)

Observed Techniques:

- Impersonation
- Process Injection
- Deobfuscate/Decode Files or Information
- Modify Registry
- Indicator Removal
- Masquerading
- Access Token Manipulation

**_Observation:_**    
Actors focus on bypassing endpoint defenses, maintaining persistence, and reducing forensic footprints.


---

### Initial Access (Moderate Overlap – Score: 3–4)

Techniques Identified:

- External Remote Services
- Valid Accounts
- Exploit Public-Facing Applications

**_Observation:_**  
Consistent exploitation of exposed services and credential misuse highlights risks in internet-facing infrastructure.


---

### Credential Access (Highly Prevalent)

Techniques Observed:

- OS Credential Dumping
- Brute Force
- Credential Exploitation

**_Observation:_**   
Credential compromise is a strategic objective, supporting domain-level access and privilege escalation across the sector.

---   

### Overlap Insight

The combined layer demonstrates that although each actor has distinct operational characteristics, several techniques are reused across campaigns. These overlapping techniques represent critical monitoring and detection opportunities for organizations operating within the Information Services sector.


---

## Author
**Olanipekun Babatunde**  
Cybersecurity Analyst







