# Cylaris AwesomeKQL 

Cylaris AWESOMEKQL is an **awesome** repository of detection R&D created exclusively by the Cylaris Threat Research Group (TRG) :fa-user-secret:

This repo is for:
- SOC Analysts (Threat Hunting) 
- SOC Engineers (Detection Packs)
- Researchers 
- Linux Nerds 

### Content

- Network Level Indicators
These are a first-effort response which use the earliest possible IOCs uncovered by bad actors exploiting vulnerabilities. Usually unreliable but good for a first response.

- Static Indicators
Static Indicators are attributes that artifacts have that have been seen historically, again, these are unreliable but can prevent many attacks nonetheless.

- Behavioural Patterns (Heuristic)
After analysis is carried out on various research, as well as tests, most malware families and even APT's share many similar traits. This is where we are able to identify these patterns. Most of our detection packs use this - however these take a LOT of time, for research and testing. So you may see us release the previous types initially as a first-effort mitigation and detection.

# detections - awesomekql
<img width="300px" border=0 src="https://cylaris.org/assets/cylarisghp.svg"></img>

![](https://img.shields.io/github/commit-activity/m/cylaris/awesomekql?color=purple&style=flat-square) ![](https://img.shields.io/website?down_color=red&style=flat-square&up_color=purple&url=https%3A%2F%2Fcylaris.org) ![](https://img.shields.io/keybase/pgp/cylaris?color=purple&style=flat-square) ![](https://img.shields.io/github/license/cylaris/awesomekql?color=purple&style=flat-square) ![](https://img.shields.io/github/issues/pandao/editor.md.svg) ![](https://img.shields.io/bower/v/editor.md.svg)


**Table of Contents**

[TOCM]

##Azure
**OAuth App Abuse**
- [Potentially Malicious OAuth app link clicked](https://github.com/cylaris/awesomekql/blob/main/Azure/Oauth/CylarisTRG-MaliciousAppAuth_EmailLinkClicked.json "Potentially Malicious OAuth app link clicked")
- [Potentially Malicious OAuth app visited](https://github.com/cylaris/awesomekql/blob/main/Azure/Oauth/CylarisTRG-MaliciousAppAuth_LinkVisited.json "Potentially Malicious OAuth app visited")

**Phishing**
- [Clicked Link tracker](https://github.com/cylaris/awesomekql/blob/main/Azure/Phishing/CylarisTRG-LinkTracker-ThreatHunt-KQL.json "Clicked Link tracker") (map email URL to Endpoint Logs)
