# NICE Framework crosswalk (AICWRF v0.1 draft)

Alignment of course modules to NICE Framework Components v2.2.0 (NIST SP 800-181 Rev. 1) work roles, task statements and the AI Security competency area. Task and statement text is quoted from the official NICE data file (https://csrc.nist.gov/csrc/media/Projects/cprt/documents/nice/v2-2-0_nf_components.json); every task ID was checked against its work role.

**Reading this document**
- This is the author's alignment, not an official NICE, NIST or DoD mapping, and no endorsement is implied.
- Numbers such as 541 are OPM codes that NICE lists beside each role. DCWF codes below are name matches from a March 2026 DoD slide deck, not a confirmed mapping.
- AI-integration items attach to NICE competency area NF-COM-002 (AI Security), not to the work roles. "Aligned to the competency area" is the only claim.
- The "Fit" column is the author's judgment of whether a lab or assignment exercises each task; it is still to be completed. No job-readiness, DoD 8140 qualification or accreditation is claimed.
- CIS 214, 280 and 282 are planned redesigns, not yet taught in this form.

# DCWF lookup (2026-11-26)

Source actually read: DoW CIO "DoD 8140 Deep Dive" slide deck, March 2026, DCWF chart "current as of January 28, 2026" (https://www.afcea.org/sites/default/files/2026-04/Tuesday_1615_CWS-Summit_8140DeepDive_FINAL_V2.pdf). cyber.mil, dodcio.defense.gov and the DoDM 8140.03 PDF blocked automated fetches, and no published NICE v2.2.0 to DCWF crosswalk was found. Pairings below are by name and function only, so they are **candidate matches, not a confirmed mapping**. For these roles the DCWF code equals the OPM code NICE lists.

| NICE v2.2.0 role | DCWF code and title as shown in the slide | Confidence |
|---|---|---|
| PD-WRL-007 Vulnerability Analysis | 541 Vulnerability Assessment Analyst | name match |
| DD-WRL-005 Software Security Assessment | 622 Secure Software Assessor | name match |
| DD-WRL-003 Secure Software Development | 621 Software Developer | name match |
| IO-WRL-007 Technical Support | 411 Technical Support Specialist | name match |
| IO-WRL-005 Systems Administration | 451 System Administrator | name match |
| PD-WRL-001 Defensive Cybersecurity | 511 Cyber Defense Analyst | name match |
| PD-WRL-003 Incident Response | 531 Cyber Defense Incident Responder | name match |
| IO-WRL-006 Systems Security Analysis | 461 Systems Security Analyst | name match |
| IO-WRL-004 Network Operations | 441 Network Operations Specialist | name match |
| PD-WRL-002 Digital Forensics | 212 Cyber Defense Forensics Analyst | name match |
| IN-WRL-002 Digital Evidence Analysis | 211 Forensics Analyst | name match |
| OG-WRL-004 Cybersecurity Curriculum Development | 711 Cyber Instructional Curriculum Developer | name match |
| OG-WRL-005 Cybersecurity Instruction | 712 Cyber Instructor | name match |
| DD-WRL-009 OT Cybersecurity Engineering | not found (462 Control Systems Security Specialist is the nearest title; unconfirmed) | not found |

These should be confirmed on an official DoD page (DCWF Work Role Tool or the DoDM 8140.03 appendix). This crosswalk is the author's alignment, not a DoD mapping.

# Crosswalk

## CIS 246 Ethical Hacking (module M4)

Live Lab password cracking, scanning, penetration-test reporting. AI module: verify AI claims in a vulnerability write-up.

**Primary work role:** PD-WRL-007 Vulnerability Analysis (OPM 541)

| Task ID | Official task statement | Fit |
|---|---|---|
| T1091 | Perform authorized penetration testing on enterprise network assets | to be assessed by author |
| T1118 | Identify vulnerabilities | to be assessed by author |
| T1119 | Recommend vulnerability remediation strategies | to be assessed by author |
| T1619 | Perform risk and vulnerability assessments | to be assessed by author |
| T1279 | Prepare audit reports | to be assessed by author |
| T1084 | Identify anomalous network activity | to be assessed by author |

**Secondary work role:** DD-WRL-005 Software Security Assessment (OPM 622)

| Task ID | Official task statement | Fit |
|---|---|---|
| T1359 | Perform penetration testing | to be assessed by author |

**AI-integration items (official NICE v2.2.0 text):**

| ID | Type | Statement | In AI Security competency area NF-COM-002 | Linked to the primary role |
|---|---|---|---|---|
| K1320 | knowledge | Knowledge of common AI security risks | yes | no |
| S0957 | skill | Skill in identifying possible mistakes or hallucinations in AI-generated outputs | yes | no |
| S0953 | skill | Skill in developing prompts for generative AI systems | yes | no |
| K1324 | knowledge | Knowledge of data poisoning cyberattacks | yes | no |
| K1333 | knowledge | Knowledge of misinformation and disinformation vulnerabilities in AI systems | yes | no |

## CIS 251 C++ Programming (module M5)

Debugging (linked-list segfault lab), secure coding component. AI module: verify AI-written code against tests.

**Primary work role:** DD-WRL-003 Secure Software Development (OPM 621)

| Task ID | Official task statement | Fit |
|---|---|---|
| T0077 | Develop secure code and error handling | to be assessed by author |
| T1197 | Identify common coding flaws | to be assessed by author |
| T1262 | Identify programming code flaws | to be assessed by author |
| T1261 | Mitigate programming vulnerabilities | to be assessed by author |
| T1073 | Perform code reviews | to be assessed by author |
| T1116 | Correct program errors | to be assessed by author |
| T1074 | Prepare secure code documentation | to be assessed by author |

**Secondary work role:** DD-WRL-005 Software Security Assessment (OPM 622)

| Task ID | Official task statement | Fit |
|---|---|---|
| T1590 | Identify programming flaws | to be assessed by author |

**AI-integration items (official NICE v2.2.0 text):**

| ID | Type | Statement | In AI Security competency area NF-COM-002 | Linked to the primary role |
|---|---|---|---|---|
| S0957 | skill | Skill in identifying possible mistakes or hallucinations in AI-generated outputs | yes | no |
| K1319 | knowledge | Knowledge of code review processes | yes | no |
| K0814 | knowledge | Knowledge of secure coding tools and techniques | yes | yes |
| K1117 | knowledge | Knowledge of coding and testing standards | yes | yes |
| S0953 | skill | Skill in developing prompts for generative AI systems | yes | no |

## CIS 268 Software Support (module M6)

DHCP and CLI troubleshooting, support runbooks. AI module: AI-drafted runbook, verified and corrected.

**Primary work role:** IO-WRL-007 Technical Support (OPM 411)

| Task ID | Official task statement | Fit |
|---|---|---|
| T0237 | Troubleshoot system hardware and software | to be assessed by author |
| T1538 | Resolve customer-reported system incidents and events | to be assessed by author |
| T1567 | Configure system hardware, software, and peripheral equipment | to be assessed by author |
| T1569 | Administer system and network user accounts | to be assessed by author |
| T1427 | Maintain incident tracking and solution databases | to be assessed by author |
| T1334 | Produce cybersecurity instructional materials | to be assessed by author |
| T1566 | Install system hardware, software, and peripheral equipment | to be assessed by author |

**AI-integration items (official NICE v2.2.0 text):**

| ID | Type | Statement | In AI Security competency area NF-COM-002 | Linked to the primary role |
|---|---|---|---|---|
| S0957 | skill | Skill in identifying possible mistakes or hallucinations in AI-generated outputs | yes | no |
| S0953 | skill | Skill in developing prompts for generative AI systems | yes | no |
| S0391 | skill | Skill in creating technical documentation | yes | no |
| S0385 | skill | Skill in communicating complex concepts | yes | no |

## CIS 214 Security Analysis (Spring 2027 redesign, planning document) (module M3)

Shared SOC monitoring of the CIS 280 network; CySA+ target (CS0-004). The planned AI-verification lesson sits here. Planned, not yet taught in this form.

**Primary work role:** PD-WRL-001 Defensive Cybersecurity (OPM 511)

| Task ID | Official task statement | Fit |
|---|---|---|
| T1084 | Identify anomalous network activity | to be assessed by author |
| T1112 | Validate network alerts | to be assessed by author |
| T1299 | Determine causes of network alerts | to be assessed by author |
| T1348 | Distinguish between benign and potentially malicious cybersecurity attacks and intrusions | to be assessed by author |
| T1350 | Perform continuous monitoring of system activity | to be assessed by author |
| T1387 | Validate intrusion detection system alerts | to be assessed by author |
| T1241 | Document cybersecurity incidents | to be assessed by author |
| T1242 | Escalate incidents that may cause ongoing and immediate impact to the environment | to be assessed by author |
| T1290 | Communicate daily network event and activity reports | to be assessed by author |

**Secondary work role:** PD-WRL-003 Incident Response (OPM 531)

| Task ID | Official task statement | Fit |
|---|---|---|
| T1250 | Perform cyber defense incident triage | to be assessed by author |
| T1332 | Produce incident findings reports | to be assessed by author |

**AI-integration items (official NICE v2.2.0 text):**

| ID | Type | Statement | In AI Security competency area NF-COM-002 | Linked to the primary role |
|---|---|---|---|---|
| S0957 | skill | Skill in identifying possible mistakes or hallucinations in AI-generated outputs | yes | no |
| K1321 | knowledge | Knowledge of common business and cybersecurity applications of AI systems | yes | no |
| K1320 | knowledge | Knowledge of common AI security risks | yes | no |
| S0900 | skill | Skill in analyzing information from multiple sources | yes | no |

## CIS 280 Network Security (Spring 2027 redesign, planning document) (module M8)

Progressive hardening of a shared class network; Security+ target. Planned redesign. OT/IoT (M11) is undecided: if included, add DD-WRL-009 Operational Technology (OT) Cybersecurity Engineering and competency area NF-COM-010.

**Primary work role:** IO-WRL-006 Systems Security Analysis (OPM 461)

| Task ID | Official task statement | Fit |
|---|---|---|
| T1212 | Implement cybersecurity countermeasures for systems and applications | to be assessed by author |
| T1563 | Implement system security measures | to be assessed by author |
| T1559 | Resolve vulnerabilities in systems and system components | to be assessed by author |
| T1548 | Determine adequacy of access controls | to be assessed by author |
| T1263 | Perform security reviews | to be assessed by author |

**Secondary work role:** IO-WRL-004 Network Operations (OPM 441)

| Task ID | Official task statement | Fit |
|---|---|---|
| T0081 | Diagnose network connectivity problems | to be assessed by author |
| T1050 | Improve network security practices | to be assessed by author |
| T1100 | Configure network hubs, routers, and switches | to be assessed by author |
| T1248 | Patch network vulnerabilities | to be assessed by author |
| T1313 | Test network infrastructure, including software and hardware devices | to be assessed by author |

**AI-integration items (official NICE v2.2.0 text):**

| ID | Type | Statement | In AI Security competency area NF-COM-002 | Linked to the primary role |
|---|---|---|---|---|
| K1320 | knowledge | Knowledge of common AI security risks | yes | no |
| K1321 | knowledge | Knowledge of common business and cybersecurity applications of AI systems | yes | no |
| S0957 | skill | Skill in identifying possible mistakes or hallucinations in AI-generated outputs | yes | no |

## CIS 282 Computer Forensics (Spring 2027 redesign, planning document) (module M9)

Evidence imaging and Autopsy/AXIOM analysis; certification MCFE (recommended) or CHFI. Planned redesign.

**Primary work role:** PD-WRL-002 Digital Forensics (OPM 212)

| Task ID | Official task statement | Fit |
|---|---|---|
| T1120 | Create forensically sound duplicates of evidence | to be assessed by author |
| T1199 | Identify digital evidence for analysis | to be assessed by author |
| T1324 | Process digital evidence | to be assessed by author |
| T1325 | Document digital evidence | to be assessed by author |
| T1486 | Process forensic images | to be assessed by author |
| T0173 | Perform timeline analysis | to be assessed by author |
| T1510 | Preserve digital evidence | to be assessed by author |
| T1607 | Recover information from forensic data sources | to be assessed by author |
| T1383 | Utilize deployable forensics toolkit | to be assessed by author |
| T1159 | Create technical summary of findings reports | to be assessed by author |
| T1175 | Determine if digital media chain or custody processes meet Federal Rules of Evidence requirements | to be assessed by author |

**Secondary work role:** IN-WRL-002 Digital Evidence Analysis (OPM 211)

| Task ID | Official task statement | Fit |
|---|---|---|
| T1542 | Document original condition of digital evidence | to be assessed by author |
| T1256 | Perform forensically sound image collection | to be assessed by author |

**AI-integration items (official NICE v2.2.0 text):**

| ID | Type | Statement | In AI Security competency area NF-COM-002 | Linked to the primary role |
|---|---|---|---|---|
| S0957 | skill | Skill in identifying possible mistakes or hallucinations in AI-generated outputs | yes | no |
| K1320 | knowledge | Knowledge of common AI security risks | yes | no |
| S0900 | skill | Skill in analyzing information from multiple sources | yes | no |

## CIS 269 Hardware and Systems Support (module M7, taught)

A+ target. Hardware and OS support labs.

**Primary work role:** IO-WRL-007 Technical Support (OPM 411)

| Task ID | Official task statement | Fit |
|---|---|---|
| T0237 | Troubleshoot system hardware and software | to be assessed by author |
| T1566 | Install system hardware, software, and peripheral equipment | to be assessed by author |
| T1567 | Configure system hardware, software, and peripheral equipment | to be assessed by author |
| T1538 | Resolve customer-reported system incidents and events | to be assessed by author |
| T1572 | Inventory technology resources | to be assessed by author |
| T1580 | Monitor client-level computer system performance | to be assessed by author |

**Secondary work role:** IO-WRL-005 Systems Administration (OPM 451)

| Task ID | Official task statement | Fit |
|---|---|---|
| T0531 | Troubleshoot hardware/software interface and interoperability problems | to be assessed by author |
| T0431 | Check system hardware availability, functionality, integrity, and efficiency | to be assessed by author |
| T1500 | Install systems and servers | to be assessed by author |
| T1502 | Troubleshoot systems and servers | to be assessed by author |
| T1588 | Diagnose faulty system and server hardware | to be assessed by author |
| T1589 | Repair faulty system and server hardware | to be assessed by author |

**AI-integration items:**

| ID | Type | Statement | In AI Security area NF-COM-002 | Work roles carrying it |
|---|---|---|---|---|
| S0957 | skill | Skill in identifying possible mistakes or hallucinations in AI-generated outputs | yes | none |
| S0953 | skill | Skill in developing prompts for generative AI systems | yes | none |
| S0391 | skill | Skill in creating technical documentation | yes | OG-WRL-012, OG-WRL-005, OG-WRL-004, PD-WRL-005, DD-WRL-009, DD-WRL-008 (+1 more) |

## CIS 146 and CIS 149 Digital Literacy and IC3 (module M1, taught; Track A)

General-education courses. **No work-role claim is made.** They teach digital literacy, not a cybersecurity occupation. The only honest alignment is to the AI Security competency area, and the items below are in no work role at all in NICE v2.2.0.

**Items (official NICE v2.2.0 text):**

| ID | Type | Statement | In AI Security area NF-COM-002 | Work roles carrying it |
|---|---|---|---|---|
| K0660 | knowledge | Knowledge of appropriate use policies and procedures | yes | none |
| K1327 | knowledge | Knowledge of ethical responsibilities of AI system users and providers | yes | none |
| K1337 | knowledge | Knowledge of responsible use principles and practices | yes | none |
| S0957 | skill | Skill in identifying possible mistakes or hallucinations in AI-generated outputs | yes | none |
| K1333 | knowledge | Knowledge of misinformation and disinformation vulnerabilities in AI systems | yes | none |

## CIS 211 Information Assurance Basics (module M2, taught)

Foundations course. **No single work role fits.** The statements below are foundation knowledge that many roles share (see last column). Use them as prerequisite knowledge in the framework, not as a role alignment.

**Items (official NICE v2.2.0 text):**

| ID | Type | Statement | In AI Security area NF-COM-002 | Work roles carrying it |
|---|---|---|---|---|
| K0728 | knowledge | Knowledge of Confidentiality, Integrity and Availability (CIA) principles and practices | yes | OG-WRL-011, OG-WRL-012, OG-WRL-013, OG-WRL-010, OG-WRL-007, OG-WRL-009 (+14 more) |
| K0742 | knowledge | Knowledge of identity and access management (IAM) principles and practices | yes | OG-WRL-012, IO-WRL-001, IO-WRL-006, PD-WRL-001, IO-WRL-002, PD-WRL-007 (+4 more) |
| K0735 | knowledge | Knowledge of risk management models and frameworks | yes | OG-WRL-017, OG-WRL-014, OG-WRL-016, OG-WRL-015, OG-WRL-011, OG-WRL-012 (+8 more) |
| K0835 | knowledge | Knowledge of risk assessment principles and practices | yes | OG-WRL-016, OG-WRL-015, OG-WRL-011, OG-WRL-010, OG-WRL-009, DD-WRL-001 (+2 more) |

## Educator row: the framework itself (not a course)

These describe the author's own work as framework author, mapped to the Cybersecurity Instruction and Curriculum Development roles. They are not a course alignment.

**Primary work role:** OG-WRL-004 Cybersecurity Curriculum Development (OPM 711)

| Task ID | Official task statement | Fit |
|---|---|---|
| T1463 | Develop cybersecurity curriculum goals and objectives | to be assessed by author |
| T1475 | Develop instructional strategies | to be assessed by author |
| T1451 | Create interactive learning exercises | to be assessed by author |
| T1608 | Perform periodic reviews of learning materials and courses for accuracy and currency | to be assessed by author |
| T1438 | Determine effectiveness of instruction and training | to be assessed by author |
| T1446 | Conduct learning needs assessments | to be assessed by author |

**Secondary work role:** OG-WRL-005 Cybersecurity Instruction (OPM 712)

| Task ID | Official task statement | Fit |
|---|---|---|
| T1413 | Develop training modules and classes | to be assessed by author |
| T1414 | Develop training assignments | to be assessed by author |
| T1415 | Develop training evaluations | to be assessed by author |
| T1416 | Develop grading and proficiency standards | to be assessed by author |
| T1418 | Develop learning objectives and goals | to be assessed by author |
| T1421 | Develop proficiency assessments | to be assessed by author |
| T1537 | Determine if cybersecurity training, education, and awareness meet established goals | to be assessed by author |
| T1609 | Recommend revisions to learning materials and curriculum | to be assessed by author |

## M10 AI security (new content, Track B; to be written)

Seeded from the CIS 214 and 280 redesigns and the AI module. **No work role claim is possible.** In NICE v2.2.0 none of the AI-security knowledge or skill statements below is linked to any work role (the one exception, K0904, is carried only by Data Analysis, IO-WRL-001). The alignment is to competency area NF-COM-002 only. NICE v2.2.0 defines no dedicated AI work role.

| ID | Type | Statement | Work roles carrying it | Fit |
|---|---|---|---|---|
| K1320 | knowledge | Knowledge of common AI security risks | none | to be assessed by author |
| K1324 | knowledge | Knowledge of data poisoning cyberattacks | none | to be assessed by author |
| K1333 | knowledge | Knowledge of misinformation and disinformation vulnerabilities in AI systems | none | to be assessed by author |
| K1334 | knowledge | Knowledge of NIST AI Risk Management Framework | none | to be assessed by author |
| K1341 | knowledge | Knowledge of test, evaluation, verification, and validation (TEVV) processes | none | to be assessed by author |
| K1342 | knowledge | Knowledge of training, validation, and test data sets | none | to be assessed by author |
| K1345 | knowledge | Knowledge of agentic AI principles and practices | none | to be assessed by author |
| S0955 | skill | Skill in evaluating machine learning models | none | to be assessed by author |
| S0956 | skill | Skill in evaluating the performance of algorithms | none | to be assessed by author |
| S0957 | skill | Skill in identifying possible mistakes or hallucinations in AI-generated outputs | none | to be assessed by author |
| S0953 | skill | Skill in developing prompts for generative AI systems | none | to be assessed by author |
| K0904 | knowledge | Knowledge of machine learning principles and practices | IO-WRL-001 | to be assessed by author |

## M11 OT/IoT (new content, to be written)

**Work role:** DD-WRL-009 Operational Technology (OT) Cybersecurity Engineering (OPM none). NICE v2.2.0 also lists competency area NF-COM-010 Operational Technology (OT) Security, but the file links **no items** to it, so no K/S statement can be cited for it. Simulation-testbed OT/IoT work by the author exists as unsubmitted drafts and is not cited here as evidence of adoption or outcomes. Module content is to be written.

| Task ID | Official task statement | Fit |
|---|---|---|
| T2047 | Inventory OT assets | to be assessed by author |
| T2028 | Develop OT inventory model for cybersecurity  | to be assessed by author |
| T2031 | Identify gaps in OT network architecture | to be assessed by author |
| T2045 | Assign networked engineering assets to security zones | to be assessed by author |
| T2032 | Assign security level targets to network zones for control systems | to be assessed by author |
| T2034 | Design cybersecurity tools for OT systems | to be assessed by author |
| T2037 | Create cybersecurity inspection and test policies and procedures for OT systems | to be assessed by author |
| T2042 | Generate cyberattack scenarios of serious physical consequence | to be assessed by author |
| T1619 | Perform risk and vulnerability assessments | to be assessed by author |
| T2051 | Train cybersecurity defense technicians on OT system processes and procedures | to be assessed by author |

