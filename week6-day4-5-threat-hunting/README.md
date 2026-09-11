# Week 6 Day 4-5: Threat Hunting and Detection Engineering

## Purpose

The purpose of this lab was to investigate a security incident by expanding the incident timeline, hunting across multiple systems, mapping attacker activity to MITRE ATT&CK, and creating detection rules to help identify similar attacks in the future.

The lab also focused on understanding the full scope of an incident and developing containment, eradication, and recovery steps.

## What I Did

During this lab, I:

- Reviewed network and host evidence
- Built an extended incident timeline
- Performed a fleet-wide threat hunt
- Identified compromised and clean systems
- Organized indicators using the Pyramid of Pain
- Mapped attacker activity to MITRE ATT&CK
- Created Sigma detection rules
- Investigated persistence and lateral movement
- Developed containment, eradication, and recovery steps
- Identified detection gaps

## What I Learned

I learned that one source of evidence does not always show the full story of an attack. Network logs helped identify attacker activity that happened before some of the available host logs.

I also learned how threat hunting can determine how far an attacker moved through an environment. MITRE ATT&CK helped me organize the attacker's actions, while Sigma rules showed me how evidence from an investigation can be turned into future detections.

Another important takeaway was that IP addresses, filenames, and other simple indicators can be changed easily by an attacker. Detecting attacker behavior can provide stronger long-term protection.

## Key Takeaways

- Multiple evidence sources are important during investigations
- Threat hunting helps determine the scope of an incident
- MITRE ATT&CK helps organize attacker behavior
- Sigma rules can turn investigation findings into detections
- Behavior-based detections are harder for attackers to avoid
- Incident findings can be used to improve future security


## Lab Documents

- [Day 4-5 Investigation Spreadsheet](https://docs.google.com/spreadsheets/d/1dvqTtX3Hlqd8hl9GnHGBgADna3Ug5jBb_u01MbLGRKI/edit?usp=sharing)
- [MTB Incident Scoping Report](https://docs.google.com/document/d/1yfNAtg24sijbJpM-LuUKV10qMlkqvyEQTl86K5qbDdM/edit?usp=sharing)
- [Threat Hunting and Detection Engineering Report](https://docs.google.com/document/d/1vfdYsbQUXGV-eLGmP035WGjScGBKfRSROZ5BRUoYE5c/edit?usp=sharing)
