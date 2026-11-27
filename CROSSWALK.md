# NICE Framework crosswalk (AICWRF v0.2)

Alignment of course modules to NICE Framework Components v2.2.0 (NIST SP 800-181 Rev. 1) work roles, task statements and the AI Security competency area. Task and statement text is quoted from the official NICE data file (https://csrc.nist.gov/csrc/media/Projects/cprt/documents/nice/v2-2-0_nf_components.json); every task ID was checked against its work role.

**Reading this document**
- This is the author's alignment, not an official NICE, NIST or DoD mapping, and no endorsement is implied.
- Numbers such as 541 are OPM codes that NICE lists beside each role. DCWF codes below are name matches from a March 2026 DoD slide deck, not a confirmed mapping.
- AI-integration items attach to NICE competency area NF-COM-002 (AI Security), not to the work roles. "Aligned to the competency area" is the only claim.
- The "Fit" column is the author's judgment of whether a lab or assignment exercises each task; entries are the author's statements about their own courses (v0.2) and have not been independently verified; Strong = students do the task and it is graded, Partial = a simulated or smaller version, Planned = not yet taught. No job-readiness, DoD 8140 qualification or accreditation is claimed.
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
| T1091 | Perform authorized penetration testing on enterprise network assets | Partial: attacks run in lab environments, not on enterprise assets |
| T1118 | Identify vulnerabilities | Strong: graded Live Labs include network reconnaissance, Nmap NSE, SQLMap, Netcat vulnerability discovery and evaluating end-of-life software |
| T1119 | Recommend vulnerability remediation strategies | Partial: remediation is part of the AI-assisted pentest write-up and the EOL software lab |
| T1619 | Perform risk and vulnerability assessments | Partial: risk and vulnerability evaluation inside graded labs; no stand-alone assessment assignment |
| T1279 | Prepare audit reports | Partial: AI-assisted pentest reporting assignment (rubric-graded); not a formal audit report |
| T1084 | Identify anomalous network activity | Partial: network traffic sniffing lab; detection and log review are described by the author but are not a separate graded item |

**Secondary work role:** DD-WRL-005 Software Security Assessment (OPM 622)

| Task ID | Official task statement | Fit |
|---|---|---|
| T1359 | Perform penetration testing | Strong: graded Live Labs cover exploitation, privilege escalation, lateral movement, post-exploitation (lab environment) |

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
| T0077 | Develop secure code and error handling | Partial: described by the author as taught; not visible as a separate graded item |
| T1197 | Identify common coding flaws | Partial: described by the author as taught; not visible as a separate graded item |
| T1262 | Identify programming code flaws | Strong: students find code flaws in their own programs (exemplar) |
| T1261 | Mitigate programming vulnerabilities | Partial: described by the author as taught; not visible as a separate graded item |
| T1073 | Perform code reviews | Partial: students verify AI-written code by compiling and running it (rubric item); no separate code-review assignment |
| T1116 | Correct program errors | Strong: students diagnose and fix program errors (exemplar: linked-list segfault) |
| T1074 | Prepare secure code documentation | Not covered as secure-code documentation: assignments use script tools, and AI is used to help students understand code (author-stated) |

**Secondary work role:** DD-WRL-005 Software Security Assessment (OPM 622)

| Task ID | Official task statement | Fit |
|---|---|---|
| T1590 | Identify programming flaws | Strong: students identify programming flaws (exemplar) |

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
| T0237 | Troubleshoot system hardware and software | Strong: CLI Troubleshooting Lab (rubric-graded) |
| T1538 | Resolve customer-reported system incidents and events | Strong: simulated tickets from the CLI Troubleshooting Lab, written up as a helpdesk portfolio (capstone Track A, rubric-graded) |
| T1567 | Configure system hardware, software, and peripheral equipment | Partial: CLI troubleshooting lab; capstone track writes a PowerShell or Bash script for a support task |
| T1569 | Administer system and network user accounts | Partial: described by the author (Active Directory server work); not visible as a separate graded item |
| T1427 | Maintain incident tracking and solution databases | Partial: ticket write-ups in the helpdesk portfolio; no maintained tracking database |
| T1334 | Produce cybersecurity instructional materials | Partial: students write support runbooks, which are instructional documents |
| T1566 | Install system hardware, software, and peripheral equipment | Strong: Week 2 lab installing Windows from a bootable USB |

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
| T1084 | Identify anomalous network activity | Planned (Spring 2027), not yet taught |
| T1112 | Validate network alerts | Planned (Spring 2027), not yet taught |
| T1299 | Determine causes of network alerts | Planned (Spring 2027), not yet taught |
| T1348 | Distinguish between benign and potentially malicious cybersecurity attacks and intrusions | Planned (Spring 2027), not yet taught |
| T1350 | Perform continuous monitoring of system activity | Planned (Spring 2027), not yet taught |
| T1387 | Validate intrusion detection system alerts | Planned (Spring 2027), not yet taught |
| T1241 | Document cybersecurity incidents | Planned (Spring 2027), not yet taught |
| T1242 | Escalate incidents that may cause ongoing and immediate impact to the environment | Planned (Spring 2027), not yet taught |
| T1290 | Communicate daily network event and activity reports | Planned (Spring 2027), not yet taught |

**Secondary work role:** PD-WRL-003 Incident Response (OPM 531)

| Task ID | Official task statement | Fit |
|---|---|---|
| T1250 | Perform cyber defense incident triage | Planned (Spring 2027), not yet taught |
| T1332 | Produce incident findings reports | Planned (Spring 2027), not yet taught |

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
| T1212 | Implement cybersecurity countermeasures for systems and applications | Planned (Spring 2027), not yet taught |
| T1563 | Implement system security measures | Planned (Spring 2027), not yet taught |
| T1559 | Resolve vulnerabilities in systems and system components | Planned (Spring 2027), not yet taught |
| T1548 | Determine adequacy of access controls | Planned (Spring 2027), not yet taught |
| T1263 | Perform security reviews | Planned (Spring 2027), not yet taught |

**Secondary work role:** IO-WRL-004 Network Operations (OPM 441)

| Task ID | Official task statement | Fit |
|---|---|---|
| T0081 | Diagnose network connectivity problems | Planned (Spring 2027), not yet taught |
| T1050 | Improve network security practices | Planned (Spring 2027), not yet taught |
| T1100 | Configure network hubs, routers, and switches | Planned (Spring 2027), not yet taught |
| T1248 | Patch network vulnerabilities | Planned (Spring 2027), not yet taught |
| T1313 | Test network infrastructure, including software and hardware devices | Planned (Spring 2027), not yet taught |

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
| T1120 | Create forensically sound duplicates of evidence | Planned (Spring 2027), not yet taught |
| T1199 | Identify digital evidence for analysis | Planned (Spring 2027), not yet taught |
| T1324 | Process digital evidence | Planned (Spring 2027), not yet taught |
| T1325 | Document digital evidence | Planned (Spring 2027), not yet taught |
| T1486 | Process forensic images | Planned (Spring 2027), not yet taught |
| T0173 | Perform timeline analysis | Planned (Spring 2027), not yet taught |
| T1510 | Preserve digital evidence | Planned (Spring 2027), not yet taught |
| T1607 | Recover information from forensic data sources | Planned (Spring 2027), not yet taught |
| T1383 | Utilize deployable forensics toolkit | Planned (Spring 2027), not yet taught |
| T1159 | Create technical summary of findings reports | Planned (Spring 2027), not yet taught |
| T1175 | Determine if digital media chain or custody processes meet Federal Rules of Evidence requirements | Planned (Spring 2027), not yet taught |

**Secondary work role:** IN-WRL-002 Digital Evidence Analysis (OPM 211)

| Task ID | Official task statement | Fit |
|---|---|---|
| T1542 | Document original condition of digital evidence | Planned (Spring 2027), not yet taught |
| T1256 | Perform forensically sound image collection | Planned (Spring 2027), not yet taught |

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
| T0237 | Troubleshoot system hardware and software | Strong: hands-on hardware and software troubleshooting (author-stated) |
| T1566 | Install system hardware, software, and peripheral equipment | Strong: students install hardware, software and peripherals (author-stated) |
| T1567 | Configure system hardware, software, and peripheral equipment | Strong: students configure systems and peripherals (author-stated) |
| T1538 | Resolve customer-reported system incidents and events | Strong: help-desk-style incident work (author-stated) |
| T1572 | Inventory technology resources | Strong: students inventory hardware and software (author-stated) |
| T1580 | Monitor client-level computer system performance | Strong: students monitor performance with system tools (author-stated) |

**Secondary work role:** IO-WRL-005 Systems Administration (OPM 451)

| Task ID | Official task statement | Fit |
|---|---|---|
| T0531 | Troubleshoot hardware/software interface and interoperability problems | Strong: hardware and software interface problems are troubleshot in the labs (author-stated) |
| T0431 | Check system hardware availability, functionality, integrity, and efficiency | Partial: availability and efficiency checks come through performance monitoring; formal integrity checks not confirmed |
| T1500 | Install systems and servers | Partial: operating-system installs are done; server-specific installs not confirmed |
| T1502 | Troubleshoot systems and servers | Partial: troubleshooting is done; server-specific exposure not confirmed |
| T1588 | Diagnose faulty system and server hardware | Partial: students diagnose faulty hardware; server hardware not confirmed |
| T1589 | Repair faulty system and server hardware | Partial: students replace or repair faulty hardware; server hardware not confirmed |

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
| T1463 | Develop cybersecurity curriculum goals and objectives | Strong: framework goals and module objectives written (author-stated) |
| T1475 | Develop instructional strategies | Strong: verify-and-correct method applied across courses (author-stated) |
| T1451 | Create interactive learning exercises | Partial: live labs and the AI exchange exercise; toolkit lesson not yet run outside |
| T1608 | Perform periodic reviews of learning materials and courses for accuracy and currency | Partial: Spring 2027 redesign planning documents review course content |
| T1438 | Determine effectiveness of instruction and training | Partial: submissions exist in CIS 251 (12 of 12); only one each in CIS 246 and 268 so far; no aggregate effectiveness analysis yet |
| T1446 | Conduct learning needs assessments | Strong: learning needs assessment done by the author (author; basis to be described) |

**Secondary work role:** OG-WRL-005 Cybersecurity Instruction (OPM 712)

| Task ID | Official task statement | Fit |
|---|---|---|
| T1413 | Develop training modules and classes | Strong: AI-module assignments exist in CIS 246, 251 and 268 (rubric-graded) |
| T1414 | Develop training assignments | Strong: AI-module assignment with a 3-criterion rubric exists in CIS 246, 251 and 268; as of 2026-11-27 submissions: CIS 251 12 of 12 (graded), CIS 246 1 of 15, CIS 268 1 of 13 |
| T1415 | Develop training evaluations | Partial: rubric-based evaluation of student AI-module work; no separate evaluation instrument stated |
| T1416 | Develop grading and proficiency standards | Strong: grading standards in the AI-module rubric (author-stated) |
| T1418 | Develop learning objectives and goals | Strong: learning objectives written for the AI modules (author-stated) |
| T1421 | Develop proficiency assessments | Strong: AI-module rubric and the toolkit rubrics (author-stated) |
| T1537 | Determine if cybersecurity training, education, and awareness meet established goals | Partial: submissions exist mainly in CIS 251; no aggregate check against goals yet |
| T1609 | Recommend revisions to learning materials and curriculum | Partial: revisions recommended in the Spring 2027 planning documents |

## M10 AI security (new content, Track B; to be written)

Seeded from the CIS 214 and 280 redesigns and the AI module. **No work role claim is possible.** In NICE v2.2.0 none of the AI-security knowledge or skill statements below is linked to any work role (the one exception, K0904, is carried only by Data Analysis, IO-WRL-001). The alignment is to competency area NF-COM-002 only. NICE v2.2.0 defines no dedicated AI work role.

| ID | Type | Statement | Work roles carrying it | Fit |
|---|---|---|---|---|
| K1320 | knowledge | Knowledge of common AI security risks | none | Planned: module to be written |
| K1324 | knowledge | Knowledge of data poisoning cyberattacks | none | Planned: module to be written |
| K1333 | knowledge | Knowledge of misinformation and disinformation vulnerabilities in AI systems | none | Planned: module to be written |
| K1334 | knowledge | Knowledge of NIST AI Risk Management Framework | none | Planned: module to be written |
| K1341 | knowledge | Knowledge of test, evaluation, verification, and validation (TEVV) processes | none | Planned: module to be written |
| K1342 | knowledge | Knowledge of training, validation, and test data sets | none | Planned: module to be written |
| K1345 | knowledge | Knowledge of agentic AI principles and practices | none | Planned: module to be written |
| S0955 | skill | Skill in evaluating machine learning models | none | Planned: module to be written |
| S0956 | skill | Skill in evaluating the performance of algorithms | none | Planned: module to be written |
| S0957 | skill | Skill in identifying possible mistakes or hallucinations in AI-generated outputs | none | Strong: students verify and correct AI output in the deployed AI modules (CIS 246, 251, 268); submissions exist, not yet aggregated (author-stated) |
| S0953 | skill | Skill in developing prompts for generative AI systems | none | Partial: students write prompts and document the AI exchange; no separate prompt-design unit stated |
| K0904 | knowledge | Knowledge of machine learning principles and practices | IO-WRL-001 | Planned: module to be written |

## M11 OT/IoT (new content, to be written)

**Work role:** DD-WRL-009 Operational Technology (OT) Cybersecurity Engineering (OPM none). NICE v2.2.0 also lists competency area NF-COM-010 Operational Technology (OT) Security, but the file links **no items** to it, so no K/S statement can be cited for it. Simulation-testbed OT/IoT work by the author exists as unsubmitted drafts and is not cited here as evidence of adoption or outcomes. Module content is to be written.

| Task ID | Official task statement | Fit |
|---|---|---|
| T2047 | Inventory OT assets | Planned: module to be written (seed: unsubmitted simulation-testbed drafts) |
| T2028 | Develop OT inventory model for cybersecurity  | Planned: module to be written (seed: unsubmitted simulation-testbed drafts) |
| T2031 | Identify gaps in OT network architecture | Planned: module to be written (seed: unsubmitted simulation-testbed drafts) |
| T2045 | Assign networked engineering assets to security zones | Planned: module to be written (seed: unsubmitted simulation-testbed drafts) |
| T2032 | Assign security level targets to network zones for control systems | Planned: module to be written (seed: unsubmitted simulation-testbed drafts) |
| T2034 | Design cybersecurity tools for OT systems | Planned: module to be written (seed: unsubmitted simulation-testbed drafts) |
| T2037 | Create cybersecurity inspection and test policies and procedures for OT systems | Planned: module to be written (seed: unsubmitted simulation-testbed drafts) |
| T2042 | Generate cyberattack scenarios of serious physical consequence | Planned: module to be written (seed: unsubmitted simulation-testbed drafts) |
| T1619 | Perform risk and vulnerability assessments | Planned: module to be written (seed: unsubmitted simulation-testbed drafts) |
| T2051 | Train cybersecurity defense technicians on OT system processes and procedures | Planned: module to be written (seed: unsubmitted simulation-testbed drafts) |

