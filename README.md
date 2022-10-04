![alt text](https://static.wixstatic.com/media/fa2da5_a22354e11ada4292a79e0f8c2289b31b~mv2.png/v1/fill/w_243,h_113,al_c,q_85,usm_0.66_1.00_0.01/Monochrome%20on%20Transparent_edited.webp)

# AWESOMEKQL - Microsoft Security Detection

AwesomeKQL is a repository of latest vulnerability research and detection efforts built by mostly @ntwrite from many references for which I am very grateful. 

These detection packs or 'rules' are KQL queries written after various testing of exploits as well as investigation into technical write ups from other vendors, including static analysis and network indicators. 

## Description

KQL is the primary querytype used by Microsoft security stack. Queries are built usually by engineers/ malware analysts etc to catch malicious behaviour on a SIEM to detect malicious behaviour on an environment, at various levels of the MITRE ATT&CK framework.

We build those to catch the latest vulnerabilities and threats.

The aim for these rules is to use 
- Network Level Indicators
  
These are a first-effort response which use the earliest possible IOCs uncovered by bad actors exploiting vulnerabilities. Usually unreliable but good    for a first response.
  
- Static Indicators

Static Indicators are attributes that artifacts have that have been seen historically, again, these are unreliable but can prevent many attacks   nonetheless.
  
- Behavioural Patterns (Heuristic)

After analysis is carried out on various research, as well as tests, most malware families and even APT's share many similar traits. This is where we   are able to identify these patterns. Most of our detection packs use this - however these take a LOT of time, for research and testing. So you may see us release the previous types initially as a first-effort mitigation and detection.

## What's this about?
Folders contain malware-family or APT specific detection packs. 

We are a non-profit using our own time to build these to protect and help people. If you would like to join us - please email extcomms@cylaris.org as we are always looking for enthusiastic and passionate volunteers.

https://cylaris.org
