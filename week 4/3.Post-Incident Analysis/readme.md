Post-Incident Analysis Report

Objective

The objective of this task is to perform a Root Cause Analysis (RCA) of a phishing incident, identify contributing factors, and evaluate SOC performance using key metrics such as MTTD and MTTR.

Tools Used

Google Sheets (RCA documentation, metrics)
Draw.io (Fishbone Diagram)

Root Cause Analysis (5 Whys Method)

Question	Answer
Why was the email opened?	User clicked a malicious link
Why was the link clicked?	Email appeared legitimate and urgent
Why did it appear legitimate?	Lack of advanced email filtering
Why was filtering weak?	Outdated security rules and no sandboxing
Why were controls outdated?	Lack of regular security updates and audits

Fishbone Diagram (Cause Analysis)

Categories Identified

1. People

Lack of security awareness training
User unable to पहचान phishing indicators

2. Process

No phishing simulation exercises
Weak incident reporting procedure

3. Technology

Ineffective email filtering
No attachment sandboxing
Missing URL reputation checks

4. Policy

No enforced email security policy
Lack of mandatory training compliance

 5. Environment

High email volume causing user fatigue
Remote work increasing exposure

SOC Metrics Calculation

Given:
Detection Time = 2 hours
Response Time = 4 hours

Metrics:

MTTD (Mean Time to Detect): 2 hours
MTTR (Mean Time to Respond): 4 hours

Metrics Summary (50 words)

The incident analysis revealed a Mean Time to Detect (MTTD) of 2 hours and a Mean Time to Respond (MTTR) of 4 hours. While detection was relatively quick, response time indicates room for improvement. Enhancing automation and alert prioritization can significantly reduce response delays and improve SOC efficiency.
