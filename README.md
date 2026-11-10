# Windows Security Event Log Analysis & Incident Investigation

## Project Overview

This project demonstrates a practical approach to investigating Windows Security events and identifying unusual authentication patterns.

The investigation focuses on analysing login-related events, correlating authentication failures with successful logins, constructing an event timeline, and documenting security findings.

The project uses a controlled synthetic dataset to simulate a Windows authentication investigation scenario.

**Data Disclaimer:** All records included in the training dataset are fictional. They are created for educational purposes and do not represent actual security events collected from a real organisation or computer.

## Investigation Objectives

- Examine common Windows Security Event IDs.
- Understand successful and failed authentication events.
- Identify repeated login failures involving a single account.
- Correlate authentication events using timestamps and available identifiers.
- Develop a chronological investigation timeline.
- Assess potentially suspicious authentication behaviour.
- Document investigation findings and recommended actions.
- Perform SHA-256 file integrity verification.

## Tools & Technologies

- Windows 11
- Windows Event Viewer
- PowerShell
- Command Prompt
- Visual Studio Code
- Git and GitHub
- CSV datasets
- SHA-256 hashing

## Windows Security Events

The investigation covers the following Windows Security Event IDs:

| Event ID | Description |
|---|---|
| 4624 | Successful Logon |
| 4625 | Failed Logon |
| 4634 | Logoff |
| 4672 | Special Privileges Assigned |

## Investigation Scenario

A fictional organisation observes an unusual authentication pattern involving a user account.

During the investigation, the analyst identifies multiple failed network logon attempts followed by a successful authentication event involving the same account and sample source IP address.

The objective is to examine this sequence, understand its potential security implications, and determine whether additional investigation is necessary.

## Initial Investigation Findings

The synthetic dataset contains:

- Four failed authentication attempts involving the same account.
- Repeated activity originating from the same documentation-only IP address.
- A successful network logon 41 seconds after the final recorded failure.
- A subsequent logoff event associated with the sample successful session.

This pattern may be consistent with password guessing or another authentication-related issue. However, the available information is insufficient to establish unauthorised access.

**Initial Assessment:** Potentially Suspicious — Further Investigation Required.

## Project Structure

```text
windows-security-log-investigation/
│
├── dataset/
├── evidence/
├── analysis/
├── reports/
├── screenshots/
│
├── README.md
└── LICENSE
```

## Investigation Methodology

The project follows a structured investigation workflow:

1. Explore Windows Security logs using Event Viewer.
2. Review relevant authentication-related Event IDs.
3. Prepare and examine the synthetic event dataset.
4. Identify repeated authentication failures.
5. Correlate failed and successful login events.
6. Construct an investigation timeline.
7. Assess the observed activity.
8. Verify dataset integrity using SHA-256.
9. Prepare a documented investigation report.

## Investigation Limitations

- The dataset contains fictional training records.
- The investigation does not establish an actual security breach.
- The available records represent only a limited set of Windows Security events.
- Additional endpoint, network, identity, and authentication evidence would be required for a real-world investigation.
- Event correlation alone cannot confirm malicious intent.

## Expected Learning Outcomes

This project demonstrates foundational skills in:

- Windows Security Event Log analysis.
- Authentication monitoring.
- Suspicious login investigation.
- Event correlation and timeline construction.
- Basic incident assessment.
- Evidence integrity verification.
- Security investigation documentation.

## Disclaimer

This project is developed strictly for cybersecurity education and practical skill development. All identities, systems, and authentication records used in the synthetic dataset are fictional.
