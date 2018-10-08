# OOB Automated Testing ![Discord](https://img.shields.io/discord/289994252241338369.svg) [![Discord Invite](https://img.shields.io/badge/discord-invite-green.svg)](https://discord.gg/QaMwnGd)

OOB Automated Testing is a scoped app to 
capture tests for all the Out of Box 
servicenow applications.

## Installation

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
  - Communities
  - Customer Service
  - Field Service
- Governance, Risk , and Compliance (GRC)
  - [Audit](https://github.com/jacebenson/x_8821_atf/issues/25)
  - Policy and Compliance
  - [Risk](https://github.com/jacebenson/x_8821_atf/issues/33)
  - [Vendor Risk](https://github.com/jacebenson/x_8821_atf/issues/34)
- HR Service Delivery
  - Case and Knowledge
  - Employee Document
  - Employee Service Center
  - Enterpise Onboarding and Transistions
  - HR Integrations
- IT Business Management
  - Agile Development
  - Business Planning Portal
  - Cost
  - Enterprise Release Management
  - Financial
  - Project Portfolio
  - Scaled Agile Frameworkf (SAFe)
  - Test Management
  - Time Card
- IT Operations Management
  - Cloud Management
  - Discovery
  - Event Management
  - Operational Intelligence
  - Service Mapping
- IT Service Management
  - [Asset](https://github.com/jacebenson/x_8821_atf/issues/30)
  - Benchmarks
  - [Change](https://github.com/jacebenson/x_8821_atf/issues/19)
  - Continual Improvement
  - Contract
  - Expense Line
  - [x] Incident
  - [Incident Communications](https://github.com/jacebenson/x_8821_atf/issues/18)
  - ITSM Virtual Agent
  - On-call Scheduling
  - [Problem](https://github.com/jacebenson/x_8821_atf/issues/20)
  - Procurement
  - Product Catalog
  - Release
  - [Request](https://github.com/jacebenson/x_8821_atf/issues/21)
  - [Service Catalog](https://github.com/jacebenson/x_8821_atf/issues/22)
  - Service Desk
  - Service Level
  - Service Portfolio
  - Vendor Performance
  - Walk-up Experience
- Security Operations
  - Configuration Compliance
  - Security Incident Response
  - Threat Intelligence
  - Trusted Security Circles
  - Vulnerability Response
- Service Management
  - Coaching Loops
  - Facilities
  - Finance
  - Legal
  - Marketing
  - Planned Maintenance
  - Structured Problem Analysis
- [Software Asset Management](https://github.com/jacebenson/x_8821_atf/issues/26)

## Contributing

Pull requests are welcome. For major changes, 
please open an issue first to discuss what you 
would like to change.

### Setting up a pdi (personal developer instance)

Create an account on [https://developer.servicenow.com/](https://developer.servicenow.com/).
Than Request a Personal Developer Instance.

### Setting up the repo

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
* [Issues](https://github.com/jacebenson/x_8821_atf/issues)