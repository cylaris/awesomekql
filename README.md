# Universal SIGMA SIEM Intrusion Detection rules


## Description
SIGMA is a relatively new, and vendor-neutral rule writing language, developed by Florian Roth @Neo23x0, it is truly revolutionary. 
Rules like these can be implemented into SIEM solutions from Elastic to Sentinel to Qradar and Splunk, chances are, if you have a SIEM solution you'll be able to make good use of SIGMA.

\For inexperienced viewers, please see the next section. Otherwise, see section titled purpose.

##What are rules?
Rules are the name given to a set of pre-defined queries which continually search for malicious, suspicious or unauthorised activity on a computer network. These are put into an IDS system, usually a SIEM, which is hooked up to the vast majority of the network, such as domain controllers, fileservers, active directory, azure or aws, 365, google, firewalls and any other service utilised by your organisation.
The rules are then automatically and constantly searching the network (depending on your set-up or differing siem software) for activity DEEMED bad by the security team. For example, in Azure Sentinel
  SecurityEvent
  | where EventID == "4625" 

SecurityEvent is the table queried by this particular query, think of it as a singular dataset, where logs are collected from windows machines, 
pipe, where operator (to specify, where x happens), Event ID, a specific value assigned to a particular event within Windows Operating systems
with its own column within the SecurityEvent table, == defines this is EXACTLY the value you are searching for in the specified column.
EventID 4625 is a logon failure, so this query is searching for a logon failure.
So, overview: the securityevent table is being queried, in the EventID column for the EXACT value of 4625, which indicates a logon failure - 
keep in mind, this does not show only interactive logon failures aka, pebdac, user error or attempted compromises, but too configuration errors, 
annoying old webservers and domain controllers, broken service accounts which may fall under network logons, but may help in identifying these issues
to resolve them from a config POV.

##What is the purpose of this repo?
BaseDFIR seeks to help others, as well as polish our own skillsets. This repo is a great resource for those looking for extra security rules and serves
us great purpose when the community submits suggestions and edits to our rules, teaching us too a lesson or two. 

###References
Florian Roth, Sigma https://github.com/Neo23x0
