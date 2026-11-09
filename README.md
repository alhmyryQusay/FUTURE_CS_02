# Future Interns | Cyber Security Task 2

## Phishing Email Detection & Awareness Report

**Candidate:** QUSAY ALHEMIRY  
**Internship:** Future Interns - Cyber Security (November 2026)  
**Review date:** 09 November 2026  
**Deliverable:** Six-page PDF report with evidence and employee awareness guidance.

## Project objective
Review publicly shared phishing-email examples, identify warning indicators, interpret available email headers and links safely, classify the samples, and prepare clear phishing-prevention guidance for employees.

## Samples and classification

| ID | Public educational email scenario | Assessment | Risk |
|---|---|---|---|
| PH-01 | Fake fax / SharePoint notification | Phishing | High (scenario) |
| PH-02 | Lookalike Microsoft account alert | Phishing | High (scenario) |
| PH-03 | Voice-message notification with HTML redirect | Phishing | High (scenario) |

All three are **public educational/research samples**, not verified live incidents. A "Safe" or "Suspicious" label is covered in the report's classification rubric; no safe email was falsely invented or tested.

## Tools used
- GitHub web interface to inspect public sample `.eml` and HTML source as static text
- Google Admin Toolbox Messageheader Analyzer for available Microsoft-alert header data
- Browser text search and static HTML/URL inspection (no suspicious URL opened)
- PDF report authored from original observations and screenshots

## Analysis approach
1. Read the available email fields and any authentication results.
2. Inspect sender claims, wording and displayed link text.
3. Examine the actual URL in `href` or redirection code **as text only**.
4. Consider evidence in combination; separate observed facts from inferences.
5. Record an assessment, limitations, and practical employee guidance.

## Evidence and sample notes
- `Phishing_Detection_Awareness_Report.pdf` - final six-page report.
- `Evidence/` - selected original screenshot excerpts and a comparison crop.
- `Sample_Analysis/` - short, defanged notes with source attribution, indicators and limits.

## Source attribution
- PH-01: https://github.com/autinerd/phishing-mail-examples/tree/main/new-fax-message/example1
- PH-02: https://github.com/jacobdcook/Phishing-Analysis-Lab/blob/main/samples/sample2.eml
- PH-03: https://github.com/autinerd/phishing-mail-examples/tree/main/voice-message/example1

These are third-party educational source samples. The original messages and datasets are **not** claimed as the candidate's creations. The analysis, screenshots captured during study, explanations and report are this training project's work.

## Safety and limitations
No suspicious link was visited or resolved, no HTML attachment was run, no passwords were provided and no malware was executed. Header-authentication outcomes were read from the public samples and analyzer output; they were **not independently verified from a live mail server**. Some source values are documentation placeholders (`example.com`, `192.0.2.1`), so do not treat them as real attacker infrastructure. The Google parser was useful for PH-02; the first sample's available headers did not support a comparable full routing analysis. This is an educational static review, not a forensic attribution of a live incident.

## Employee takeaway
**Stop - Verify independently - Report.** Do not trust branding or message urgency, and do not open unexpected HTML attachments or shortened links.
