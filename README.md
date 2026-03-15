📌 Incident Management - Reference & Guidelines

🔍 What is a Data Production Incident

A data production incident refers to any event that disrupts the expected flow, accuracy, performance, or accessibility of data products or pipelines within the enterprise data engineering, reporting, and analytics environment.

Incidents are typically logged and tracked through operational tools and are prioritised based on severity, business impact, and affected stakeholders.



📏 Measurement Approach

The measurement approach for data production incidents involves systematically tracking, categorising, and analysing events that impact the flow, accuracy, performance, or accessibility of data across the data engineering and analytics environment.

This includes capturing key attributes such as incident type, severity, priority, affected systems, resolution time, and root cause, to assess operational performance, identify recurring issues, and monitor service level compliance.

The goal is to provide actionable insights into incident trends, reduce overall incident volume, and improve time to resolution and data reliability across the enterprise.



⚠️ Severity & Priority Matrix Framework

Sev/Pri

P1 (Highest) 

P2 (High)

P3 (Medium)

P4 (Low)

Sev1 (Critical)

P1 SEV1: Immediate action required. Complete outage or failure affecting critical reporting access. 

⏱ SLA: Response within 1 hour | Resolution within 1 working day

P2 SEV1: Action required after critical issues. Failure in a key pipeline used by ops/daily reporting. 

⏱ SLA: Response within 1 working day | Resolution within 2 working days



P3 SEV1: Address during routine ops. Important metric outage in non-critical dashboard; workaround available.

⏱ SLA: Response within 1 working day | Resolution within 5 working days

P4: SEV1: Critical label flagged, but low user impact or capacity impact. Resolve when time permits. 

⏱ SLA: Response within 2 working days | Resolution within 7 working days

Sev2 (High)

Rapid response required. Partial pipeline disruption or stale data in critical reports. 

⏱ SLA: Response within 1 working day | Resolution within 2 working days

Timely action expected. Missed refresh in dashboard or repeated delays in key process. 

⏱ SLA: Response within 1 working day | Resolution within 3 working days

Fix in routine cycle. Low-volume data feed failed or semi-critical reporting delay for a group of users. 

⏱ SLA: Response within 1–2 working days | Resolution within 7 working days

Critical but capacity dependent or small workaround in place. Heavy file slowing down ETL. 

⏱ SLA: Response within 2 working days | Resolution within 9 working days

Sev3 (Medium)

Semi-critical SFTP file load failed or bad data file. 

⏱ SLA:   Response within 1 working day | Resolution within 3 working days

Handle post-critical work due to interim solution in place. Semi-critical SFTP file load failure or  non-critical pipeline failure. 

⏱ SLA:  Response within 1–2 working days | Resolution within 7 working days

Sprint-ready due to capacity. Data inconsistencies in reporting or Non-critical SFTP file delays

⏱ SLA: Response within 1–2 working days | Resolution within 2–4 weeks (depending on complexity)  

Track for review. SFTP file metadata changes. or data inaccuracy fixes needed. 

⏱ SLA: Response within 3 working days | Resolution reviewed and prioritised within 2–4 weeks

Sev4 (Low)

Non-urgent. Cosmetic issue in high-visibility dataset. 

⏱ SLA: Response within 1 working day | Resolution within 5 working days

Log as tech debt. Deprecated column still in feed. 

⏱ SLA:  Response within 2 working days | Resolution within 2 weeks or next sprint

Enhancement worthy. User request to clean headers or improve data labels in exports. 

⏱ SLA: Response within 3 working days | Reviewed and planned within sprint backlog

Monitor unless repeated. Visual or naming tweaks with zero operational impact.

⏱ SLA: Response within 3 working days | Resolution within 4–6 weeks, unless re-prioritised sooner due to repeated occurrences or user impact



📝 Notes:

Sev3 incidents often involve active interim solutions that reduce business impact temporarily. These issues are still monitored closely, and resolution is prioritised based on risk of escalation or interim failure.

Sev4 incidents may not require immediate action and are typically cosmetic or logged for future backlog review.

SLAs are tracked from the moment the incident is confirmed and assigned with a validated priority.



📢 Incident Communication Plan

🛑 Comms Plan for P1 (SEV1) Incidents

Initial Notification:
Within 1 hour of identifying a P1 incident, a call will be arranged to discuss the resolution approach. Affected users and key stakeholders will receive an email outlining the incident, its impact, next steps, and an initial estimate of the resolution timeframe.

Ongoing Updates:
If the issue isn't resolved or an interim solution is not in place by the end of the working day, an email will be sent notifying progress, any blockers, and updates on the estimated resolution timeframe.

Resolution Notification:
Once the incident is resolved, a final email will be sent to all stakeholders. A separate email will be sent to the Head of Data, providing a detailed summary of the root cause, impact, mitigation, and resolution, including timeframes.



⚠️ Comms Plan for P2 (SEV2) Incidents 

Initial Notification:
Within 1 working day of identifying a P2 incident, affected users and key stakeholders will receive an immediate email outlining the incident, its impact, next steps, and an initial estimate of the resolution timeframe. A call will be arranged if necessary to discuss the approach.

Ongoing Updates:
If the issue isn’t resolved within the same working day or if there is any significant delay, an email will be sent providing progress updates, any blockers, and changes to the estimated resolution timeframe.

Resolution Notification:
Once the incident is resolved, a final email will be sent to all stakeholders with the resolution details.



🛠 Comms Plan for P3 & P4 (SEV3 / SEV4) Incidents 

Initial Notification:
Affected users and key stakeholders will be notified via email within 1-2 working days for P3, or 2-3 working days for P4. The email will provide an overview of the issue, impact, and any interim solution in place.

Ongoing Updates:
If the issue isn’t resolved within the timeframe, or there’s a significant update, an email will be sent with progress updates, blockers, and any changes to the expected resolution timeframe. These updates will be sent periodically as needed.

Resolution Notification:
Once the issue is resolved, a final email will be sent to all relevant stakeholders.



🔄 General Lifecycle of a Data Production Incident

1. Incident Detection

Detected automatically or reported by users.

Logged with required details, including severity, priority and affected systems. 

2. Incident Notification

Immediate email notifications to affected users and stakeholders with impact and next steps.

Team assignment for resolution.

3. Investigation & Root Cause Analysis

Team investigates root cause and applies interim solutions if needed.

4. Ongoing Updates & Communication

Regular updates sent based on incident severity, with progress and resolution timeframes.

5. Resolution & Fix Implementation

Root cause identified and fixed, tested, and validated.

6. Incident Closure

Incident closed after validation, and a final notification is sent to stakeholders.

7. Post-Incident Review & Documentation

Incident review for impact, root cause, and lessons learned.

Action plan for future prevention, if needed.

8. Continual Improvement

Update processes and tools to improve future incident responses.
