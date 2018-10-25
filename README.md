---
layout: default
---
# OOB Automated Testing ![Discord](https://img.shields.io/discord/289994252241338369.svg) [![Discord Invite](https://img.shields.io/badge/discord-invite-green.svg)](https://discord.gg/QaMwnGd)

OOB Automated Testing is a scoped app to 
capture tests for all the Out of Box 
servicenow applications.

## Installation

Due to this being a Scoped Application, to make this work with simplifying tests,
one modification must be made in Global Scope.  On 
`/sys_db_object.do?sysparm_query=name=sys_user_group`
under "Application Access", check "Can create", "Can update", "Can delete", and
save.

* servicenow instance London or newer
* Import `https://github.com/jacebenson/x_8821_atf.git` 
  to source control within Studio.

## Features

Tests will exist for and already exist for some of servicenow.

Below is the suite hierarcy.  If checked done.

- API Testing
  - [Agent Intelligence](https://github.com/jacebenson/x_8821_atf/issues/1)
  - [Aggregate API](https://github.com/jacebenson/x_8821_atf/issues/2)
  - [Application Service API](https://github.com/jacebenson/x_8821_atf/issues/3)
  - [Attachment API](https://github.com/jacebenson/x_8821_atf/issues/4)
  - [CI Lifecycle Mangement API](https://github.com/jacebenson/x_8821_atf/issues/5)
  - [Clotho Time Series API](https://github.com/jacebenson/x_8821_atf/issues/6)
  - [CMDB Instance API](https://github.com/jacebenson/x_8821_atf/issues/7)
  - [CMDB Meta API](https://github.com/jacebenson/x_8821_atf/issues/8)
  - [Email API](https://github.com/jacebenson/x_8821_atf/issues/29)
  - [IdentifyReconcile API](https://github.com/jacebenson/x_8821_atf/issues/9)
  - [Import Set API](https://github.com/jacebenson/x_8821_atf/issues/28)
  - [Interaction Management API](https://github.com/jacebenson/x_8821_atf/issues/10)
  - [Major Incident Management API](https://github.com/jacebenson/x_8821_atf/issues/11)
  - [Performance Analytics API](https://github.com/jacebenson/x_8821_atf/issues/12)
  - [Service Catalog API](https://github.com/jacebenson/x_8821_atf/issues/13)
  - [Table API](https://github.com/jacebenson/x_8821_atf/issues/14)
  - [Task Communication Management API](https://github.com/jacebenson/x_8821_atf/issues/15)
  - [User Role Maintenance API](https://github.com/jacebenson/x_8821_atf/issues/16)
- Customer Service Management
  - [Communities](https://github.com/jacebenson/x_8821_atf/issues/37)
  - [Customer Service](https://github.com/jacebenson/x_8821_atf/issues/38)
  - [Field Service](https://github.com/jacebenson/x_8821_atf/issues/39)
- Governance, Risk , and Compliance (GRC)
  - [Audit](https://github.com/jacebenson/x_8821_atf/issues/25)
  - [Policy and Compliance](https://github.com/jacebenson/x_8821_atf/issues/40)
  - [Risk](https://github.com/jacebenson/x_8821_atf/issues/33)
  - [Vendor Risk](https://github.com/jacebenson/x_8821_atf/issues/34)
- HR Service Delivery
  - [Case and Knowledge](https://github.com/jacebenson/x_8821_atf/issues/41)
  - [Employee Document](https://github.com/jacebenson/x_8821_atf/issues/42)
  - [Employee Service Center](https://github.com/jacebenson/x_8821_atf/issues/43)
  - [Enterpise Onboarding and Transistions](https://github.com/jacebenson/x_8821_atf/issues/44)
  - [HR Integrations](https://github.com/jacebenson/x_8821_atf/issues/45)
- IT Business Management
  - [Agile Development](https://github.com/jacebenson/x_8821_atf/issues/46)
  - [Business Planning Portal](https://github.com/jacebenson/x_8821_atf/issues/47)
  - [Cost](https://github.com/jacebenson/x_8821_atf/issues/48)
  - [Enterprise Release Management](https://github.com/jacebenson/x_8821_atf/issues/49)
  - [Financial](https://github.com/jacebenson/x_8821_atf/issues/50)
  - [Project Portfolio](https://github.com/jacebenson/x_8821_atf/issues/51)
  - [Scaled Agile Frameworkf (SAFe)](https://github.com/jacebenson/x_8821_atf/issues/52)
  - [Test Management](https://github.com/jacebenson/x_8821_atf/issues/53)
  - [Time Card](https://github.com/jacebenson/x_8821_atf/issues/54)
- IT Operations Management
  - [Cloud Management](https://github.com/jacebenson/x_8821_atf/issues/55)
  - [Discovery](https://github.com/jacebenson/x_8821_atf/issues/56)
  - [Event Management](https://github.com/jacebenson/x_8821_atf/issues/57)
  - [Operational Intelligence](https://github.com/jacebenson/x_8821_atf/issues/58)
  - [Service Mapping](https://github.com/jacebenson/x_8821_atf/issues/59)
- IT Service Management
  - [Asset](https://github.com/jacebenson/x_8821_atf/issues/30)
  - [Benchmarks](https://github.com/jacebenson/x_8821_atf/issues/60)
  - [Change](https://github.com/jacebenson/x_8821_atf/issues/19)
  - [Continual Improvement](https://github.com/jacebenson/x_8821_atf/issues/61)
  - [Contract](https://github.com/jacebenson/x_8821_atf/issues/62)
  - [Expense Line](https://github.com/jacebenson/x_8821_atf/issues/63)
  - [Incident](https://github.com/jacebenson/x_8821_atf/issues/17)
  - [Incident Communications](https://github.com/jacebenson/x_8821_atf/issues/18)
  - [ITSM Virtual Agent](https://github.com/jacebenson/x_8821_atf/issues/64)
  - [On-call Scheduling](https://github.com/jacebenson/x_8821_atf/issues/65)
  - [Problem](https://github.com/jacebenson/x_8821_atf/issues/20)
  - [Procurement](https://github.com/jacebenson/x_8821_atf/issues/66)
  - [Product Catalog](https://github.com/jacebenson/x_8821_atf/issues/67)
  - [Release](https://github.com/jacebenson/x_8821_atf/issues/68)
  - [Request](https://github.com/jacebenson/x_8821_atf/issues/21)
  - [Service Catalog](https://github.com/jacebenson/x_8821_atf/issues/22)
  - [Service Desk](https://github.com/jacebenson/x_8821_atf/issues/69)
  - [Service Level](https://github.com/jacebenson/x_8821_atf/issues/70)
  - [Service Portfolio](https://github.com/jacebenson/x_8821_atf/issues/71)
  - [Vendor Performance](https://github.com/jacebenson/x_8821_atf/issues/72)
  - [Walk-up Experience](https://github.com/jacebenson/x_8821_atf/issues/73)
- Now Platform
  - [Agent Intelligence](https://github.com/jacebenson/x_8821_atf/issues/74)
  - [CMDB](https://github.com/jacebenson/x_8821_atf/issues/75)
  - [Compliance](https://github.com/jacebenson/x_8821_atf/issues/76)
  - [Connect](https://github.com/jacebenson/x_8821_atf/issues/77)
  - [Content Management System](https://github.com/jacebenson/x_8821_atf/issues/78)
  - [Data Certification](https://github.com/jacebenson/x_8821_atf/issues/79)
  - [Dependency Views](https://github.com/jacebenson/x_8821_atf/issues/80)
  - [Flow Designer](https://github.com/jacebenson/x_8821_atf/issues/81)
  - [IntegrationHub](https://github.com/jacebenson/x_8821_atf/issues/82)
  - [Interaction Management](https://github.com/jacebenson/x_8821_atf/issues/83)
  - [Knowledge Management](https://github.com/jacebenson/x_8821_atf/issues/84)
  - [Live Feed](https://github.com/jacebenson/x_8821_atf/issues/85)
  - [Managed Documents](https://github.com/jacebenson/x_8821_atf/issues/86)
  - [MetricBase](https://github.com/jacebenson/x_8821_atf/issues/87)
  - [Notifications](https://github.com/jacebenson/x_8821_atf/issues/88)
  - [Notify](https://github.com/jacebenson/x_8821_atf/issues/89)
  - [Orchestration](https://github.com/jacebenson/x_8821_atf/issues/90)
  - [Password Reset](https://github.com/jacebenson/x_8821_atf/issues/91)
  - [Service Administration](https://github.com/jacebenson/x_8821_atf/issues/92)
  - [Service Portal](https://github.com/jacebenson/x_8821_atf/issues/93)
  - [Subscription Management](https://github.com/jacebenson/x_8821_atf/issues/95)
  - [Survey Management](https://github.com/jacebenson/x_8821_atf/issues/94)
  - [Task Communication Management](https://github.com/jacebenson/x_8821_atf/issues/96)
  - [Virtual Agent](https://github.com/jacebenson/x_8821_atf/issues/97)
  - [Visual Task Boards](https://github.com/jacebenson/x_8821_atf/issues/98)
  - [Workflow](https://github.com/jacebenson/x_8821_atf/issues/99)
- Security Operations
  - [Configuration Compliance](https://github.com/jacebenson/x_8821_atf/issues/100)
  - [Security Incident Response](https://github.com/jacebenson/x_8821_atf/issues/101)
  - [Threat Intelligence](https://github.com/jacebenson/x_8821_atf/issues/102)
  - [Trusted Security Circles](https://github.com/jacebenson/x_8821_atf/issues/103)
  - [Vulnerability Response](https://github.com/jacebenson/x_8821_atf/issues/104)
- Service Management
  - [Coaching Loops](https://github.com/jacebenson/x_8821_atf/issues/35)
  - [Facilities](https://github.com/jacebenson/x_8821_atf/issues/36)
  - [Finance](https://github.com/jacebenson/x_8821_atf/issues/105)
  - [Legal](https://github.com/jacebenson/x_8821_atf/issues/106)
  - [Marketing](https://github.com/jacebenson/x_8821_atf/issues/107)
  - [Planned Maintenance](https://github.com/jacebenson/x_8821_atf/issues/108)
  - [Structured Problem Analysis](https://github.com/jacebenson/x_8821_atf/issues/109)
- [Software Asset Management](https://github.com/jacebenson/x_8821_atf/issues/26)
 

## Contributing

Pull requests are welcome. For major changes, 
please open an issue first to discuss what you 
would like to change.

I'd suggest starting on an [issue that seems well made](https://github.com/jacebenson/x_8821_atf/issues?q=is%3Aopen+is%3Aissue+label%3A%22good+first+issue%22).

However there are a lot of issues for everything I could find in servicenow.  If you know that application feel free to fill out the issue and comment on it.

### Setting up a pdi (personal developer instance)

Create an account on [https://developer.servicenow.com/](https://developer.servicenow.com/).
Than Request a Personal Developer Instance.

### Setting up the repo

Due to this being a Scoped Application, to make this work with simplifying tests,
one modification must be made in Global Scope.  On 
`/sys_db_object.do?sysparm_query=name=sys_user_group`
under "Application Access", check "Can create", "Can update", "Can delete", and
save.

1.  Fork this project
2.  Log into your PDI
3.  Open Studio
4.  Import your Forked Repo's `https` url

### Actually Contributing

1.  Comment on the issue
2.  Ensure you're in the OOB Automated Testing application
3.  Create the tests and suites appropriate to test the application
4.  Put your tests in the appropriate suites
4.  Commit your repo
5.  Comeback onto github, and make a Pull Request from your repo.

## Resources

* If you need to `set fields` but cannot find 
  you're field, this script might be useful;
  ```js
  var gr = new GlideRecord('sys_atf_step');
  gr.get('f1a43c15db0123008096a455ca961915');
  var fields = gr.inputs.field_values.toString();
  gs.info(fields);
  fields = fields.replace('^EQ','^kb_knowledge_base=dfc19531bf2021003f07e2c1ac0739ab^EQ');
  gs.info(fields);
  gr.inputs.field_values = fields;
  gr.update();
  ```
