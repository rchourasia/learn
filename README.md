
***

### Content
1. [Overview](#overview)
2. [Escalation Process - Level 1](#process)
3. [New Escalation Issue Creation on GitHub](#issuecreation)
4. [Issue Assignment Workflow](#assignment)
5. [Engineering Escalation Duty Roster](#roster)
6. [Key Resources](#resources)

<a name="overview"></a>
# 1. Overview
The primary objective of this document is to explain the process involved with seeking escalation support from Runtime Engineering. Source of the such could range from reporting a bug of significant impact to an Existing Customer deployment to an issue blocking sale or renewal opportunities.

As the first phase of the new escalation process, new GitHub repository dedicated for escalations is being instituted wherein each new issue reported triggers PagerDuty alerts to On-call Engineering Contacts in the follow-the-Sun model between SFO, Paris & Cambridge timezones, who would then route the issues to appropriate teams. In later phases, more optimizations and automation are targeted to further streamline and optimize the process.

<a name="process"></a>
# 2. Escalation Process - Level 1

<img src="https://github.com/rchourasia/learn/blob/master/escalationprocess.png" width="100%">

<a name="issuecreation"></a>
# 3. New Escalation Issue Creation on GitHub

* **Repository** - Create New Issue in [Escalation](https://github.com/docker/escalation/) Repository
* **Title** - Provide short description of the issue. Description Should Include: 
    * Problem/Feature Request Description
    * Issue Reported by: Customer Name, Pre-sales, Existing Deployment
    * Environment details [If applicable]: Dev/Test , Production
* **Severity [label]**
    * S0-catastrophic: Watchlist Issues; Production System Down; No Workaround; Sales/Renewal Impacting
    * S1-broken: Major Functionality Loss; No Workaround
    * S2-major: Major Functionality Loss; Workaround available
    * S3-minor: Minor Issues; Usability Issues; Workaround available
* **Type [label]** - bug ; enhancement ; process ; question 
* **Version [label]**
    * 1.11 (ucp: - dtr: 2.0)
    * 1.12 (ucp: - dtr 2.1)
    * 1.13 (ucp: - dtr: n/a)
    * 17.03 (ucp: 2.1 - dtr 2.2)
    * 17.06 (ucp: 2.2 - dtr 2.3)
* **Workaround [label]** - Yes [if workaround available]
* **Area [label]** (If known)
    * DTR 
    * engine
    * network
    * orchestration
    * packaging
* **Logs [Attachment]** - UCP - UCP Support Dumps ; Engine - Engine Logs

<a name="assignment"></a>
# 4. Issue Assignment Workflow

<img src="https://github.com/rchourasia/learn/blob/master/assignmentworkflow.png" width="100%">

<a name="roster"></a>
# 5. Engineering Escalation Duty Roster
* Coverage provided by SFO, Paris & Cambridge teams [Monday - Friday]
* Hours with **NO on-call coverage**  - Between 5 PM (Pacific) & 11 PM (Pacific)
* Relies on PagerDuty to trigger and escalate incidents during supported hours
* [Duty Roster - Living Document](https://docs.google.com/a/docker.com/spreadsheets/d/1Ae20C1RLnG5b_c51aoYmy9wvcXoJf5Ym2sYs55WmGhg/edit?usp=sharing)


<a name="resources"></a>
# 6. Key Resources
* [PagerDuty](https://docker.pagerduty.com)
* [GitHub Escalation Repo](https://github.com/docker/escalation/)
* Engineering Assignments [**To be Used by Leads to route the escalations within engineering**]
    * [UCP](https://github.com/docker/orca/wiki)
    * DTR (Viktor to provide)
    * Engine (Victor to Provide)
