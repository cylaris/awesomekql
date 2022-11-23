# Cylaris AwesomeKQL 

Cylaris AWESOMEKQL is an **awesome** repository of detection R&D created exclusively by the Cylaris Threat Research Group (TRG)

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

![](https://img.shields.io/github/commit-activity/m/cylaris/awesomekql?color=purple&style=flat-square) ![](https://img.shields.io/website?down_color=red&style=flat-square&up_color=purple&url=https%3A%2F%2Fcylaris.org) ![](https://img.shields.io/keybase/pgp/cylaris?color=purple&style=flat-square) ![](https://img.shields.io/github/license/cylaris/awesomekql?color=purple&style=flat-square)


# Content

## Azure

**OAuth App Abuse**
- [Potentially Malicious OAuth app link clicked](https://github.com/cylaris/awesomekql/blob/main/Azure/Oauth/CylarisTRG-MaliciousAppAuth_EmailLinkClicked.json "Potentially Malicious OAuth app link clicked")
- [Potentially Malicious OAuth app visited](https://github.com/cylaris/awesomekql/blob/main/Azure/Oauth/CylarisTRG-MaliciousAppAuth_LinkVisited.json "Potentially Malicious OAuth app visited")

**Phishing**
- [Clicked Link tracker](https://github.com/cylaris/awesomekql/blob/main/Azure/Phishing/CylarisTRG-LinkTracker-ThreatHunt-KQL.json "Clicked Link tracker") (map email URL to Endpoint Logs)

## LOLBAS

**App Installer abuse**
- [Abuse of the native Win bin ms-appinstaller](https://github.com/cylaris/awesomekql/blob/main/lolbas/lol-appinstaller-sentinel-kql.txt "Abuse of the native Win bin ms-appinstaller")

**BITSAdmin Abuse**
- [Abuse of the native Win bin Background Intelligent Transfer Service, BITSadmin]()

**Certutil Abuse**
- [Abuse of the native Win bin certutil, certutil.exe](https://github.com/cylaris/awesomekql/blob/main/lolbas/lol-bitsadmin-abuse-download.json "Abuse of the native Win bin certutil")

**CScript Abuse**
- [Abuse of the native Win bin cscript, cscript.exe](https://github.com/cylaris/awesomekql/blob/main/lolbas/lol-cscript-ads-sentinel-kql.txt "Abuse of the native Win bin cscript")

**Findstr Abuse**
- [Abuse of the native Win bin findstr, findstr.exe](https://github.com/cylaris/awesomekql/blob/main/lolbas/lol-findstr-abuse-sentinel-kql "Abuse of the native Win bin findstr")

## Malware Tracking

**HAFNIUM**
- [Tracking of the malware Hafnium](https://github.com/cylaris/awesomekql/tree/main/malwaretracking/hafnium "Tracking of the malware Hafnium") Likely aligned with APT40. Known to target US

**QakBot**
- [Tracking of the QBot/Qakbot malware](https://github.com/cylaris/awesomekql/tree/main/malwaretracking/qbot-tracking "Tracking of the QBot/Qakbot malware") This is a modular information stealer

**Ransomware**
- [Tracking of various ransomware groups + wares](https://github.com/cylaris/awesomekql/tree/main/malwaretracking/ransomware "Tracking of various ransomware groups + wares")

## Threat Intel
- [Twitter IOC ingestion inline](https://github.com/cylaris/awesomekql/blob/main/threatintel/cti-twitter-ioc-ingestion.json "Twitter IOC ingestion inline") Pulls from [0xDanielLopez Tweetfeed](https://github.com/0xDanielLopez/TweetFeed "0xDanielLopez Tweetfeed"). Ingests inline. Also includes a [mapped version](https://github.com/cylaris/awesomekql/blob/main/threatintel/cti-twitter-ioc-mapping.json "mapped version"). 

## Vulnerabilities Tracking
- [ProxyNotShell, a Sysmon and W3CIISLog version](https://github.com/cylaris/awesomekql/tree/main/vulnerabilities/ProxyNotShell "ProxyNotShell, a Sysmon and W3CIISLog version")
- [CVE-2021-28310, DWM. Win32k Elevation of Privilege](https://github.com/cylaris/awesomekql/tree/main/vulnerabilities/cve-2021-28310 "CVE-2021-28310, DWM. Win32k Elevation of Privilege")

